---
title: 新しい XML 要素
TOCTitle: 新しい XML 要素
ms:assetid: 8c9c7788-53b1-460f-88b5-c8f4f4fdedf7
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968581(v=office.12)
ms:contentKeyID: 16741864
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# 新しい XML 要素

Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) には、Office Project 2007 の新機能や拡張機能をサポートする新しい XML 要素が含まれています。

## Project 2007 の新しい XML 要素

以下のセクションでは、Project 2007 の Project XML データ交換スキーマに加わった新しい要素について簡単に説明します。また、Project 2007 にはユーザー設定フィールドの一部情報を XML で表現する方法の変更も盛り込まれています。詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。

この記事では、このスキーマ リファレンスの編成と同じく、以下のセクション内の新しい要素をアルファベット順にまとめます。XML 要素の構造の詳細については、「[Project データ交換の要素](project-data-interchange-elements.md)」を参照してください。

  - 表 1 : 新しい Project 要素

  - 表 2 : 新しい OutlineCode 要素

  - 表 3 : 新しい ExtendedAttribute 要素

  - 表 4 : 新しい Calendar 要素

  - 表 5 : 新しい Task 要素

  - 表 6 : 新しい Resource 要素

  - 表 7 : 新しい Assignment 要素

**表 1 : 新しい Project 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>CurrencyCode</strong></p></td>
<td><p>ISO 4217 通貨コード データに対する上位互換性を提供します。</p></td>
</tr>
<tr class="even">
<td><p><strong>SaveVersion</strong></p></td>
<td><p>XML ファイルの保存元 Project のバージョン。</p></td>
</tr>
</tbody>
</table>


**表 2 : 新しい OutlineCode 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>FieldGUID</strong></p></td>
<td><p>アウトライン コード値のグローバル一意識別子 (GUID)。</p></td>
</tr>
<tr class="even">
<td><p><strong>Guid</strong></p></td>
<td><p>アウトライン コードの GUID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>アウトライン コードの種類。</p></td>
</tr>
</tbody>
</table>


**表 3 : 新しい ExtendedAttribute 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>AutoRollDown</strong></p></td>
<td><p>割り当てへの自動細分化が有効になっているかどうか。</p></td>
</tr>
<tr class="even">
<td><p><strong>CFType</strong></p></td>
<td><p>ユーザー設定フィールドの種類です。</p></td>
</tr>
<tr class="odd">
<td><p><strong>ElemType</strong></p></td>
<td><p>ユーザー設定フィールドの関連付け。</p></td>
</tr>
<tr class="even">
<td><p><strong>DefaultGuid</strong></p></td>
<td><p>既定のユーザー設定フィールド値の GUID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Guid</strong></p></td>
<td><p>ユーザー設定フィールドの GUID。</p></td>
</tr>
<tr class="even">
<td><p><strong>Ltuid</strong></p></td>
<td><p>ユーザー設定フィールドに関連付けられた参照テーブルの GUID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>MaxMultiValues</strong></p></td>
<td><p>候補リストから選択できるアイテムの最大数。</p></td>
</tr>
<tr class="even">
<td><p><strong>Phonetic</strong></p></td>
<td><p>ユーザー設定フィールド名のふりがな情報。</p></td>
</tr>
<tr class="odd">
<td><p><strong>SecondaryPID</strong></p></td>
<td><p>ユーザー設定フィールドのセカンダリ PID。</p></td>
</tr>
<tr class="even">
<td><p><strong>UserDef</strong></p></td>
<td><p>ユーザー設定フィールドがユーザー定義であるかどうか。</p></td>
</tr>
</tbody>
</table>


