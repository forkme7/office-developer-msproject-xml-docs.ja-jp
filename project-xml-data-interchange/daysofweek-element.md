---
title: DaysOfWeek 要素
TOCTitle: DaysOfWeek 要素
ms:assetid: 83ab0be5-93bb-41c0-bf4c-4a4fce3d2cf5
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968569(v=office.12)
ms:contentKeyID: 16741106
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# DaysOfWeek 要素

例外が有効な曜日を指定します。

    <DaysOfWeek>
      IntegerValue
    </DaysOfWeek>

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
<td><p>1</p></td>
<td><p>日曜日</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>月曜日</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>火曜日</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>水曜日</p></td>
</tr>
<tr class="odd">
<td><p>16</p></td>
<td><p>木曜日</p></td>
</tr>
<tr class="even">
<td><p>32</p></td>
<td><p>金曜日</p></td>
</tr>
<tr class="odd">
<td><p>64</p></td>
<td><p>土曜日</p></td>
</tr>
</tbody>
</table>


## 備考

複数の曜日を表すには、値を追加します。たとえば、62 という値は、例外がすべての週日に発生することを示します (2 + 4 + 8 + 16 + 32 = 62)。

## 例

次の例の **DaysOfWeek** 要素は、カレンダー例外が火曜日と木曜日に発生することを示しています (4 + 16 = 20)。

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-12-28T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>104</Occurrences>
  <Name>Team Meeting </Name>
  <Type>6</Type>
  <Period>1</Period>
  <DaysOfWeek>20</DaysOfWeek>
  <DayWorking>1</DayWorking>
  <WorkingTimes>
    <WorkingTime>
      <FromTime>08:00:00</FromTime>
      <ToTime>12:00:00</ToTime>
    </WorkingTime>
    <WorkingTime>
      <FromTime>13:00:00</FromTime>
      <ToTime>14:00:00</ToTime>
    </WorkingTime>
    <WorkingTime>
      <FromTime>15:00:00</FromTime>
      <ToTime>16:00:00</ToTime>
    </WorkingTime>
  </WorkingTimes>
</Exception>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

