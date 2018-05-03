---
title: Work 要素
TOCTitle: Work 要素
ms:assetid: 84494840-6469-4cbd-ae35-8246d88dfe97
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968571(v=office.12)
ms:contentKeyID: 16741155
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Work 要素

** Task** の場合は、** Work **は割り当てられている全リソースによってタスクで実行されるスケジュールされた作業の総時間数です。

** Resource** の場合は、割り当てられている全タスクでリソースが実行するスケジュールされた作業の総時間数です。

** Assignment** の場合、タスクに対してリソースが実行する計画された作業時間の合計です。

** Baseline** の場合は、ベースラインが保存されたときの、タスク、リソース、または割り当てのスケジュールされた作業時間です。

    <Work>
      DurationValue
    </Work>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a>、<a href="baseline-element.md">Baseline</a></p></td>
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

次の例は、タスク T3 ですべてのリソースに 16 時間の作業時間がスケジュールされていることを示しています。スケジュールされた期間も 16 時間なので、タスクの作業は開始していません。**Work** の値 PT16H0M0S は、16 時間、0 分、0 秒を指定します。PT は Project Time の略で、内部で使用するためのものです。

``` xml
<Task>
   <UID>3</UID>
   <ID>3</ID>
   <Name>T3</Name>
   <Type>1</Type>
   <IsNull>0</IsNull>
   <CreateDate>2007-11-09T15:30:00</CreateDate>
   <WBS>3</WBS>
   <OutlineNumber>3</OutlineNumber>
   <OutlineLevel>1</OutlineLevel>
   <Priority>500</Priority>
   <Start>2007-11-15T08:00:00</Start>
   <Finish>2007-11-16T17:00:00</Finish>
   <Duration>PT16H0M0S</Duration>
   <DurationFormat>53</DurationFormat>
   <Work>PT16H0M0S</Work>
   . . .
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

