---
title: SaveVersion 要素
TOCTitle: SaveVersion 要素
ms:assetid: b6a5948c-cdf5-480d-8b08-d748895809e9
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968654(v=office.12)
ms:contentKeyID: 16745239
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# SaveVersion 要素

XML ファイルを保存した Microsoft Office Project のバージョンです。

    <SaveVersion>
      IntegerValue
    </SaveVersion>

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
<td><p>最小 : 1</p>
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

**integer** 型のテキスト値が必要です。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><ul>
<li><p>値</p></li>
</ul></th>
<th><ul>
<li><p>説明</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><ul>
<li><p>12</p></li>
</ul></td>
<td><ul>
<li><p>Microsoft Office Project 2007</p></li>
</ul></td>
</tr>
</tbody>
</table>


## 備考

**SaveVersion** 要素は Project 2007 で新たに追加されました。Project の将来のリリースで、**SaveVersion** の値が追加される予定です。

## 例

以下の例では、**SaveVersion** 要素を使用して、Project 2007 で XML ファイルが保存されたことを示します。

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
  …
  <SaveVersion>12</SaveVersion>
  …
</Project>
```

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

