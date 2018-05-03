---
title: ConstraintType 要素
TOCTitle: ConstraintType 要素
ms:assetid: d8ade667-0c92-4c1e-b0d8-76f8d2411330
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968703(v=office.12)
ms:contentKeyID: 16748360
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ConstraintType 要素

タスクの開始または終了日付に対する制約。

    <ConstraintType>
      IntegerValue
    </ConstraintType>

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
<td><p>できるだけ早く</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>できるだけ遅く</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>次の時点で開始が必要</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>次の時点で終了が必要</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>次の時点よりも遅く開始</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>次の時点よりも早く開始</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>次の時点よりも遅く終了</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>次の時点よりも早く終了</p></td>
</tr>
</tbody>
</table>


## 備考

**ConstraintType** が 0 または 1 に設定されている場合を除き、** ConstraintDate ** は同じタスクで設定されていることが必要。

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

