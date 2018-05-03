---
title: BCWP 要素
TOCTitle: BCWP 要素
ms:assetid: e4f0b550-4c8a-4d66-8041-6bed732a03a6
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968714(v=office.12)
ms:contentKeyID: 16749264
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# BCWP 要素

**BCWP** は実績作業の予算コストです。

** Task** の場合、**BCWP** は、状況報告日または今日の日付までの、タスクの時間単位の達成率に、タスクの時間単位の基準コストを掛けた累計値です。

** Resource** の場合は、状況報告日または今日の日付までで計算された、すべての割り当てタスクに対するリソースの BCWP 値を重ね合わせたサマリーです。

** Assignment** の場合は、日付への割り当てに対する実際作業時間です。

** Task** の ** Baseline ** の場合、**BCWP** は、状況報告日または今日の日付までの、タスクの時間単位の達成率に、タスクの時間単位の基準コストを掛けた累計値です。

** Resource** の ** Baseline ** の場合は、日付へのプロジェクトに対するリソースによる実際作業時間です。

** Assignment** の ** Baseline ** の場合は、日付への割り当てに対する実際作業時間です。

    <BCWP>
      DecimalValue
    </BCWP>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a>、<a href="baseline-element.md">Baseline</a></p></td>
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


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

