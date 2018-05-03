---
title: WorkVariance 要素
TOCTitle: WorkVariance 要素
ms:assetid: cd8c71ed-bf3a-4013-8e17-dd970785e79b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968689(v=office.12)
ms:contentKeyID: 16747473
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# WorkVariance 要素

** Task** の場合、** WorkVariance ** はタスクの基準作業時間と現在スケジュールされている作業時間の差です。

** Resource** の場合、リソースの基準作業時間の合計と現在スケジュールされている作業時間の差です。

** Assignment** の場合、基準作業時間と割り当て作業時間の差を 1000 分単位で表します。

    <WorkVariance>
      FloatValue
    </WorkVariance>

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


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

