---
title: BCWS 要素
TOCTitle: BCWS 要素
ms:assetid: 0e9e4541-0619-4545-bc05-63826397c10f
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968411(v=office.12)
ms:contentKeyID: 16731728
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# BCWS 要素

**BCWS** は予定作業の予算コストです。

** Task** の場合、**BCWS** は、状況報告日または今日の日付までの時間配分された累積コストです。

** Resource** の場合は、割り当てられたすべてのタスクに対するリソースの BCWS 値をまとめた合計です。

** Assignment** の場合は、割り当てに対する作業時間の予算コストです。

** Task** の ** Baseline ** の場合、**BCWS** は、状況報告日または今日の日付までの時間配分された累積基準コストです。

** Resource** の ** Baseline ** の場合は、リソースによって実行される作業時間の予算コストです。

** Assignment** の ** Baseline ** の場合、今日の日付までの割り当てに対する作業時間の予算コストです。

    <BCWS>
      DecimalValue
    </BCWS>

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

