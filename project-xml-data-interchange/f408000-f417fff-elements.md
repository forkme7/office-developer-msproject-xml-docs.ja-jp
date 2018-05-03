---
title: f408000 ～ f417fff 要素
TOCTitle: f408000 ～ f417fff 要素
ms:assetid: cc4a5f30-5707-4861-8243-18bd138dcc95
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968688(v=office.12)
ms:contentKeyID: 16747364
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# f408000 ～ f417fff 要素

割り当てレベルのエンタープライズ ユーザー設定フィールドの値です。

    <f408000>
        CustomFieldValue
    </f408000>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignment-element.md">Assignment</a></p></td>
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
<p>最大 : 一意な要素名ごとに 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

テキスト値は必須です。割り当て用のエンタープライズ ユーザー設定フィールド値を指定します。

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
<td><p>テキスト値は、ユーザー設定フィールドの定義で必要なデータ型と一致する必要があります。</p></td>
</tr>
</tbody>
</table>


## 備考

エンタープライズ ユーザー設定フィールドの値を格納する XML 要素の名前は、ユーザー設定フィールド ID の 16 進表現に対応します。

表 1 に、割り当てレベルのエンタープライズ ユーザー設定フィールドのユーザー設定フィールド ID として有効な範囲を 10 進数と 16 進数で示します。

**表 1. 割り当てレベルのエンタープライズ ユーザー設定フィールド ID**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>ユーザー設定フィールド ID の範囲 (10 進)</th>
<th>ユーザー設定フィールド ID の範囲 (16 進)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>255885312-255950847</p></td>
<td><p>f408000 ～ f417fff</p></td>
</tr>
</tbody>
</table>


詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。

## 参照

#### その他の技術情報

[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)

