---
title: ExternalTask 要素
TOCTitle: ExternalTask 要素
ms:assetid: 96f30b4f-3b97-45d0-964a-eb28a4042af1
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968595(v=office.12)
ms:contentKeyID: 16742715
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ExternalTask 要素

タスクに外部プロジェクトのタスクがリンクしているかどうかを示します。

    <ExternalTask>
      BooleanValue
    </ExternalTask>

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
<td><p>偽。現在のプロジェクトに由来するタスクであり、外部リンクはありません。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>真。タスクは外部プロジェクトのタスクにリンクしています。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

