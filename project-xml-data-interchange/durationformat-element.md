---
title: DurationFormat 要素
TOCTitle: DurationFormat 要素
ms:assetid: ac69c48f-4758-4462-a9c3-edf085d52437
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968637(v=office.12)
ms:contentKeyID: 16744421
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# DurationFormat 要素

** Project** の場合、**DurationFormat ** はプロジェクト内のすべての期間の既定の形式です。

**Task** の場合は、タスクの期間を表示するために使用される形式です。

** Baseline** の場合は、タスク基準の期間を表す形式です。

** ExtendedAttribute** の場合は、期間ユーザー設定フィールドなどの拡張属性の期間の形式です。

    <DurationFormat>
      IntegerValue
    </DurationFormat>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>、<a href="task-element.md">Task</a>、<a href="baseline-element.md">Baseline</a>、<a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

**integer** 型のテキスト値が必要です。

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968475.note(ja-jp,office.12).gif" alt="Note" class="note" />メモ :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>経過時間には、プロジェクト カレンダー、リソース カレンダー、またはタスク カレンダーで指定された非稼働時間を含む、すべての時間が含まれます。たとえば、カレンダーで土曜日と日曜日が非稼働日に指定されている場合、期間 7d は、月曜日から金曜日までと、翌週の月曜日および火曜日の、7 日間の稼働日です。期間 7ed は、月曜日から日曜日までの 7 日間の経過日です。</p></td>
</tr>
</tbody>
</table>


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


## 備考

**DurationFormat** は、** Task** だけでなく、** Resource ** または ** Assignment** の ** Baseline ** または ** ExtendedAttribute ** 内に含めることもできます。この要素は、** Project ** 要素の既定の期間形式をオーバーライドするために使用されます。

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

