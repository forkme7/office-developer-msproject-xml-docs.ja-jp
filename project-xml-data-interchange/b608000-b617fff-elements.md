---
title: b608000 ～ b617fff 要素
TOCTitle: b608000 ～ b617fff 要素
ms:assetid: 6c774043-2a50-47f8-97a0-815ade5bf2ad
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968536(v=office.12)
ms:contentKeyID: 16739201
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# b608000 ～ b617fff 要素

プロジェクトレベルのエンタープライズ ユーザー設定フィールドの値。

    <b608000>
        CustomFieldValue
    </b608000>

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

テキスト値は必須です。このテキストは、プロジェクトのエンタープライズ ユーザー設定フィールド値を指定します。

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

表 1 は、プロジェクト レベルのエンタープライズ ユーザー設定フィールドのユーザー設定フィールド ID の有効な範囲を、10 進と 16 進の形式で示したものです。

**表 1. プロジェクト レベルのエンタープライズ ユーザー設定フィールドの ID**

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
<td><p>190873600 – 190939135</p></td>
<td><p>b608000 ～ b617fff</p></td>
</tr>
</tbody>
</table>


詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。

## 例

以下の例では、エンタープライズ プロジェクト ユーザー設定フィールド データの 2 種類の表現を示します。

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
<td><p><strong>b608007</strong></p></td>
<td><p>190873607</p></td>
<td><p><strong>FieldName</strong> : ProjectNumberTest、参照テーブルのある数値ユーザー設定フィールド。</p>
<p><strong>Guid</strong> : ユーザー設定フィールド GUID を参照します。</p>
<p><strong>DefaultGuid</strong> : 関連する参照テーブルで ProjectNumberTest ユーザー設定フィールドの既定値を参照します。</p>
<p><strong>b608007</strong> 要素の GUID 値は、実際の参照テーブルの値を指定します。</p></td>
</tr>
<tr class="even">
<td><p><strong>b60800a</strong></p></td>
<td><p>205553676</p></td>
<td><p><strong>FieldName</strong> : ProjectDurationNL、参照テーブルのない期間ユーザー設定フィールド。</p>
<p><strong>DurationFormat</strong>=&quot;9&quot;という属性は、期間の形式が週であることを示します。</p>
<p>PT280H0M0S という値は、280 時間、0 分、0 秒を示します。1 週間の労働時間は 40 時間なので、これは 7 週間になります (PT は Project Time (プロジェクト時間) の略、内部用)。</p>
<p>Project Professional では、ユーザー設定フィールドの値は &quot;7 wks&quot; と示されます。</p></td>
</tr>
</tbody>
</table>


``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>190873607</FieldID>
         <FieldName>ProjectNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>7AA9C196-A0BB-4FA0-BBDD-E16B6C36901A</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>190873610</FieldID>
         <FieldName>ProjectDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>0FA0F636-98A0-4841-8129-08B84560E977</Guid>
         <ElemType>20</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <b608007>59B6725E-92B7-4242-9CCB-00AFA1B0A9C1</b608007>
         <b60800a DurationFormat="9">PT280H0M0S</b60800a>
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

