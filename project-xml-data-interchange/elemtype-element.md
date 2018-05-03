---
title: ElemType 要素
TOCTitle: ElemType 要素
ms:assetid: b9db69dd-41c2-4247-9e88-efa1fa74cff1
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968655(v=office.12)
ms:contentKeyID: 16745508
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# ElemType 要素

ユーザー設定フィールド定義に関連付けられているエンティティの種類 (タスク、リソース、または割り当て) です。

    <ElemType>
      IntegerValue
    </ElemType>

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
<td><p>20</p></td>
<td><p>タスク</p></td>
</tr>
<tr class="even">
<td><p>21</p></td>
<td><p>リソース</p></td>
</tr>
<tr class="odd">
<td><p>23</p></td>
<td><p>割り当て</p></td>
</tr>
</tbody>
</table>


## 備考

ユーザー設定フィールド定義では、関連付けられているプロジェクト エンティティの種類を指定する必要があります。たとえば、Team Name という名前のユーザー設定フィールドの **ElemType** が 21 である場合、このフィールドはリソース エンティティと関連付けられています。エンタープライズ プロジェクト ユーザー設定フィールドの場合、プロジェクト内のすべてのタスクが同じユーザー設定フィールド値を取ります。

## 例

以下の例で、Health エンタープライズ ユーザー設定フィールドは **Text** 型で (**CFType** = 7)、タスク エンティティに関連付けられています (**ElemType** = 20)。**FieldID** の 10 進値は、タスク内の **b408001** 要素名に対応しています。ここで、タスク **UID** 1 の参照テーブル値は "On Schedule" であり、タスク **UID** 2 の参照テーブル値は "Late" です。

Plant ID エンタープライズ プロジェクト ユーザー設定フィールド値は、プロジェクト サマリー タスクを含めたすべてのタスクに関連付けられています (**UID** = 0)。**FieldID** の 10 進値 190873613 は、**b60800d** 要素名の 16 進値です。Plant ID エンタープライズ ユーザー設定フィールド値は、すべてのタスクにおいて "Plant 47" です。

``` xml
<ExtendedAttributes>
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
   <ExtendedAttribute>
      <FieldID>190873613</FieldID>
      <FieldName>Plant ID</FieldName>
      <CFType>7</CFType>
      <Guid>F162D66B-BF32-4030-998D-C2AA7BEAD285</Guid>
      <ElemType>20</ElemType>
      <MaxMultiValues>1</MaxMultiValues>
      <UserDef>1</UserDef>
   </ExtendedAttribute>
</ExtendedAttributes>
. . .
<Tasks>
   <Task>
      <UID>0</UID>
      <ID>0</ID>
      . . .
      <b60800d>Plant 47</b60800d>
   </Task>
   <Task>
      <UID>1</UID>
      <ID>1</ID>
      . . .
      <b408001>0000BB21-B2AE-410A-88B6-82C108903823</b408001>
      <b60800d>Plant 47</b60800d>
   </Task>
   <Task>
      <UID>2</UID>
      <ID>2</ID>
      . . .
      <b408001>0000C45D-8A43-4EB0-9B74-E535B391988A</b408001>
      <b60800d>Plant 47</b60800d>
   </Task>
</Tasks>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

