---
title: OutlineNumber 要素
TOCTitle: OutlineNumber 要素
ms:assetid: b3a0a187-116d-4dec-898e-2cc3381525a5
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968651(v=office.12)
ms:contentKeyID: 16744987
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# OutlineNumber 要素

アウトライン内のタスクの正確な位置を示します。たとえば、"7.2" は、このタスクが 7 番目の最上位サマリー タスクの 2 番目のサブタスクであることを示します。

    <OutlineNumber>
      String(512)Value
    </OutlineNumber>

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

**OutlineNumber** は、アウトライン階層におけるタスクの位置を示す文字列であり、"5.2.6" などになります。** OutlineLevel ** は 2 などのシンプルな番号です。

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

