---
title: ValueList 要素
TOCTitle: ValueList 要素
ms:assetid: d797b79a-8f07-4309-851c-fcf8ffce49d2
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968702(v=office.12)
ms:contentKeyID: 16748270
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ValueList 要素

拡張属性の値がスキーマの要素のプロパティとして指定されている場合、それらは値、またはリストに含まれる値への参照によって指定できます。アプリケーションは、**ValueListSortOrder** (昇順または降順) により指定される方法で順序付けられた値のリストを取ることができます。

    <ValueList>
      ComplexTypeValue
    </ValueList>

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


## 子要素


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="value-element.md">Value</a></p></td>
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

**ValueList** 要素には、** ExtendedAttribute** の **Value** 要素のコレクションが含まれます。**OutlineCode** 要素の ** Value ** 要素は、** Values** コレクションに含まれています。

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

