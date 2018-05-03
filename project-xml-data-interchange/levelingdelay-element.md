---
title: LevelingDelay 要素
TOCTitle: LevelingDelay 要素
ms:assetid: 02a5a3be-5569-4f08-97b0-c23dceb35861
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968397(v=office.12)
ms:contentKeyID: 16730780
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# LevelingDelay 要素

** Task** の場合、** LevelingDelay **は、リソースの平準化の結果としてタスクを最早開始日から延期する時間の量です。

** Assignment** の場合、タスクに対してリソースが実行する計画された作業時間の合計です。

    <LevelingDelay>
      IntegerValue
    </LevelingDelay>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="assignment-element.md">Assignment</a></p></td>
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


## 備考

**LevelingDelay** を使用するには ** LevelingDelayFormat ** を指定する必要があります。たとえば、タスクでの平準化による 3 日の延期期間は次のように表します。

``` xml
<Task>
    ...
    <LevelingDelay>3</LevelingDelay>
    <LevelingDelayFormat>7</LevelingDelayFormat>
    ...
</Task>
```

## 参照

#### その他の技術情報

[LevelingDelayFormat 要素](levelingdelayformat-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

