---
title: TimePeriod 要素 (Calendar)
TOCTitle: TimePeriod 要素 (Calendar)
ms:assetid: bded10b6-c40c-4d6e-83c2-0ec82dd3eac8
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968661(v=office.12)
ms:contentKeyID: 16745819
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# TimePeriod 要素 (Calendar)

例外日または稼働日を定義します。

    <TimePeriod>
      ComplexTypeValue
    </TimePeriod>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekday-element.md">WeekDay</a>、<a href="workweek-element.md">WorkWeek</a></p></td>
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
<td><p><a href="fromdate-element-calendar.md">FromDate</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの例外または稼働日の開始日。</p></td>
</tr>
<tr class="even">
<td><p><a href="todate-element-calendar.md">ToDate</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの例外または稼働日の終了日。</p></td>
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

カレンダーの例外と稼働日を含む例については、「[Calendar 要素](calendar-element.md)」を参照してください。

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

