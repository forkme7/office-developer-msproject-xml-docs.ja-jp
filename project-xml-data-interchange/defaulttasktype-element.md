---
title: DefaultTaskType 要素
TOCTitle: DefaultTaskType 要素
ms:assetid: 9a0cae2a-2c23-4351-b8a9-7b3c22a1f60c
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968603(v=office.12)
ms:contentKeyID: 16742981
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# DefaultTaskType 要素

新しいタスクの既定の種類。

    <DefaultTaskType>
      IntegerValue
    </DefaultTaskType>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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

**integer** 型のテキスト値が必要です。

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
<td><p>単位数固定 (既定)。タスクの作業時間や期間に関係なく、リソース数 (割り当て単位数) が一定になります。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>期間固定。割り当てられたリソースの数 (割り当て単位数) や作業時間に関係なく、タスクの期間が一定になります。</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>作業時間固定。期間やタスクに割り当てられたリソースの数 (割り当て単位数) の変化に関係なく、作業時間が一定になります。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

