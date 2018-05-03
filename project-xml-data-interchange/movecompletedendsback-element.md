---
title: MoveCompletedEndsBack 要素
TOCTitle: MoveCompletedEndsBack 要素
ms:assetid: 31ad7845-ee66-48b4-8079-d36065d708d1
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968457(v=office.12)
ms:contentKeyID: 16734499
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# MoveCompletedEndsBack 要素

状況報告日の後に始まるようにスケジュールされているが、早く始まったタスクの完了部分の終わりを状況報告日に戻す必要があるかどうかを示します。

    <MoveCompletedEndsBack>
      BooleanValue
    </MoveCompletedEndsBack>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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


## 備考

**MoveCompletedEndsBack** 要素では、丸めエラーが発生します。内部的な作業時間の値は 8 桁であり、1 分ごとに 0.001 秒が失われ、その結果として丸めエラーが発生します。

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

