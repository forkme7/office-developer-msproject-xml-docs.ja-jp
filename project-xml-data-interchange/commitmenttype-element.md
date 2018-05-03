---
title: CommitmentType 要素
TOCTitle: CommitmentType 要素
ms:assetid: e00871cd-1614-4fa8-83b2-66f2d1130428
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968709(v=office.12)
ms:contentKeyID: 16748881
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# CommitmentType 要素

タスクに、関連付けられた成果物または関連付けられた成果物に対する依存関係があるかどうかを示します。

    <CommitmentType>
      IntegerValue
    </CommitmentType>

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
<td><p>タスクには、成果物または成果物に対する依存関係はありません。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>タスクには関連付けられた成果物があります。</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>タスクには関連付けられた成果物に対する依存関係があります。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

