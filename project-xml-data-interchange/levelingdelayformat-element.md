---
title: LevelingDelayFormat 要素
TOCTitle: LevelingDelayFormat 要素
ms:assetid: 2c22da44-4968-417b-887f-a2a1e05bdec9
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968448(v=office.12)
ms:contentKeyID: 16734026
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# LevelingDelayFormat 要素

**LevelingDelayFormat** は、タスクまたは割り当ての ** LevelingDelay ** 期間を表す形式です。

    <LevelingDelayFormat>
      IntegerValue
    </LevelingDelayFormat>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a>、<a href="assignment-element.md">Assignment</a></p></td>
</tr>
</tbody>
</table>


### 要素のプロパティ

**LevelingDelayFormat** 要素は、以下のいずれかの時間単位を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>3</p></td>
<td><p>m (分数)</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>em (経過分数)</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>h (時間数)</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>eh (経過時間数)</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>d (日数)</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>ed (経過日数)</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>w (週数)</p></td>
</tr>
<tr class="even">
<td><p>10</p></td>
<td><p>ew (経過週数)</p></td>
</tr>
<tr class="odd">
<td><p>11</p></td>
<td><p>mo (月数)</p></td>
</tr>
<tr class="even">
<td><p>12</p></td>
<td><p>emo (経過月数)</p></td>
</tr>
<tr class="odd">
<td><p>19</p></td>
<td><p>% (パーセント)</p></td>
</tr>
<tr class="even">
<td><p>20</p></td>
<td><p>e% (経過パーセント)</p></td>
</tr>
<tr class="odd">
<td><p>21</p></td>
<td><p>Null</p></td>
</tr>
<tr class="even">
<td><p>35</p></td>
<td><p>m? (見積もり分数)</p></td>
</tr>
<tr class="odd">
<td><p>36</p></td>
<td><p>em? (見積もり経過分数)</p></td>
</tr>
<tr class="even">
<td><p>37</p></td>
<td><p>h? (見積もり時間数)</p></td>
</tr>
<tr class="odd">
<td><p>38</p></td>
<td><p>eh? (見積もり経過時間)</p></td>
</tr>
<tr class="even">
<td><p>39</p></td>
<td><p>d? (見積もり日数)</p></td>
</tr>
<tr class="odd">
<td><p>40</p></td>
<td><p>ed? (見積もり経過日数)</p></td>
</tr>
<tr class="even">
<td><p>41</p></td>
<td><p>w? (見積もり週数)</p></td>
</tr>
<tr class="odd">
<td><p>42</p></td>
<td><p>ew? (見積もり経過週数)</p></td>
</tr>
<tr class="even">
<td><p>43</p></td>
<td><p>mo? (見積もり月数)</p></td>
</tr>
<tr class="odd">
<td><p>44</p></td>
<td><p>emo? (見積もり経過月数)</p></td>
</tr>
<tr class="even">
<td><p>51</p></td>
<td><p>%? (見積もりパーセント)</p></td>
</tr>
<tr class="odd">
<td><p>52</p></td>
<td><p>e%? (見積もり経過パーセント)</p></td>
</tr>
<tr class="even">
<td><p>53</p></td>
<td><p>Null</p></td>
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

**LevelingDelay** を使用するには ** LevelingDelayFormat ** を指定する必要があります。たとえば、タスクでの平準化による 3 日の延期期間は次のように表します。

``` xml
<Task>
    ...
    <LevelingDelay>3</LevelingDelay>
    <LevelingDelayFormat>7</LevelingDelayFormat>
    ...
</Task>
```

## 参照

#### その他の技術情報

[LevelingDelay 要素](levelingdelay-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

