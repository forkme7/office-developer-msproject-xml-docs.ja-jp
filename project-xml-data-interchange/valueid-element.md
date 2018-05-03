---
title: ValueID 要素
TOCTitle: ValueID 要素
ms:assetid: 0b4257c5-1238-4f8d-81fa-6fe80bb5af3e
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968406(v=office.12)
ms:contentKeyID: 16731474
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ValueID 要素

**OutlineCode** では、** ValueID ** はアウトライン コード値のローカル ID です。

**ExtendedAttribute** では、拡張属性 (ユーザー設定フィールド) の値の ID です。**ValueID** はプロジェクト内でのみ一意です。

    <ValueID>
      IntegerValue
    </ValueID>

## 親要素

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

**ValueID** は、** OutlineCode** では ** Value ** 要素の子です。**Values** 要素には、** Value ** 要素のコレクションが含まれます。**ValueID** は、Project 2007 で保存された XML ファイルを Microsoft Office Project 2003 で読み取るために必要です。Project 2007 では、**ValueID** は無視され、**FieldGUID** が使用されます。

## 備考

**ExtendedAttribute** にも ** Value ** 要素が含まれていますが、この値は ** ValueList ** コレクションの一部です。** ExtendedAttribute ** の値は、** ValueID** ではなく、** ID** を持ちます。

## 参照

#### その他の技術情報

[FieldGUID 要素](fieldguid-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

