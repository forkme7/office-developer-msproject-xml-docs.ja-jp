---
title: AvailabilityPeriod 要素
TOCTitle: AvailabilityPeriod 要素
ms:assetid: a4c03ace-1ef0-41a7-92df-99abc612aa73
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968625(v=office.12)
ms:contentKeyID: 16743833
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# AvailabilityPeriod 要素

リソースが利用可能な期間を定義します。

    <AvailabilityPeriod>
      ComplexTypeValue
    </AvailabilityPeriod>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="availabilityperiods-element.md">AvailabilityPeriods</a></p></td>
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
<td><p><a href="availablefrom-element.md">AvailableFrom</a>、<a href="availableto-element.md">AvailableTo</a>、<a href="availableunits-element.md">AvailableUnits</a></p></td>
</tr>
</tbody>
</table>


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
<td><p><a href="availablefrom-element.md">AvailableFrom</a></p></td>
<td><p>オプション</p></td>
<td><p>現在の期間に指定されている単位数でリソースを作業に使用できる期間の開始日です。</p></td>
</tr>
<tr class="even">
<td><p><a href="availableto-element.md">AvailableTo</a></p></td>
<td><p>オプション</p></td>
<td><p>現在の期間に指定されている単位数で、リソースを作業に利用できる期間の終了日です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="availableunits-element.md">AvailableUnits</a></p></td>
<td><p>オプション</p></td>
<td><p>指定された期間内にリソースを利用できるパーセンテージです。</p></td>
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
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

