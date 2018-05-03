---
title: Exception 要素
TOCTitle: Exception 要素
ms:assetid: 4918cdc1-9871-4124-8dba-6df6a7f49512
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968492(v=office.12)
ms:contentKeyID: 16736361
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Exception 要素

**Exception** 要素は、1 つのカレンダー例外を定義します。

    <Exception>
            ComplexTypeValue
    </Exception>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="exceptions-element.md">Exceptions</a></p></td>
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
<td><p><a href="enteredbyoccurrences-element.md">EnteredByOccurrences</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダー例外の頻度の範囲が、発生回数または終了日のどちらで定義されているかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="timeperiod-element-calendar.md">TimePeriod</a></p></td>
<td><p>オプション</p></td>
<td><p>一連の例外日を定義します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="occurrences-element.md">Occurrences</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの例外が有効になる回数。</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの例外の名前。</p></td>
</tr>
<tr class="odd">
<td><p>Type</p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの例外の種類 (毎日、毎年同じ日、毎月カレンダー上の固定位置にくる日、毎週、第何日目、など)。</p></td>
</tr>
<tr class="even">
<td><p><a href="period-element.md">Period</a></p></td>
<td><p>オプション</p></td>
<td><p>例外が繰り返される期間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="daysofweek-element.md">DaysOfWeek</a></p></td>
<td><p>オプション</p></td>
<td><p>例外が有効な曜日 (複数可) を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="monthitem-element.md">MonthItem</a></p></td>
<td><p>オプション</p></td>
<td><p>定期的な例外が予定されている月アイテム (日、週日、日曜日、月曜日、など)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="monthposition-element.md">MonthPosition</a></p></td>
<td><p>オプション</p></td>
<td><p>月の中の月アイテムの位置 (最初の、第 2、第 3、第 4、または最後の)。</p></td>
</tr>
<tr class="even">
<td><p><a href="month-element.md">Month</a></p></td>
<td><p>オプション</p></td>
<td><p>定期的な例外が予定されている月 (0 = 1 月、…、11 = 12 月)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="monthday-element.md">MonthDay</a></p></td>
<td><p>オプション</p></td>
<td><p>定期的な例外が予定されている日。</p></td>
</tr>
<tr class="even">
<td><p><a href="dayworking-element-calendar.md">DayWorking</a></p></td>
<td><p>オプション</p></td>
<td><p>指定された例外日の種類が稼働日であるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="workingtimes-element-calendar.md">WorkingTimes</a></p></td>
<td><p>オプション</p></td>
<td><p>稼働日の稼働時間を定義する稼働時間のコレクション。<strong>WorkingTime</strong> は最低でも 1 つ必要です。最大 5 つ定義できます。</p></td>
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


## 例

次の例では、**Exception** 要素は、2007 年 1 月 1 日から 2026 年 1 月 1 日まで、20 回の元日をカレンダーの例外として定義します。

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
     <ToDate>2026-01-01T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>20</Occurrences>
  <Name>New Year's Day</Name>
  <Type>2</Type>
  <Month>0</Month>
  <MonthDay>1</MonthDay>
  <DayWorking>0</DayWorking>
</Exception>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

