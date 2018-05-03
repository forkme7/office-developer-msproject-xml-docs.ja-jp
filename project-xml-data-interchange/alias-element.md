---
title: Alias 要素
TOCTitle: Alias 要素
ms:assetid: 01c1a8dd-39cc-490d-84de-d75c4ba95fd1
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968395(v=office.12)
ms:contentKeyID: 16730702
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Alias 要素

ユーザー設定フィールドまたはアウトライン コードのエイリアスです。

    <Alias>
      String(50): for OutlineCode or ExtendedAttribute
    </Alias>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a>、<a href="outlinecode-element.md">OutlineCode</a></p></td>
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


## 例

次の例では、タスクの Duration6 というローカル ユーザー設定フィールドのエイリアスはテストの継続時間です。Microsoft Office Project では、このユーザー設定フィールドが一覧に \[テスト継続時間 (Duration6)\] と表示されます。

``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188743957</FieldID>
      <FieldName>Duration6</FieldName>
      <Alias>Test Duration</Alias>
      <SecondaryPID>255868973</SecondaryPID>
      <RollupType>3</RollupType>
      <CalculationType>1</CalculationType>
      <Formula>[Duration]*3</Formula>
   </ExtendedAttribute>
</ExtendedAttributes>
```

## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

