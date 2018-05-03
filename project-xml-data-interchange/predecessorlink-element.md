---
title: PredecessorLink 要素
TOCTitle: PredecessorLink 要素
ms:assetid: e372749d-6fbd-47a8-b73b-a037b24fcb05
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968712(v=office.12)
ms:contentKeyID: 16749145
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# PredecessorLink 要素

開始日または終了日に関してタスクが依存する先行タスクを定義します。

    <PredecessorLink>
      ComplexTypeValue
    </PredecessorLink>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
</tr>
</tbody>
</table>


## 子要素


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
<td><p><a href="predecessoruid-element.md">PredecessorUID</a></p></td>
<td><p>オプション</p></td>
<td><p>先行タスクの一意の ID 番号。</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>オプション</p></td>
<td><p>先行タスク リンクの種類 (FF、FS、SF、SS)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="crossproject-element.md">CrossProject</a></p></td>
<td><p>オプション</p></td>
<td><p>先行タスクが別のプロジェクトの一部であるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="crossprojectname-element.md">CrossProjectName</a></p></td>
<td><p>オプション</p></td>
<td><p>外部先行プロジェクト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="linklag-element.md">LinkLag</a></p></td>
<td><p>オプション</p></td>
<td><p>先行タスクからの間隔時間 (単位は 1/10 分)。</p></td>
</tr>
<tr class="even">
<td><p><a href="lagformat-element.md">LagFormat</a></p></td>
<td><p>オプション</p></td>
<td><p><strong>LinkLag</strong> で指定されている間隔の時間形式 (時、日など) を示します。</p></td>
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

