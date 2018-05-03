---
title: EnteredByOccurrences 要素
TOCTitle: EnteredByOccurrences 要素
ms:assetid: 81819336-f180-44ea-a4a4-c6140398d105
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968564(v=office.12)
ms:contentKeyID: 16740943
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# EnteredByOccurrences 要素

カレンダー例外の頻度の範囲が、発生回数または終了日のどちらで定義されているかを示します。

    <EnteredByOccurrences>
      BooleanValue
    </EnteredByOccurrences>

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

**boolean** 型のテキスト値が必要です。

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
<td><p>False。例外の頻度の範囲は、終了日で定義されています。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True。例外の頻度の範囲は、発生回数で定義されています。</p></td>
</tr>
</tbody>
</table>


## 備考

## 例

次の例では、**EnteredByOccurrences** 要素を使用して、このカレンダー例外は頻度の範囲が終了日で定義されて入力されたことを示しています。

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2007-01-01T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>1</Occurrences>
  <Name>New Year's Day</Name>
  <Type>1</Type>
  <DayWorking>0</DayWorking>
</Exception>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

