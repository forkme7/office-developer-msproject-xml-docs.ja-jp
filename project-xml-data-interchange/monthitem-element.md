---
title: MonthItem 要素
TOCTitle: MonthItem 要素
ms:assetid: 7fb52838-fb36-49d2-b078-556ae4d97021
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968560(v=office.12)
ms:contentKeyID: 16740793
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# MonthItem 要素

例外頻度をスケジュールする月アイテム。

    <MonthItem>
      IntegerValue
    </MonthItem>

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


## テキスト値

**integer** 型のテキスト値が必要です。

有効な値を表 1 に示します。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>値</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>日</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>週日</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>週末</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>日曜日</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>月曜日</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>火曜日</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>水曜日</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>木曜日</p></td>
</tr>
<tr class="odd">
<td><p>8</p></td>
<td><p>金曜日</p></td>
</tr>
<tr class="even">
<td><p>9</p></td>
<td><p>土曜日</p></td>
</tr>
</tbody>
</table>


## 例

次の例の **MonthItem** 要素は、Thanksgiving という名前のカレンダー例外が木曜日に発生することを示しています。

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-11-22T00:00:00</FromDate>
    <ToDate>2026-11-30T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>20</Occurrences>
  <Name>Thanksgiving</Name>
  <Type>3</Type>
  <Month>10</Month>
  <MonthItem>7</MonthItem>
  <MonthPosition>3</MonthPosition>
  <DayWorking>0</DayWorking>
</Exception>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

