---
title: UID 要素
TOCTitle: UID 要素
ms:assetid: 90074e2d-5cbf-475c-b456-5649c1b2949b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968590(v=office.12)
ms:contentKeyID: 16742143
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# UID 要素

**UID** 要素は一意識別子です。**UID** は 1 プロジェクト内のいずれかの親要素のデータ レコードを指定します。

    <UID>
      String(16): for Project
      Integer: for all other parent elements
    </UID>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>、<a href="calendar-element.md">Calendar</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a>、<a href="task-element.md">Task</a>、<a href="extendedattribute-element.md">ExtendedAttribute</a>、<a href="timephaseddata-element.md">TimephasedData</a></p></td>
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
<td><p>最小 : 1</p>
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## 備考

**UID** 要素は** Project **要素の場合のみ文字列となります。Microsoft Office Project 2007 では、**Project** 内の **UID** 子要素は非推奨です。

他の親要素の場合、**UID** は整数です。**UID** の値はプロジェクト内でのみ一意であり、複数のプロジェクトにわたって一意なのではありません。

タスクの場合、各 **UID** はプロジェクト内で 1 回だけ使用されます。T3 というタスクを UID = 3、ID = 3 で作成し、そのタスクを削除してから T3 という新しいタスクを ID = 3 で作成した場合、新しいタスクの UID は 4 です。

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)  
[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)

