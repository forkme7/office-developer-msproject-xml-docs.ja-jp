---
title: AutoRollDown 要素
TOCTitle: AutoRollDown 要素
ms:assetid: 1c644e22-6e35-4a74-a845-e7665a45da1b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968428(v=office.12)
ms:contentKeyID: 16732785
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# AutoRollDown 要素

ユーザー設定フィールドの割り当てレベルへの自動的な細分化が有効であるかどうかを示します。

    <AutoRollDown>
      BooleanValue
    </AutoRollDown>

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

## 例

以下の例では、**AutoRollDown** 要素を使用して、ユーザー設定フィールド Team Name の構成済みの値を割り当てレベルに細分化することを指定しています。

``` xml
<ExtendedAttribute>
  <FieldID>205553664</FieldID>
  <FieldName>Team Name</FieldName>
  <CFType>7</CFType>
  <Guid>0000740F-CF67-4B93-A405-F0C12C5BC942</Guid>
  <ElemType>21</ElemType>
  <MaxMultiValues>1</MaxMultiValues>
  <UserDef>1</UserDef>
  <SecondaryPID>255885312</SecondaryPID>
  <AutoRollDown>1</AutoRollDown>
</ExtendedAttribute>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

