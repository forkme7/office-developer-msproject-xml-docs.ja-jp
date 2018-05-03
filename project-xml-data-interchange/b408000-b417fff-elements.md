---
title: b408000 ～ b417fff 要素
TOCTitle: b408000 ～ b417fff 要素
ms:assetid: eb451420-0c38-4c84-8029-4a3261f24a01
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968719(v=office.12)
ms:contentKeyID: 16749792
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# b408000 ～ b417fff 要素

タスクレベルのエンタープライズ ユーザー設定フィールドの値。

    <b408000>
        CustomFieldValue
    </b408000>

## 属性

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>属性</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>DurationFormat</strong></p></td>
<td><p>期間ユーザー設定フィールド値の形式を指定します (日、週、月など)。詳細については、「<a href="durationformat-element.md">DurationFormat 要素</a>」を参照してください。</p></td>
</tr>
</tbody>
</table>


## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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
<p>最大 : 一意な要素名ごとに 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

テキスト値は必須です。このテキストは、タスクのエンタープライズ ユーザー設定フィールドの値を指定します。

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968475.note(ja-jp,office.12).gif" alt="Note" class="note" />メモ :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>テキスト値は、ユーザー設定フィールドの定義で必要なデータ型と一致する必要があります。</p></td>
</tr>
</tbody>
</table>


## 備考

エンタープライズ ユーザー設定フィールドの値を格納する XML 要素の名前は、ユーザー設定フィールド ID の 16 進表現に対応します。

表 1 に、10 進と 16 進両方の形式で、タスクレベルのエンタープライズ ユーザー設定フィールドのユーザー設定フィールド ID の有効な範囲を示します。

**表 1. タスクレベルのエンタープライズ ユーザー設定フィールド ID**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>ユーザー設定フィールド ID の範囲 (10 進)</th>
<th>ユーザー設定フィールド ID の範囲 (16 進)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>188776448 – 188841983</p></td>
<td><p>b408000 ～ b417fff</p></td>
</tr>
</tbody>
</table>


詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。

## 例

次の例に、エンタープライズ タスク ユーザー設定フィールド データの 3 つの異なる表現を示します。

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素</strong></th>
<th><strong>FieldID の 10 進値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>b408011</strong></p></td>
<td><p>188776465</p></td>
<td><p><strong>FieldName</strong>: TaskNumberTest、参照テーブルのある数値のユーザー設定フィールド。</p>
<p><strong>Guid</strong> : ユーザー設定フィールド GUID を参照します。</p>
<p><strong>DefaultGuid</strong>: TaskNumberTest ユーザー設定フィールドの関連付けられた参照テーブルの既定値を参照します。</p>
<p><strong>b408011</strong> 要素の GUID 値は、実際の参照テーブルの値を指定します。</p></td>
</tr>
<tr class="even">
<td><p><strong>b408013</strong></p></td>
<td><p>188776467</p></td>
<td><p><strong>FieldName</strong>: TaskCostNL、参照テーブルのないコスト ユーザー設定フィールド。</p>
<p><strong>b408013</strong> 要素の値は 7000 です。Project Professional の米国英語インストールでは、この値は $70.00 と表示されます。</p></td>
</tr>
<tr class="odd">
<td><p><strong>b408015</strong></p></td>
<td><p>188776469</p></td>
<td><p><strong>FieldName</strong>: TaskDurationNL、参照テーブルのない期間ユーザー設定フィールド。</p>
<p><strong>DurationFormat</strong>=&quot;7&quot; 属性は、期間の形式を日として指定します。</p>
<p>値 PT40H0M0S は、40 時間、0 分、0 秒を指定します。稼働日は 8 時間であるため、5 日に相当します。(PT は Project Time (プロジェクト時間) の略、内部用)。</p>
<p>Project Professional はユーザー設定フィールドの値を &quot;5 日&quot; として表示します。</p></td>
</tr>
</tbody>
</table>


``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>188776465</FieldID>
         <FieldName>TaskNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>DE6BF35E-9D93-40EC-A1A4-72506A9CFBDC</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885321</SecondaryPID>
         <AutoRollDown>1</AutoRollDown>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>188776467</FieldID>
         <FieldName>TaskCostNL</FieldName>
         <CFType>0</CFType>
         <Guid>8E00874F-EA6F-4FED-BBB7-332BCCA44B3E</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885323</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>188776469</FieldID>
         <FieldName>TaskDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>BBC34DFF-D929-4CF3-8335-EFDA2DD38F11</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885325</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <b408011>D3561646-A7F0-4196-B211-E67E232A46EC</b408011>
         <b408013>7000</b408013>
         <b408015 DurationFormat="7">PT40H0M0S</b408015>
         . . .
      </Task>
   </Tasks>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)

