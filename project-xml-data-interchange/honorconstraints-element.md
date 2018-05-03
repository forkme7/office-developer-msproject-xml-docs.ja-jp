---
title: HonorConstraints 要素
TOCTitle: HonorConstraints 要素
ms:assetid: 9f270de3-5c09-4e66-ba58-ff358fcd66af
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968614(v=office.12)
ms:contentKeyID: 16743398
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# HonorConstraints 要素

Microsoft Office Project が、タスクの依存関係ではなく制約の指定日に従って、タスクをスケジュールするかどうかを示します。

    <HonorConstraints>
      BooleanValue
    </HonorConstraints>

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


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

