---
title: MoveRemainingStartsBack 要素
TOCTitle: MoveRemainingStartsBack 要素
ms:assetid: b2fa4c92-1740-4532-bd40-03e32ed8a8c3
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968650(v=office.12)
ms:contentKeyID: 16744920
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# MoveRemainingStartsBack 要素

状況報告日以後に開始が予定されていたにもかかわらず早く開始されたタスクの、残りの部分の開始日を状況報告日まで前倒しするかどうかを示します。

    <MoveRemainingStartsBack>
      BooleanValue
    </MoveRemainingStartsBack>

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

**MoveRemainingStartsBack** 要素では、丸めエラーが発生します。内部的な作業時間の値は 8 桁であり、1 分ごとに 0.001 秒が失われ、その結果として丸めエラーが発生します。

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

