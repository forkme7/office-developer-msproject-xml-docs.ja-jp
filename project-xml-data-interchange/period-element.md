---
title: Period 要素
TOCTitle: Period 要素
ms:assetid: 7a3c8c71-6993-4b8b-8b50-9743ea95e732
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968554(v=office.12)
ms:contentKeyID: 16740302
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Period 要素

カレンダー例外の反復の間隔。

    <Period>
      IntegerValue
    </Period>

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


## 例

次の例の **Period** 要素は、Team Meeting という名前のカレンダー例外が 2 週間に 1 回発生することを示しています。

``` xml
<Exception>
  <EnteredByOccurrences>1</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-12-26T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>52</Occurrences>
  <Name>Team Meeting</Name>
  <Type>6</Type>
  <Period>2</Period>
  <DaysOfWeek>8</DaysOfWeek>
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

