---
title: IsCostResource 要素
TOCTitle: IsCostResource 要素
ms:assetid: 74fc88e2-ebe0-45e9-8092-b3cfb7bc6e59
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968549(v=office.12)
ms:contentKeyID: 16739911
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# IsCostResource 要素

リソースがコスト リソースであるかどうかを示します。

    <IsCostResource>
      BooleanValue
    </IsCostResource>

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

**boolean** 型のテキスト値が必要です。

有効な値を表 1 に示します。

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


## 例

次の例では、**IsCostResource** 要素を使用して、リソースがコスト リソースであることを示しています。

``` xml
<Resource>
  …
  <IsCostResource>1</IsCostResource>
  …
</Resource>
```

## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

