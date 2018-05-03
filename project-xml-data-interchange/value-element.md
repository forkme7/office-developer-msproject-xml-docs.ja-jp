---
title: Value 要素
TOCTitle: Value 要素
ms:assetid: d367ebe0-7f26-4e01-8c3b-b248996da52d
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968696(v=office.12)
ms:contentKeyID: 16747936
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Value 要素

** OutlineCode** 要素の場合、** Value ** はユーザー設定アウトライン コードの実際の値です。

** ExtendedAttribute** 要素の場合、**Value ** は拡張属性 (ユーザー設定フィールド) の実際の値です。

** TimephasedData** 要素の場合、**Value ** はタイムスケール データ レコードの各単位の値です。

    <Value>
      StringValue
    </Value>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="valuelist-element.md">ValueList</a>、<a href="values-element.md">Values</a>、<a href="extendedattribute-element.md">ExtendedAttribute</a>、TimephasedData</p></td>
</tr>
</tbody>
</table>


## OutlineCode 内での子要素

**OutlineCode** 要素内では、**Values** が **Value** 要素の親です。

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素</strong></th>
<th><strong>必須/オプション</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="valueid-element.md">ValueID</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定アウトライン コードの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldguid-element.md">FieldGUID</a></p></td>
<td><p>必須</p></td>
<td><p>Project 2007 の新しい要素。アウトライン コード値の GUID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>必須</p></td>
<td><p>Project 2007 の新しい要素。アウトライン コードの種類 (テキスト、日付、期間、フラグ、コスト、数)。</p></td>
</tr>
<tr class="even">
<td><p><a href="parentvalueid-element.md">ParentValueID</a> </p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定アウトライン コードの親ノードの一意の ID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Value</strong></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定アウトライン コードの実際の値。</p></td>
</tr>
<tr class="even">
<td><p><a href="description-element.md">Description</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定アウトライン コードの説明。</p></td>
</tr>
</tbody>
</table>


## ExtendedAttribute 内での子要素

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素</strong></th>
<th><strong>必須/オプション</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="id-element.md">ID</a> </p></td>
<td><p>必須</p></td>
<td><p>アウトライン コードまたはユーザー設定フィールドの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><strong>Value</strong></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードまたはユーザー設定フィールドの実際の値。</p></td>
</tr>
<tr class="odd">
<td><p><a href="description-element.md">Description</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードまたはユーザー設定フィールドの説明。</p></td>
</tr>
<tr class="even">
<td><p><a href="phonetic-element.md">Phonetic</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドまたはアウトライン コードの名前の読み方。</p></td>
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

**Value** は、** OutlineCode ** 内では ** Values ** 要素の一部として、** ExtendedAttribute ** 内では ** ValueList** 要素の一部として繰り返し使用されます。

**TimephasedData** 要素は、** Assignment **、** Baseline **、** Resource **、および ** Task ** 要素で使用されます。

**Value** の子要素は順不同です。

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)  
[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)  
[OutlineCode 要素](outlinecode-element.md)  
[Assignment 要素](assignment-element.md)  
[Baseline 要素](baseline-element.md)  
[Resource 要素](resource-element.md)  
[Task 要素](task-element.md)

