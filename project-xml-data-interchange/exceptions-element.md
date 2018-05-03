---
title: Exceptions 要素
TOCTitle: Exceptions 要素
ms:assetid: a0b410df-e930-4b2c-89a2-823e2359f800
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968618(v=office.12)
ms:contentKeyID: 16743518
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Exceptions 要素

カレンダーに関連付けられる例外のコレクションです。

    <Exceptions>
      <Exception>…</Exception>
    </Exceptions>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendar-element.md">Calendar</a></p></td>
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

次の例では、2 つのカレンダーの例外の定義が **Exceptions** 要素に含まれています。New Year's Day は、日付 (**Type** = 2) によって毎年定義されています。Thanksgiving は、位置 (**Type** = 3) によって毎年定義されています。この休日は、11 月 (**Month** = 10) の 4 番目 (**MonthPosition** = 3) の木曜日 (**MonthItem** = 7) です。

``` xml
<Exceptions>
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
</Exceptions>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

