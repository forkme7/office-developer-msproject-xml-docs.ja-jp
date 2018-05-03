---
title: c408000 ～ c417fff 要素
TOCTitle: c408000 ～ c417fff 要素
ms:assetid: 603a3b7d-fa41-44eb-8aef-7cc99c54439c
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968524(v=office.12)
ms:contentKeyID: 16738234
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# c408000 ～ c417fff 要素

リソースレベルのエンタープライズ ユーザー設定フィールド値。

    <c408000>
        CustomFieldValue
    </c408000>

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
<td><p><a href="resource-element.md">Resource 要素</a></p></td>
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

テキスト値は必須です。テキストは、リソースのエンタープライズ ユーザー設定フィールド値を指定します。

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

**FieldID** 要素の 16 進表現に対応するエンタープライズ ユーザー設定フィールド値を格納する XML 要素の名前。

表 1 は、リソースレベルのエンタープライズ ユーザー設定フィールドのユーザー設定フィールド ID の有効な範囲を、10 進と 16 進の形式で示したものです。

**表 1. リソースレベルのエンタープライズ ユーザー設定フィールドの ID**

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
<td><p>205553664 – 205619199</p></td>
<td><p>c408000 ～ c417fff</p></td>
</tr>
</tbody>
</table>


詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。

## 例

以下の例では、エンタープライズ リソース ユーザー設定フィールド データの 3 種類の表現を示します。

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
<td><p><strong>c408008</strong></p></td>
<td><p>205553672</p></td>
<td><p><strong>FieldName</strong> : ResourceNumberTest、参照テーブルのある数値ユーザー設定フィールド。</p>
<p><strong>Guid</strong> : ユーザー設定フィールド GUID を参照します。</p>
<p><strong>DefaultGuid</strong> : 関連する参照テーブルで ResourceNumberTest ユーザー設定フィールドの既定値を参照します。</p>
<p><strong>c408008</strong> 要素の GUID 値は、実際の参照テーブルの値を指定します。</p></td>
</tr>
<tr class="even">
<td><p><strong>c40800b</strong></p></td>
<td><p>205553675</p></td>
<td><p><strong>FieldName</strong> : ResourceDateNL、参照テーブルのない日付ユーザー設定フィールド。</p>
<p>Project Professional のアメリカ英語版インストールでのユーザー設定フィールドの値は、&quot;Thu 11/8/07&quot; (2007 年 11 月 8 日木曜日) です。</p></td>
</tr>
<tr class="odd">
<td><p><strong>c40800c</strong></p></td>
<td><p>205553676</p></td>
<td><p><strong>FieldName</strong> : ResourceDurationNL、参照テーブルのない期間ユーザー設定フィールド。</p>
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
         <FieldID>205553672</FieldID>
         <FieldName>ResourceNumberTest</FieldName>
         <CFType>5</CFType>
         <Guid>F570EA97-EE3E-4D5D-8444-B9DCDA75ADD0</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885332</SecondaryPID>
         <AutoRollDown>1</AutoRollDown>
         <DefaultGuid>EBDF240A-AE0B-4224-A8B8-3FA4B7EA709F</DefaultGuid>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>205553675</FieldID>
         <FieldName>ResourceDateNL</FieldName>
         <CFType>1</CFType>
         <Guid>303073AE-54FC-429B-9105-E9407E2BE7F2</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885335</SecondaryPID>
         <RollupType>0</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
      <ExtendedAttribute>
         <FieldID>205553676</FieldID>
         <FieldName>ResourceDurationNL</FieldName>
         <CFType>2</CFType>
         <Guid>C7FFB2E7-9BA1-4A0D-97A8-8EFB8F0BD286</Guid>
         <ElemType>21</ElemType>
         <MaxMultiValues>1</MaxMultiValues>
         <UserDef>1</UserDef>
         <SecondaryPID>255885336</SecondaryPID>
         <RollupType>3</RollupType>
         <CalculationType>1</CalculationType>
         <AutoRollDown>1</AutoRollDown>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Resources>
      <Resource>
         . . .
         <c408008>C0141D97-54F0-4CBD-97A6-48611227CD81</c408008>
         <c40800b>2007-11-08T08:00:00</c40800b>
         <c40800c DurationFormat="9">PT280H0M0S</c40800c>
         . . .
      </Resource>
   </Resources>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)

