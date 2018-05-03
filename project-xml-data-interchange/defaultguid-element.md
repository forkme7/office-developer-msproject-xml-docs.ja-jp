---
title: DefaultGuid 要素
TOCTitle: DefaultGuid 要素
ms:assetid: 22c2fd78-5409-4ce5-9e81-c62bd6403757
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968436(v=office.12)
ms:contentKeyID: 16733251
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# DefaultGuid 要素

既定の参照テーブル エントリの GUID を指定します。

    <DefaultGuid>
      StringValue
    </DefaultGuid>

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

**string** 型のテキスト値が必要です。この **string** 型の値は "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" の形式 (H は 0 ～ F の 16 進数値) である必要があります。

## 備考

## 例

以下の例では、**DefaultGuid** 要素を使用して、エンタープライズ ユーザー設定フィールド Health について、既定の参照テーブル値の GUID を指定しています。

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

