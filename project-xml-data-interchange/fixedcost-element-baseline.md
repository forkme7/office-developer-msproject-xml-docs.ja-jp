---
title: FixedCost 要素 (Baseline)
TOCTitle: FixedCost 要素
ms:assetid: 4b64e229-c147-4b3a-9deb-cae32a27fb11
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968494(v=office.12)
ms:contentKeyID: 16736559
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# FixedCost 要素 (Baseline)

基準計画を保存したときのタスクの固定コストです。

    <FixedCost>
      FloatValue
    </FixedCost>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
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

**float** 型のテキスト値が必要です。

## 備考

固定コストとは、タスクの期間、リソースによって実行される作業の量、および割り当て単位数に関係なく、一定したタスクのコストです。

## 例

次の例では、**FixedCost** 要素を使用して、タスクには固定コストがないことを示します。

``` xml
<Task>
  …
  <FixedCost>0</FixedCost>
  …
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

