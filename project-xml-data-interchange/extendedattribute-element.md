---
title: ExtendedAttribute 要素
TOCTitle: ExtendedAttribute 要素
ms:assetid: c16eb20b-416e-4659-9d5a-2c006a45a1fb
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968669(v=office.12)
ms:contentKeyID: 16746092
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# ExtendedAttribute 要素

拡張属性は、Microsoft Office Project ではユーザー設定フィールドやアウトライン コードです。拡張属性は、ローカル ユーザー設定フィールドやアウトライン コード、またはエンタープライズ ユーザー設定フィールドである場合があります。定義は、拡張属性が ** ExtendedAttributes ** コレクションで定義されたか、それとも** Task**、** Resource**、または ** Assignment** で定義されたかによって異なります。一般に、拡張属性の数に制限はありませんが、制約について解説セクションで説明します。

    <ExtendedAttribute>
      ComplexTypeValue
    </ExtendedAttribute>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattributes-element.md">ExtendedAttributes</a>、<a href="task-element.md">Task</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a></p></td>
</tr>
</tbody>
</table>


## ExtendedAttributes コレクションの子要素


<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>オプション</p></td>
<td><p>ローカル ユーザー設定フィールドの列挙値に対応 (Text1、Text2 など)。<strong>FieldID</strong> は複数のプロジェクトで一意ではありません。</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldname-element.md">FieldName</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定フィールドの名前。</p></td>
</tr>
<tr class="odd">
<td><p><a href="cftype-element.md">CFType</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドの種類 (コスト、日付、期間、終了、フラグ、数、開始、またはテキスト)。</p></td>
</tr>
<tr class="even">
<td><p><a href="guid-element-multiple-parents.md">Guid</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドの GUID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="elemtype-element.md">ElemType</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドに関連付けられているエンティティの種類 (タスク、リソース、または割り当て)。</p></td>
</tr>
<tr class="even">
<td><p><a href="maxmultivalues-element.md">MaxMultiValues</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールド値リストで選択できる値の最大数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="userdef-element.md">UserDef</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドがユーザーによって定義されたものかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="alias-element.md">Alias</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定フィールドのエイリアス。</p></td>
</tr>
<tr class="odd">
<td><p><a href="secondarypid-element.md">SecondaryPID</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。割り当てを細分化する場合のユーザー設定フィールドのセカンダリ プロジェクト識別子 (PID)。</p></td>
</tr>
<tr class="even">
<td><p><a href="autorolldown-element.md">AutoRollDown</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールド値を割り当てレベルに自動的に細分化するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultguid-element.md">DefaultGuid</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。既定の参照テーブル エントリの GUID を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="ltuid-element.md">Ltuid</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールドに関連付けられた参照テーブルの GUID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="phoneticalias-element.md">PhoneticAlias</a></p></td>
<td><p>オプション</p></td>
<td><p>ひらがなまたはカタカナのいずれかで示した拡張属性の読み方。Project の日本語版でのみ使用します。</p></td>
</tr>
<tr class="even">
<td><p><a href="rolluptype-element.md">RollupType</a></p></td>
<td><p>オプション</p></td>
<td><p>サマリー タスクへの重ね合わせの計算に使用するメソッドを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="calculationtype-element.md">CalculationType</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクおよびグループのサマリー行の重ね合わせを計算するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="formula-element.md">Formula</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定フィールドに入力するために Project で使用される式。</p></td>
</tr>
<tr class="odd">
<td><p><a href="restrictvalues-element.md">RestrictValues</a></p></td>
<td><p>オプション</p></td>
<td><p>ファイルで使用できる値をリスト内の値に限定するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="valuelistsortorder-element.md">ValuelistSortOrder</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。値リストの並び順を示します (降順または昇順)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="appendnewvalues-element.md">AppendNewValues</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトに追加された新しい値を、リストに自動的に追加するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="default-element-extendedattribute.md">Default</a></p></td>
<td><p>オプション</p></td>
<td><p>リスト内の既定値の ID を参照します。既定セットがない場合、この要素は使用されません。</p></td>
</tr>
<tr class="odd">
<td><p><a href="valuelist-element.md">ValueList</a></p></td>
<td><p>オプション</p></td>
<td><p>拡張属性値のコレクション。</p></td>
</tr>
</tbody>
</table>


