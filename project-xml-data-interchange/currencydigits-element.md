---
title: CurrencyDigits 要素
TOCTitle: CurrencyDigits 要素
ms:assetid: adb6f90f-bbe0-4843-994b-390255360400
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968638(v=office.12)
ms:contentKeyID: 16744515
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# CurrencyDigits 要素

Microsoft Office Project が通貨値を表示するときに、小数点の後ろに表示される桁数です。

    <CurrencyDigits>
      IntegerValue
    </CurrencyDigits>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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

**Integer** 型のテキスト値が必要です。

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
<td><p>小数点の後ろに桁を表示しません。例 : $0</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>小数点の後ろに 1 桁を表示します。例 : $0.0</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>小数点の後ろに 2 桁を表示します。例 : $0.00</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

