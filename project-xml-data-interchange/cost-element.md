---
title: Cost 要素
TOCTitle: Cost 要素
ms:assetid: 5e1959e5-0af9-4ea1-bbe7-33c7d277cfbd
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968522(v=office.12)
ms:contentKeyID: 16738072
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Cost 要素

** Task** の場合、** Cost **はタスクの総計画 (または予測) コストです。このコストは、そのタスクに割り当てられたすべてのリソースが既に終了した作業のコストと、割り当ての残存作業の計画コストを合計したものです。

** Resource** の場合は、特定のリソースに割り当てられたすべてのタスクに関するそのリソースの総計画コストです。このコストは、割り当てられたすべてのタスクでそのリソースが既に終了した作業のコストと、残存作業の計画コストを合計したものです。

** Assignment** の場合は、基準計画を保存した時点での割り当ての総予測コストです。

** Baseline** の場合は、割り当ての総計画 (または予測) コストです。このコストは、リソースがタスクで既に終了した作業のコストと、割り当ての残存作業の計画コストを合計したものです。

    <Cost>
      DecimalValue
    </Cost>

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

