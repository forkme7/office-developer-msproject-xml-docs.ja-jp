---
title: CurrencyCode 要素
TOCTitle: CurrencyCode 要素
ms:assetid: 8535d7d5-1414-4222-baaf-f16f8bc8131c
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968575(v=office.12)
ms:contentKeyID: 16741231
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# CurrencyCode 要素

3 文字の通貨文字コード。

    <CurrencyCode>
        StringValue
    </CurrencyCode>

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

**string** 型のテキスト値が必要です。**string** には 4 文字以上は指定できません。

## 備考

通貨の文字コードは、ISO 4217 で定義されています。たとえば、米国のドルは USD、日本の円は JPY、および欧州のユーロは EUR になります。

新しいプロジェクトの既定値は、エンタープライズ グローバル テンプレートによって決まります。エンタープライズ グローバル テンプレート値がない場合、既定値は Project Server を実行する Windows オペレーティング システムから取得されます。

## 例

次の例の **CurrencyCode** 要素は、プロジェクトの通貨が米国ドルであることを示しています。

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
  …
  <CurrencyCode>USD</CurrencyCode>
  …
</Project>
```

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

