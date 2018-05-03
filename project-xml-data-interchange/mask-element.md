---
title: Mask 要素
TOCTitle: Mask 要素
ms:assetid: bd78e7ac-a2b7-40a6-8e8a-2947ae8c01c3
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968659(v=office.12)
ms:contentKeyID: 16745787
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Mask 要素

すべてのリソースおよびタスクと共にユーザー設定アウトライン コードを使用する必要があるかどうかを示します。

    <Mask>
      ComplexTypeValue
    </Mask>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="masks-element.md">Masks</a></p></td>
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
<td><p><a href="level-element.md">Level</a></p></td>
<td><p>オプション</p></td>
<td><p>各アウトライン コード値に割り当てられたレベル。開始値は 1 です。</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>オプション</p></td>
<td><p>最初のレベルのタスクのコード文字列の種類です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="length-element.md">Length</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コード値の文字の最大長。使用できる値は 1 ～ 255。長さが任意の場合、値は 0 です。</p></td>
</tr>
<tr class="even">
<td><p><a href="separator-element.md">Separator</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コード レベルを区切るために使用される文字。</p></td>
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


## 備考

マスクの 4 つの要素によって、アウトライン コードの表示形式が決定されます。

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)

