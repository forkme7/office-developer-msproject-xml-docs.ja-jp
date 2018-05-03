---
title: SecondaryPID 要素
TOCTitle: SecondaryPID 要素
ms:assetid: 3605321a-9c32-45a0-8b9d-b544a0b21c1b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968460(v=office.12)
ms:contentKeyID: 16734857
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# SecondaryPID 要素

ユーザー設定フィールドを割り当てへの細分化に使用するセカンダリ プロジェクト識別子 (PID) です。

    <SecondaryPID>
      StringValue
    </SecondaryPID>

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

**string** 型のテキスト値が必要です。

## 例

次の例では、**SecondaryPID** 要素は Health 社のユーザー設定フィールドの PID を表します。このフィールドは割り当てへの細分化に使用されます。

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

