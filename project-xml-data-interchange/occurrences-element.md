---
title: Occurrences 要素
TOCTitle: Occurrences 要素
ms:assetid: e04aaef6-8207-47a9-8711-a66e628ad2ae
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968710(v=office.12)
ms:contentKeyID: 16748899
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Occurrences 要素

カレンダーの例外が有効である出現回数。

    <Occurrences>
      IntegerValue
    </Occurrences>

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

次の例では、**Occurrences** 要素は、カレンダーの例外は 1 回のみ出現することを示しています。

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

