---
title: FreeSlack 要素
TOCTitle: FreeSlack 要素
ms:assetid: a26cf9d8-e0e9-4c34-a476-24ea8dee4b38
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968623(v=office.12)
ms:contentKeyID: 16743647
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# FreeSlack 要素

後続のタスクを遅延させることなくタスクを遅延させることができる実際の期間です。後続タスクが存在しない場合、余裕期間は、プロジェクト全体を遅延させることなくタスクを遅延させることができる期間です。

    <FreeSlack>
      IntegerValue
    </FreeSlack>

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


## 例

次の例は、1 日の作業時間が 8 時間の場合に、タスクを 2 日間遅延させることができることを示しています (2 日間 x 8 時間/日 x 60 分/時 x 10 x 1/10 分 = 9600 x 1/10 分)。この場合に使用可能な実際の余裕期間 (**FreeSlack**) は、総余裕期間と同じです。

``` xml
<Task>
   . . .
   <FreeSlack>9600</FreeSlack>
   <TotalSlack>9600</TotalSlack>
   . . .
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

