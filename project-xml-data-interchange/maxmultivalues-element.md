---
title: MaxMultiValues 要素
TOCTitle: MaxMultiValues 要素
ms:assetid: 56c818ed-8004-43a9-9339-45364ff93fee
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968512(v=office.12)
ms:contentKeyID: 16737472
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# MaxMultiValues 要素

ユーザー設定フィールド候補リストで選択できる値の最大数。

    <MaxMultiValues>
      IntegerValue
    </MaxMultiValues>

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

## 例

以下の例の **MaxMultiValues** 要素は、Health エンタープライズ ユーザー設定フィールドでは 1 つの値のみを選択できることを示しています。

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

