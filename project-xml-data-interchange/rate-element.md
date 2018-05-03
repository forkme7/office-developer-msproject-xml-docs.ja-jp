---
title: Rate 要素
TOCTitle: Rate 要素
ms:assetid: e9de4a2a-10e0-47f3-81e7-9f98ceafbb4a
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968716(v=office.12)
ms:contentKeyID: 16749679
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Rate 要素

期間の定義、およびその期間にリソースに対して適用される単価。

    <Rate>
      ComplexTypeValue
    </Rate>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="rates-element.md">Rates</a></p></td>
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
<td><p><a href="ratesfrom-element.md">RatesFrom</a></p></td>
<td><p>必須</p></td>
<td><p>単価が使用可能になる日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="ratesto-element.md">RatesTo</a></p></td>
<td><p>必須</p></td>
<td><p>単価が使用可能である最後の日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="ratetable-element.md">RateTable</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースのコスト単価テーブル (A ～ E) の一意識別子。</p></td>
</tr>
<tr class="even">
<td><p><a href="standardrate-element.md">StandardRate</a></p></td>
<td><p>オプション</p></td>
<td><p>定義された期間のリソースの標準支払単価。</p></td>
</tr>
<tr class="odd">
<td><p><a href="standardrateformat-element.md">StandardRateFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>標準単価を表示するために使用される単位。</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimerate-element.md">OvertimeRate</a></p></td>
<td><p>オプション</p></td>
<td><p>定義された期間のリソースの超過単価。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimerateformat-element.md">OvertimeRateFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>超過時間料金の表示に使用される単位。</p></td>
</tr>
<tr class="even">
<td><p><a href="costperuse-element.md">CostPerUse</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの導入コスト。</p></td>
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
<p>最大 : 25</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

