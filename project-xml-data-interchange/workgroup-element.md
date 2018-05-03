---
title: WorkGroup 要素
TOCTitle: WorkGroup 要素
ms:assetid: ed14d8e2-f8d6-4565-92db-6b1a7c91558d
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968721(v=office.12)
ms:contentKeyID: 16749928
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# WorkGroup 要素

リソースが属するワークグループの種類。**WorkGroup** は、プロジェクト チームとのコミュニケーションに使用されるメッセージ方式の種類も指定します。

    <WorkGroup>
      IntegerValue
    </WorkGroup>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="resource-element.md">Resource</a></p></td>
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

必須の **Integer** 値。

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
<td><p>既定値</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>なし。このプロジェクトではワークグループのメッセージが使用されていません。</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>電子メールのみ</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Web (Project Web Access)</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