## Task、Resource、または Assignment の子要素

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>拡張属性のフィールド ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="value-element.md">Value 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>拡張属性の実際の値。</p></td>
</tr>
<tr class="odd">
<td><p><a href="durationformat-element.md">DurationFormat 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>拡張属性で使用できる期間形式の列挙 (日、週、月など)。</p></td>
</tr>
<tr class="even">
<td><p><a href="valueguid-element.md">ValueGUID</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーザー設定フィールド値リスト内の値の GUID。複数値ユーザー設定フィールドの場合、<strong>ValueGUID</strong> は、<strong>Value</strong> 要素内の <strong>FieldGUID</strong> と一致します。</p></td>
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
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 備考

タスク、リソース、または割り当てで **ExtendedAttribute** の値を指定するには、次の 2 つのデータが必要です。

  - **FieldID** 要素によって指定される拡張属性定義へのポインタ。

  - **Value** 要素によって、または値リスト内の **Value** 要素への **ValueGUID** ポインタによって指定される、ユーザー設定フィールド値。**ValueGUID** は、値リストの **FieldGUID** と一致します。

ユーザー設定フィールドの型が **Duration** である場合、その値には **DurationFormat** 要素が必要です。ユーザー設定フィールドが式によって計算される場合、**ValueGUID** は次の値になります。`<ValueGUID>00000000-0000-0000-0000-000000000000</ValueGUID>`

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
<td><p>XML データとして保存されたプロジェクトを読み込む場合、Microsoft Office Project では最大 5000 の <strong>ValueList</strong> 要素が認識されます。それを超える部分はすべて無視されます。</p></td>
</tr>
</tbody>
</table>


## 例

**FieldName** 値は **FieldID** 要素内の **PjCustomField** 列挙値に対応しています。たとえば、Information ローカル ユーザー設定フィールドの **FieldID** 188743731 は [PjCustomField (英語)](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx) 内の **pjCustomTaskText1** 値に一致します。

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
<td><p><strong>FieldID</strong> 205521019 は、現在のところ <strong>PjCustomField</strong> のドキュメントに記載されていません。ただし、Project Visual Basic Editor (VBE) のオブジェクト ブラウザでは見ることができます。これは <strong>pjCustomResourceCost1</strong> を表す値です。</p></td>
</tr>
</tbody>
</table>


``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188743731</FieldID>
      <FieldName>Text1</FieldName>
      <Alias>Information</Alias>
      <Ltuid>6F76DA0E-4294-467A-9A66-5E2909578CE8</Ltuid>
      <SecondaryPID>255869028</SecondaryPID>
      <DefaultGuid>D2C35FC6-639A-4F88-A1FF-987F432F3A9D</DefaultGuid>
   </ExtendedAttribute>
   <ExtendedAttribute>
      <FieldID>205521019</FieldID>
      <FieldName>Cost1</FieldName>
      <Alias>Extra Cost</Alias>
      <Ltuid>06AC981F-E8E6-4F20-A26F-8A408A36660B</Ltuid>
      <SecondaryPID>255852663</SecondaryPID>
      <AutoRollDown>1</AutoRollDown>
   </ExtendedAttribute>
</ExtendedAttributes>
. . .
<Tasks>
   <Task>
      <UID>1</UID>
      <ID>1</ID>
      <Name>T1</Name>
      . . .
      <ExtendedAttribute>
         <FieldID>188743731</FieldID>
         <Value>Info 1</Value>
         <ValueGUID>D2C35FC6-639A-4F88-A1FF-987F432F3A9D</ValueGUID>
      </ExtendedAttribute>
   </Task>
   </Task>
</Tasks>
. . .
<Resources>
   <Resource>
      <UID>1</UID>
      <ID>1</ID>
      <Name>R1</Name>
      . . .
      <ExtendedAttribute>
         <FieldID>205521019</FieldID>
         <Value>3000</Value>
         <ValueGUID>1EBF58AF-8EF0-400C-8E36-78628FF0E21C</ValueGUID>
      </ExtendedAttribute>
   </Resource>
</Resources>
```

## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)  
[OutlineCode 要素](outlinecode-element.md)

