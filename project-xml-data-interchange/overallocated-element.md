---
title: OverAllocated 要素
TOCTitle: OverAllocated 要素
ms:assetid: 9f8faa7d-0f6a-4822-99a0-aaf381af279b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968615(v=office.12)
ms:contentKeyID: 16743420
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# OverAllocated 要素

** Task** の場合、** Overallocated **は、タスクの割り当てリソースにそのタスクで割り当てられている作業量が、通常作業可能な量を超えているかどうかを示します。

**Resource** の場合は、リソースにすべてのタスクで割り当てられている作業量が、通常作業可能な量を超えているかどうかを示します。

** Assignment** の場合は、特定のタスクについてリソースに割り当てられている作業量が、リソースが通常作業可能な量を超えているかどうかを示します。

    <Overallocated>
      BooleanValue
    </Overallocated>

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

**boolean** 型のテキスト値が必要です。

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
<td><p>0</p></td>
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
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

