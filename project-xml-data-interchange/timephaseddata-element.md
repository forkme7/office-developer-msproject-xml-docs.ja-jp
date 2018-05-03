---
title: TimephasedData 要素
TOCTitle: TimephasedData 要素
ms:assetid: 41c66612-a3af-499c-b9ba-c552216d5820
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968479(v=office.12)
ms:contentKeyID: 16735794
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# TimephasedData 要素

**TimephasedData** は、時間経過に沿ったタスク、リソース、割り当てに関する情報です。タイムスケール領域にあるデータは、タスクまたは割り当ての基準計画に関連している場合もあります。

    <TimephasedData>
        <UID>IntegerValue</UID>
      . . .
    </TimephasedData>

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


## 子要素


<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域にある 76 種類のデータの 1 つ</p></td>
</tr>
<tr class="even">
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>必須</p></td>
<td><p>タイムスケール領域にあるデータレコードの一意の ID</p></td>
</tr>
<tr class="odd">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域にあるデータのレコードの開始日</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域にあるデータのレコードの終了日</p></td>
</tr>
<tr class="odd">
<td><p><a href="unit-element.md">Unit</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域にあるデータのレコードの時間単位</p></td>
</tr>
<tr class="even">
<td><p><a href="value-element.md">Value</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域にあるデータのレコードの各単位の値</p></td>
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
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 例

次の例は、タスクのタイムスケール領域にあるデータの種類が達成率 (%) (**Type** = 11) で、時間単位が日 (**Unit** = 2) であり、このタスクが 50% 達成していることを示しています。タスクの作業時間は、開始が 2007 年 11 月 9 日の午前 8 時で、終了が同じ日の午後 5 時です。

``` xml
<Task>
   . . .
   <TimephasedData>
      <Type>11</Type>
      <UID>2</UID>
      <Start>2007-11-09T08:00:00</Start>
      <Finish>2007-11-09T17:00:00</Finish>
      <Unit>2</Unit>
      <Value>50</Value>
   </TimephasedData>
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
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)  
[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)

