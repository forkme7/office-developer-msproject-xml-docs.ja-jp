---
title: HyperlinkAddress 要素
TOCTitle: HyperlinkAddress 要素
ms:assetid: 7fb7cf52-7d90-4ff8-a35b-c02f737eb13a
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968561(v=office.12)
ms:contentKeyID: 16740794
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# HyperlinkAddress 要素

タスク、リソース、または割り当てと関連付けられたハイパーリンクのアドレス。

    <HyperlinkAddress>
      String(512)Value
    </HyperlinkAddress>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="resource-element.md">Resource</a>、<a href="assignment-element.md">Assignment</a></p></td>
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

次の例は、T2 という名前のタスクのハイパーリンクを示しています。この場合、完全な URL は [http://msdn2.microsoft.com/en-us/library/bb456485.aspx\#officepj2007platform\_\_documentation](http://msdn2.microsoft.com/en-us/library/bb456485.aspx) となります。

``` xml
<Task>
    <UID>2</UID>
    <ID>2</ID>
    <Name>T2</Name>
    . . .
    <Hyperlink>Links for Project documentation</Hyperlink>
    <HyperlinkAddress>http://msdn2.microsoft.com/en-us/library/bb456485.aspx</HyperlinkAddress>
    <HyperlinkSubAddress>officepj2007platform__documentation</HyperlinkSubAddress>
. . .
</Task>
```

## 参照

#### その他の技術情報

[Hyperlink 要素](hyperlink-element.md)  
[HyperlinkSubAddress 要素](hyperlinksubaddress-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

