---
title: EarnedValueMethod 要素
TOCTitle: EarnedValueMethod 要素
ms:assetid: a151ec3f-e5f5-4141-aeaa-c595d57702e8
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968620(v=office.12)
ms:contentKeyID: 16743565
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# EarnedValueMethod 要素

** Project** の場合、** EarnedValueMethod ** は達成額を計算するための既定の方法です。

** Task** の場合は、タスクで使用する達成額の計算方法の種類を示します。

    <EarnedValueMethod>
      IntegerValue
    </EarnedValueMethod>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>、<a href="task-element.md">Task</a></p></td>
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

**Integer** 型のテキスト値が必要です。

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
<td><p>達成率を使用します</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>実際の達成率を使用します</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

