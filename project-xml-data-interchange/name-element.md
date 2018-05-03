---
title: Name 要素
TOCTitle: Name 要素
ms:assetid: 99549287-024d-430e-8fde-53c3af351065
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968600(v=office.12)
ms:contentKeyID: 16742910
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Name 要素

プロジェクト、カレンダー、カレンダーの例外、有効稼働日、リソース、またはタスクの名前。

    <Name>
      String(512): for Project, Exception, or WorkWeek; 
        String(255): for Calendar, Resource, or Task
    </Name>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>、<a href="calendar-element.md">Calendar</a>、<a href="exception-element.md">Exception</a>、<a href="workweek-element.md">WorkWeek</a>、<a href="resource-element.md">Resource</a>、<a href="task-element.md">Task</a></p></td>
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

**string** 型のテキスト値が必要です。テキスト値は、**Project**、**Exception**、または **WorkWeek** 要素では 512 文字、その他の要素では 255 文字を超えることはできません。

## 例

次の例では、**Name** 要素を使用して、カレンダーの例外が New Year's Day という名前であることを示しています。

``` xml
<Exception>
  <EnteredByOccurrences>0</EnteredByOccurrences>
  <TimePeriod>
    <FromDate>2007-01-01T00:00:00</FromDate>
    <ToDate>2026-01-01T23:59:00</ToDate>
  </TimePeriod>
  <Occurrences>20</Occurrences>
  <Name>New Year's Day</Name>
  <Type>2</Type>
  <Month>0</Month>
  <MonthDay>1</MonthDay>
  <DayWorking>0</DayWorking>
</Exception>
```

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

