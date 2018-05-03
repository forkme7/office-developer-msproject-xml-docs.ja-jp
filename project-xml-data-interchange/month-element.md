---
title: Month 要素
TOCTitle: Month 要素
ms:assetid: 2d77e623-efaa-4695-a08f-1b64e8525292
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968450(v=office.12)
ms:contentKeyID: 16734144
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Month 要素

定期的な例外が予定されている月です。

    <Month>
      IntegerValue
    </Month>

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
<td><p>0</p></td>
<td><p>1 月</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>2 月</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>3 月</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>4 月</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>5 月</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>6 月</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>7 月</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>8 月</p></td>
</tr>
<tr class="odd">
<td><p>8</p></td>
<td><p>9 月</p></td>
</tr>
<tr class="even">
<td><p>9</p></td>
<td><p>10 月</p></td>
</tr>
<tr class="odd">
<td><p>10</p></td>
<td><p>11 月</p></td>
</tr>
<tr class="even">
<td><p>11</p></td>
<td><p>12 月</p></td>
</tr>
</tbody>
</table>


## 例

以下の例では、**Month** 要素を使用して、1 月に "New Year's Day" という名前のカレンダーの例外が発生することを示します。

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

