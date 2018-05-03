---
title: RollupType 要素
TOCTitle: RollupType 要素
ms:assetid: 422ed965-01fe-45ec-8b7e-0a606b174c66
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968480(v=office.12)
ms:contentKeyID: 16735835
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# RollupType 要素

ユーザー設定フィールドでサマリー タスクの重ね合わせの値を計算する方法を示します。

    <RollupType>
      IntegerValue
    </RollupType>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

必須 **Integer**

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
<td><p>最大 (フラグ フィールドでは OR)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>最小 (フラグ フィールドでは AND)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>すべて計算</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>合計</p></td>
</tr>
<tr class="odd">
<td><p>4</p></td>
<td><p>平均</p></td>
</tr>
<tr class="even">
<td><p>5</p></td>
<td><p>平均 (最初のサブレベル)</p></td>
</tr>
<tr class="odd">
<td><p>6</p></td>
<td><p>計算 (最初のサブレベル)</p></td>
</tr>
<tr class="even">
<td><p>7</p></td>
<td><p>計算 (非サマリー)</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)

