---
title: MonthPosition 要素
TOCTitle: MonthPosition 要素
ms:assetid: a48960a9-a435-423e-9a15-1f01ed366621
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968624(v=office.12)
ms:contentKeyID: 16743813
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# MonthPosition 要素

月アイテムの月内での位置です。

    <MonthPosition>
      IntegerValue
    </MonthPosition>

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
<td><p>第 1 位置</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>第 2 位置</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>第 3 位置</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>第 4 位置</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>最後の位置</p></td>
</tr>
</tbody>
</table>


## 例

以下の例では、**MonthPosition** 要素は、Thanksgiving という名前の例外が 11 月の第 4 木曜日に発生することを指定しています。

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

