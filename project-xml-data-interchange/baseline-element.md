---
title: Baseline 要素
TOCTitle: Baseline 要素
ms:assetid: 985cf3e5-7378-41a9-b1d8-ebf03c1584aa
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968599(v=office.12)
ms:contentKeyID: 16742841
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Baseline 要素

タスク、リソース、または割り当てに関連付けられた基準値のコレクション。

    <Baseline>
      ComplexTypeValue
    </Baseline>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a></p></td>
</tr>
</tbody>
</table>


## Task に対する子要素


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
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準計画に関連付けられたタイムスケール データ ブロック。</p></td>
</tr>
<tr class="even">
<td><p><a href="number-element.md">Number</a></p></td>
<td><p>必須</p></td>
<td><p>基準データ レコードの一意番号。</p></td>
</tr>
<tr class="odd">
<td><p><a href="interim-element.md">Interim</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画が中間計画であるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのタスクの予定開始日。</p></td>
</tr>
<tr class="odd">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのタスクの予定終了日。</p></td>
</tr>
<tr class="even">
<td><p><a href="duration-element.md">Duration</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのタスクの予定期間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="durationformat-element.md">DurationFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>タスク基準計画の期間を示す形式。</p></td>
</tr>
<tr class="even">
<td><p><a href="estimatedduration-element.md">EstimatedDuration</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの期間が見積もりであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのタスクの予定作業時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのタスクの予測コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p><strong>BCWS</strong> は予定作業の予算コストです。状況報告日または今日の日付までの時間単位の基準コストの累計です。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p><strong>BCWP</strong> は実績作業の予算コストです。タスクの時間単位の達成率に、タスクの時間単位の基準コストを掛けた、状況報告日または今日の日付までの累計値です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="fixedcost-element-baseline.md">FixedCost</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で <strong>Baseline</strong> に加わった新しい要素。基準計画を保存したときのタスクの固定コストです。</p></td>
</tr>
</tbody>
</table>


## Resource に対する子要素

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
<td><p><a href="number-element.md">Number</a></p></td>
<td><p>必須</p></td>
<td><p>基準データ レコードの一意番号。</p></td>
</tr>
<tr class="even">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのリソースに割り当てられた作業時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときのリソースの予測コスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの予定作業時間の予算コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがプロジェクトに関して現在までに行った作業の予算コスト。</p></td>
</tr>
</tbody>
</table>


## Assignment に対する子要素


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
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準計画に関連付けられたタイムスケール データ ブロック。</p></td>
</tr>
<tr class="even">
<td><p><a href="number-element.md">Number</a></p></td>
<td><p>必須</p></td>
<td><p>基準データ レコードの一意番号。</p></td>
</tr>
<tr class="odd">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときの割り当ての予定開始日。</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときの割り当ての予定終了日。</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときの割り当ての予定作業時間の合計。</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>基準計画を保存したときの割り当ての予測コストの合計。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての予定作業時間の予算コスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関して現在までに行われた作業の予算コスト。</p></td>
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


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

