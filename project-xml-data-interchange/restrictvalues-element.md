---
title: RestrictValues 要素
TOCTitle: RestrictValues 要素
ms:assetid: a6aca4dd-c947-496f-bcce-a4742f73bab3
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968626(v=office.12)
ms:contentKeyID: 16743964
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# RestrictValues 要素

ユーザー設定フィールドの値がリスト内の値に制限されるかどうかを示します。

    <RestrictValues>
      BooleanValue
    </RestrictValues>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

`<RestrictValues>0</RestrictValues>` は、ユーザーがユーザー設定フィールドに追加の値を入力できることを意味します。

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

