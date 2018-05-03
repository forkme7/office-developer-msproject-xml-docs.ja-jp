---
title: CurrencySymbolPosition 要素
TOCTitle: CurrencySymbolPosition 要素
ms:assetid: a800ac60-fceb-4aec-9d82-05c683b2e424
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968631(v=office.12)
ms:contentKeyID: 16744063
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# CurrencySymbolPosition 要素

通貨記号の位置です。

    <CurrencySymbolPosition>
      IntegerValue
    </CurrencySymbolPosition>

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
<td><p>前、スペースなし (既定)。例 : $0</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>後ろ、スペースなし。例 : 0$</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>前、スペースあり。例 : $ 0</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>後ろ、スペースあり。例 : 0 $</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

