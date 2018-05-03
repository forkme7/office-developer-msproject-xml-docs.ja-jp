---
title: AssnOwner 要素
TOCTitle: AssnOwner 要素
ms:assetid: 0c2e69c8-c02a-430d-8470-931b6cb07440
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968408(v=office.12)
ms:contentKeyID: 16731535
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# AssnOwner 要素

割り当て所有者の名前。

    <AssnOwner>
      StringValue
    </AssnOwner>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a>、<a href="resource-element.md">Resource</a></p></td>
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

**string** 型のテキスト値が必要です。

## 例

次の例では、**AssnOwner** 要素と **AssnOwnerGuid** 要素を使用して、割り当て所有者が Ioannis Xylaras であることを指定しています。

``` xml
<Assignment>
  …
  <AssnOwner>Ioannis Xylaras</AssnOwner>
  <AssnOwnerGuid>479C3510-B506-4CE9-BA9A-60C585111E18</AssnOwnerGuid>
  …
</Assignment>
```

## 参照

#### その他の技術情報

[AssnOwnerGuid 要素](assnownerguid-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

