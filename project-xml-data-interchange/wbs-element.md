---
title: WBS 要素
TOCTitle: WBS 要素
ms:assetid: 82e4cde0-01e5-4a2a-93e1-aa5de8c701cb
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968566(v=office.12)
ms:contentKeyID: 16741042
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# WBS 要素

プロジェクトの階層構造内でのタスクの位置を表す一意のコード (Work Breakdown Structure)。

    <WBS>
       StringValue
    </WBS>

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


## 備考

既定では、WBS コードはタスクのアウトライン番号です (最上位タスクの場合は 1、2、…、n、タスク 1 の下のサブタスクの場合は 1.1、1.2、…、1.n、以下同様)。WBS コードを定義するには、Microsoft Office Project で \[プロジェクト\] メニューの \[WBS\] をクリックします。詳細については、「[\[WBS 番号\] フィールド](http://office.microsoft.com/ja-jp/project/hp010259301041.aspx)」を参照してください。

## 参照

#### その他の技術情報

[WBSLevel 要素](wbslevel-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

