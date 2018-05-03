---
title: WorkWeek 要素
TOCTitle: WorkWeek 要素
ms:assetid: 608d30fc-c808-40e6-b8b4-6d7f77397d7b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968525(v=office.12)
ms:contentKeyID: 16738267
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WorkWeek 要素

有効稼働日を定義する要素を含みます。

    <WorkWeek>
      ComplexTypeValue
    </WorkWeek>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workweeks-element.md">WorkWeeks</a></p></td>
</tr>
</tbody>
</table>


## 子要素


<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="timeperiod-element-calendar.md">TimePeriod</a></p></td>
<td><p>オプション</p></td>
<td><p>連続する一連の稼働日を定義します。</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>オプション</p></td>
<td><p>有効な週の名前です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="weekday-element.md">WeekDay</a></p></td>
<td><p>オプション</p></td>
<td><p>稼働日を定義します。</p></td>
</tr>
</tbody>
</table>


## 出現回数

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>最小 : 0</p>
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 備考

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968496.Caution(ja-jp,office.12).gif" alt="Caution note" class="note" />注意 :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Project 2007 SP1 までのリリースでは、XML として変更された稼働時間を含む稼働日のあるプロジェクトを保存するとき、<strong>WorkWeek</strong> 要素は閉じられません。また、変更した <strong>WorkingTimes</strong> 要素は保存されません。XML ファイルを Project で開こうとすると、&quot;ファイルを読み込み中に予期しない問題が発生しました。このファイルは壊れている可能性があります。&quot;というエラー メッセージが表示されます。XML ファイルを編集し、ファイルが有効で正常に開くようにすることができます。ただし、Project 2007 は変更された稼働時間を XML ファイルから正しく読み取ることができないので、今後のサービス パックでエラーが解決されるまでは、Project XML ファイルを使用して稼働日データを保存しないようお勧めします。</p></td>
</tr>
</tbody>
</table>


XML ファイルを開くことができるようにするには、ファイルを次のように編集します。

  - **WorkWeeks** セクションの空の開始要素と終了要素に、**WorkWeeks** の名前を追加します。

  - `</WeekDay>` を追加して、すべての **WeekDay** 要素を閉じます。

  - 足りない **WorkingTimes** セクションおよび子要素 **FromTime** と **ToTime** を追加します。

## 例

次の例では、手動で編集したセクション (太字の部分) とコメントを示します。この XML ファイルは Project で開くので、他のデータは使用できますが、稼働時間にはやはり既定の時間が表示されます。

``` xml
<Calendar>
   <Calendars>
      . . .
      <WorkWeeks>       <!-- Add element name-->
         <WorkWeek>
            <TimePeriod>
               <FromDate>2007-11-26T00:00:00</FromDate>
               <ToDate>2007-11-26T23:59:00</ToDate>
            </TimePeriod>
            <Name>Training day</Name>
            <WeekDay>
               <DayType>2</DayType>
               <DayWorking>1</DayWorking>
               <WorkingTimes>   <!-- Add modified working times-->
                  <WorkingTime><FromTime>14:00:00</FromTime><ToTime>17:00:00</ToTime></WorkingTime></WorkingTimes></WeekDay>    <!-- Add closing element -->
         </WorkWeek>
      </WorkWeeks>   <!-- Add element name-->
   </Calendar>
</Calendars>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

