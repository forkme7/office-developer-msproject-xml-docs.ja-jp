---
title: StatusManager 要素
TOCTitle: StatusManager 要素
ms:assetid: a87e6390-ab36-4041-baa1-939bc6b448f7
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968633(v=office.12)
ms:contentKeyID: 16744107
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# StatusManager 要素

タスク進捗管理者の名前です。

    <StatusManager>
      StringValue
    </StatusManager>

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

**string** 型のテキスト値が必要です。

## 備考

タスクの進捗管理者は、プロジェクト マネージャと異なる人物にすることができます。進捗管理者は、タスク割り当ての所有者となり、それらの割り当てに対する進捗の更新をすべて受け取ります。

## 例

以下の例では、**StatusManager** 要素を使用して、Ioannis Xylaras がタスクの進捗管理者であることを示しています。

``` xml
<Task>
  . . .
  <StatusManager>Ioannis Xylaras</StatusManager>
  . . .
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

