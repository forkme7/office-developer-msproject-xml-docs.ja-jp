---
title: Guid 要素 (複数の親)
TOCTitle: Guid 要素
ms:assetid: 24a60efb-8976-4308-b601-e5a285b8a79f
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968441(v=office.12)
ms:contentKeyID: 16733402
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Guid 要素 (複数の親)

アウトライン コードまたはエンタープライズ ユーザー設定フィールドのグローバル一意識別子 (GUID)。

    <Guid>
        StringValue
    <Guid>

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
<td><p>最小 : ローカル ユーザー設定フィールドの場合は 0、アウトライン コードおよびエンタープライズ ユーザー設定フィールドの場合は 1</p>
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

**string** 型のテキスト値が必要です。この **string** 型の値は "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" の形式 (H は 0 ～ F の 16 進数値) である必要があります。

## 備考

**ExtendedAttribute** 要素の場合、**Guid** はユーザー設定フィールドの GUID です。

**OutlineCode** 要素の場合、**Guid** はアウトライン コードの GUID です。ローカル アウトライン コードおよびエンタープライズ ユーザー設定フィールドでは **Guid** 要素が必要ですが、ローカル ユーザー設定フィールドでは必要ありません。

## 例

以下の例では、Text1 はローカル タスク ユーザー設定フィールドであり、**Guid** 要素は含まれていません。Health はエンタープライズ ユーザー設定フィールドであり、**Guid** 要素を使用してエンタープライズ ユーザー設定フィールドの GUID を表しています。

``` xml
<ExtendedAttributes>
  <ExtendedAttribute>
    <FieldID>188743731</FieldID>
    <FieldName>Text1</FieldName>
    <Alias>Test Task CF</Alias>
    <Ltuid>ED2E65AD-00A1-4457-97FA-A3FC708C9183</Ltuid>
    <SecondaryPID>255869028</SecondaryPID>
  </ExtendedAttribute>
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
</ExtendedAttributes>
```

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

