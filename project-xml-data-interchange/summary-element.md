---
title: Summary 要素
TOCTitle: Summary 要素
ms:assetid: 3a98d88c-72ab-48dd-a0a7-97928fbea13e
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968468(v=office.12)
ms:contentKeyID: 16735224
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Summary 要素

タスクがサマリー タスクであるかどうか、またはリソースがサマリー タスクに割り当てられているかどうかを示します。

    <Summary>
      BooleanValue
    </Summary>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a>、<a href="task-element.md">Task</a></p></td>
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


## 備考

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
<td><p>通常、リソースはサマリー タスクではなく、個々のサブタスクに割り当てる必要があります。詳細については、Project 2007 Help and How-to ガイドの「<a href="http://office.microsoft.com/ja-jp/project/ha101935931041.aspx">タスクにリソースを割り当てる</a>」を参照してください。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

