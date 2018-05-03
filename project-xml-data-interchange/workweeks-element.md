---
title: WorkWeeks 要素
TOCTitle: WorkWeeks 要素
ms:assetid: 4be76fb8-eb91-4f77-8447-4e2153e0e3d9
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968496(v=office.12)
ms:contentKeyID: 16736609
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WorkWeeks 要素

稼働日の定義のコレクションが含まれます。

    <WorkWeeks>
    </WorkWeeks>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="exception-element.md">Exception</a></p></td>
</tr>
</tbody>
</table>


## 子要素


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workweek-element.md">WorkWeek</a></p></td>
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
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## 備考

**WorkWeeks** 要素を使用する例については、「[Calendar 要素](calendar-element.md)」を参照してください。

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
<td><p>Project 2007 SP1 までのリリースでは、既定以外の稼働日を持つプロジェクトを XML として保存すると、<strong>WorkWeeks</strong> 要素名が失われます。XML ファイルを Project で開こうとすると、&quot;ファイルを読み込み中に予期しない問題が発生しました。このファイルは壊れている可能性があります。&quot;というエラー メッセージが表示されます。この回避策としては、XML ファイルを編集して、次の例に示すように <strong>WorkWeeks</strong> 要素名を追加します。これで、XML ファイルは正常に開きます。ただし、<strong>WorkWeek</strong> 要素には他のエラーも含まれているので、今後のサービス パックでエラーが修正されるまでは、稼働日を保存する場合は Project XML ファイルを使用しないことをお勧めします。他の稼働日要素の編集の詳細については、「<a href="workweek-element.md">WorkWeek 要素</a>」を参照してください。</p></td>
</tr>
</tbody>
</table>


## 例

次の例では、"Test work week" という名前の標準以外の稼働日を定義します。**WorkWeeks** の開始要素と終了要素は手動で編集されます。

``` xml
<Calendar>
   . . .
   <WorkWeeks>
      <WorkWeek>
         <TimePeriod>
            <FromDate>2007-11-26T00:00:00</FromDate>
            <ToDate>2007-11-26T23:59:00</ToDate>
         </TimePeriod>
         <Name>Test work week</Name>
      </WorkWeek>
   </WorkWeeks>
</Calendar>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

