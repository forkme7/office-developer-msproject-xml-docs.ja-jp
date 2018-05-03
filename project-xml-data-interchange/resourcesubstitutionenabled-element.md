---
title: ResourceSubstitutionEnabled 要素
TOCTitle: ResourceSubstitutionEnabled 要素
ms:assetid: 268bba0c-25fe-4d1b-b68f-87388ad411fa
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968443(v=office.12)
ms:contentKeyID: 16733559
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ResourceSubstitutionEnabled 要素

ユーザー設定アウトライン コードが Project のリソースの切り替えウィザードで使用されるかどうかを示します。エンタープライズ テキスト ユーザー設定フィールドとして追加されたアウトライン コードについてのみ使用されます。

    <ResourceSubstitutionEnabled>
      BooleanValue
    </ResourceSubstitutionEnabled>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
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
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>


## 備考

**ResourceSubstitutionEnabled** は、エンタープライズ リソース テキストユーザー設定フィールドとして Microsoft Office Project Server 2007 に追加されたリソース アウトライン コードについてのみ True になる場合があります。

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)