**表 4 : 新しい Calendar 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>DaysOfWeek</strong></p></td>
<td><p>例外が有効な曜日。</p></td>
</tr>
<tr class="even">
<td><p><strong>EnteredByOccurrences</strong></p></td>
<td><p>例外の繰り返し回数が、数で定義されるか、終了日で定義されるか。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Exception</strong></p></td>
<td><p>カレンダーの例外を定義する要素を含みます。</p></td>
</tr>
<tr class="even">
<td><p><strong>Exceptions</strong></p></td>
<td><p>カレンダーの例外のコレクションを含みます。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Month</strong></p></td>
<td><p>例外の繰り返しがスケジュールされる月。</p></td>
</tr>
<tr class="even">
<td><p><strong>MonthDay</strong></p></td>
<td><p>例外の繰り返しがスケジュールされる日。</p></td>
</tr>
<tr class="odd">
<td><p><strong>MonthItem</strong></p></td>
<td><p>例外の繰り返しがスケジュールされる月アイテム。</p></td>
</tr>
<tr class="even">
<td><p><strong>MonthPosition</strong></p></td>
<td><p>月アイテムの月内での位置です。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Name</strong> (親 <strong>Exception</strong>)</p></td>
<td><p>例外の名前。</p></td>
</tr>
<tr class="even">
<td><p><strong>Name</strong> (親 <strong>WorkWeek</strong>)</p></td>
<td><p>有効稼働日の名前。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Occurrences</strong></p></td>
<td><p>例外の発生回数。</p></td>
</tr>
<tr class="even">
<td><p><strong>Period</strong></p></td>
<td><p>例外が繰り返される期間。</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>例外の種類。</p></td>
</tr>
<tr class="even">
<td><p><strong>WorkWeek</strong></p></td>
<td><p>有効稼働日を定義する要素を含みます。</p></td>
</tr>
<tr class="odd">
<td><p><strong>WorkWeeks</strong></p></td>
<td><p>カレンダーに関連付けられた有効稼働日のコレクションを含みます。</p></td>
</tr>
</tbody>
</table>


**表 5 : 新しい Task 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>CommitmentFinish</strong></p></td>
<td><p>成果物の終了日。</p></td>
</tr>
<tr class="even">
<td><p><strong>CommitmentStart</strong></p></td>
<td><p>成果物の開始日。</p></td>
</tr>
<tr class="odd">
<td><p><strong>CommitmentType</strong></p></td>
<td><p>タスクに、関連する成果物、または関連する成果物への依存関係があるかどうか。</p></td>
</tr>
<tr class="even">
<td><p><strong>FixedCost</strong></p></td>
<td><p>基準計画を保存したときのタスクの固定コストです。</p></td>
</tr>
<tr class="odd">
<td><p><strong>IsPublished</strong></p></td>
<td><p>タスクが発行済みかどうか。</p></td>
</tr>
<tr class="even">
<td><p><strong>StatusManager</strong></p></td>
<td><p>タスクの進捗管理者の名前。</p></td>
</tr>
</tbody>
</table>


**表 6 : 新しい Resource 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>AssnOwner</strong></p></td>
<td><p>割り当て所有者の名前。</p></td>
</tr>
<tr class="even">
<td><p><strong>AssnOwnerGuid</strong></p></td>
<td><p>割り当て所有者の GUID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>IsBudget</strong></p></td>
<td><p>リソースが予算リソースであるかどうか。</p></td>
</tr>
<tr class="even">
<td><p><strong>IsCostResource</strong></p></td>
<td><p>リソースがコスト型リソースであるかどうか。</p></td>
</tr>
</tbody>
</table>


**表 7 : 新しい Assignment 要素**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>要素名</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>AssnOwner</strong></p></td>
<td><p>割り当て所有者の名前。</p></td>
</tr>
<tr class="even">
<td><p><strong>AssnOwnerGuid</strong></p></td>
<td><p>割り当て所有者の GUID。</p></td>
</tr>
<tr class="odd">
<td><p><strong>BudgetCost</strong></p></td>
<td><p>この割り当てのコスト型リソースに対する予算コスト。</p></td>
</tr>
<tr class="even">
<td><p><strong>BudgetWork</strong></p></td>
<td><p>この割り当ての時間単価型リソースまたは数量単価型リソースに対する予算作業量。</p></td>
</tr>
<tr class="odd">
<td><p><strong>PeakUnits</strong></p></td>
<td><p>タスクにリソースを割り当てる単位の最大数。</p></td>
</tr>
<tr class="even">
<td><p><strong>Summary</strong></p></td>
<td><p>タスクがサマリー タスクであるかどうか。</p></td>
</tr>
<tr class="odd">
<td><p><strong>SV</strong></p></td>
<td><p>プロジェクトの状況報告日までの、達成額とスケジュールの差異です。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project XML データの概要](introduction-to-project-xml-data.md)  
[Project データ交換の要素](project-data-interchange-elements.md)

