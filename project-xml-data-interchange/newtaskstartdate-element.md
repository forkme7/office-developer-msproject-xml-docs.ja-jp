---
title: NewTaskStartDate 要素
TOCTitle: NewTaskStartDate 要素
ms:assetid: d621417d-eb69-4fdb-abf7-cebd523eaad0
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968699(v=office.12)
ms:contentKeyID: 16748142
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# NewTaskStartDate 要素

新規タスクの既定の開始日付がプロジェクトの開始日付と現在の日付のどちらであるかを指定します。

    <NewTaskStartDate>
      IntegerValue
    </NewTaskStartDate>

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

必須 **Integer**

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
<td><p>プロジェクトの開始日付</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>現在の日付</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

