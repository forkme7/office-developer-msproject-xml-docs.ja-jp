---
title: Formula 要素
TOCTitle: Formula 要素
ms:assetid: 5fe72a47-57ae-4871-9fc0-a9efbe596351
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968523(v=office.12)
ms:contentKeyID: 16738206
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Formula 要素

Microsoft Office Project がタスクのユーザー設定フィールドを設定するために使用する式。

    <Formula>
      StringValue
    </Formula>

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


## 例

次の例では、Test Duration タスクのユーザー設定フィールドは式 `[Duration]*3` を使用します。値は計算されるので、タスクでの **ValueGUID** はゼロです。プロジェクト サマリー タスク (タスク **UID** = 0) での **Value** は、168 時間、0 分、0 秒 (PT168H0M0S の PT は Project Time (プロジェクト時間) の略、内部用) です。サマリー タスクへの重ね合わせは、サブタスクの値の合計です (**RollupType** = 3)。

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
. . .
<Tasks>
   <Task>
      <UID>0</UID>
      <ID>0</ID>
      . . .
      <ExtendedAttribute>
         <FieldID>188743957</FieldID>
         <Value>PT168H0M0S</Value>
         <DurationFormat>21</DurationFormat>
         <ValueGUID>00000000-0000-0000-0000-000000000000</ValueGUID>
      </ExtendedAttribute>
   </Task>
</Tasks>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

