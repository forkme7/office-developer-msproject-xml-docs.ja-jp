---
title: IsPublished 要素
TOCTitle: IsPublished 要素
ms:assetid: 54c16411-8ce2-4eda-aa3c-7558a525f690
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968507(v=office.12)
ms:contentKeyID: 16737313
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# IsPublished 要素

タスクが発行されたかどうかを示します。

    <IsPublished>
      BooleanValue
    </IsPublished>

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
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>


## 例

以下の例では、**IsPublished** 要素を使用して、タスクが発行済みであることを示しています。

``` xml
<Task>
  …
  <IsPublished>1</IsPublished>
  …
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

