---
title: Ltuid 要素
TOCTitle: Ltuid 要素
ms:assetid: 9c171e76-bf69-48e6-836d-7eb83080e430
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968607(v=office.12)
ms:contentKeyID: 16743147
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Ltuid 要素

ユーザー設定フィールドに関連付けられた参照テーブルのグローバル一意識別子 (GUID)。

    <Ltuid>
      StringValue
    </Ltuid>

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

**string** 型のテキスト値が必要です。この **string** は、"HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" の形式 ("H" は 0 ～ F の 16 進数を表します) になっている必要があります。

## 例

次の例では、**Ltuid** 要素を使用して、ローカル ユーザー設定フィールドに対して定義された参照テーブルの GUID を指定しています。

``` xml
<ExtendedAttribute>
  <FieldID>188743731</FieldID>
  <FieldName>Text1</FieldName>
  <Alias>MyLocalCustomField</Alias>
  <Ltuid>E8B19FF9-82ED-492C-A524-530640FBF913</Ltuid>
  <SecondaryPID>255869028</SecondaryPID>
  <DefaultGuid>0972C697-2DE3-46C5-8841-9CD7209989AE</DefaultGuid>
</ExtendedAttribute>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

