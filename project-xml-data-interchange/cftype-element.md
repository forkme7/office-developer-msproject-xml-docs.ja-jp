---
title: CFType 要素
TOCTitle: CFType 要素
ms:assetid: c4a58f3b-68ef-419f-9d73-1a50b5bc019e
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968675(v=office.12)
ms:contentKeyID: 16746349
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# CFType 要素

ユーザー設定フィールドの種類です。

    <CFType>
      IntegerValue
    </CFType>

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

**integer** 型のテキスト値が必要です。

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
<td><p>コスト</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>日付</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>期間</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>終了日</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>フラグ</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>数</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>開始日</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>テキスト</p></td>
</tr>
</tbody>
</table>


## 備考

## 例

以下の例では、**CFType** 要素を使用して、エンタープライズ Health ユーザー設定フィールドがテキスト フィールドであることを示します。

``` xml
<ExtendedAttribute>
  <FieldID>188776449</FieldID>
  <FieldName>Health</FieldName>
  <CFType>7</CFType>
  <Guid>0000E8D9-65F1-4769-9BD2-819D38036FCC</Guid>
  <ElemType>20</ElemType>
  <MaxMultiValues>1</MaxMultiValues>
  <UserDef>1</UserDef>
  <SecondaryPID>255885314</SecondaryPID>
  <DefaultGuid>000079D2-4A43-41FC-B264-98D23FADD84B</DefaultGuid>
</ExtendedAttribute>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

