---
title: FieldID 要素
TOCTitle: FieldID 要素
ms:assetid: 3ed97e9e-cb2a-4aea-911c-a192b9e11891
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968474(v=office.12)
ms:contentKeyID: 16735555
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# FieldID 要素

** OutlineCode** では、** FieldID ** はアウトライン コードのフィールド番号 (プロジェクト ID、または PID) です。

** ExtendedAttribute** では、ローカル ユーザー設定フィールドの列挙値に対応します ("テキスト 1"、"テキスト 2"、"期間 1"、"期間 2"、など)。

    <FieldID>
        IntegerValue
    </FieldID>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="outlinecode-element.md">OutlineCode</a>、<a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

複数のプロジェクト間、または Microsoft Office Project の複数のバージョン間で一意であることを示す場合、**FieldID** は使用しないでください。

エンタープライズ ユーザー設定フィールドの場合、**FieldID** の整数値は、16 進数で表されるエンタープライズ ユーザー設定フィールド要素名を 10 進数で表したものです。たとえば、エンタープライズ リソース ユーザー設定フィールド要素が **c408005** の場合、**FieldID** 値は 205553669 です。詳細については、「[c408000 ～ c417fff 要素](c408000-c417fff-elements.md)」を参照してください。

ローカル ユーザー設定フィールドの場合、**FieldID** は **PjCustomField** 列挙値に対応します。たとえば、**FieldID** 188743731 は、「[PjCustomField Enumeration (英語)](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)」の **pjCustomTaskText1** 値と一致します。

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968475.note(ja-jp,office.12).gif" alt="Note" class="note" />メモ :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>FieldID</strong> の一部の値は現在、<strong>PjCustomField</strong> ドキュメントに記載されていません。ただし、Project Visual Basic Editor (VBE) のオブジェクト ブラウザで、すべての列挙値を検索できます。たとえば、<strong>FieldID</strong> 205521019 を検索すると、<strong>pjCustomResourceCost1</strong> となります。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[PjCustomField Enumeration (英語)](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)

