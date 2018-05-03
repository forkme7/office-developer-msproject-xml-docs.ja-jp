---
title: MicrosoftProjectServerURL 要素
TOCTitle: MicrosoftProjectServerURL 要素
ms:assetid: 7949f2d6-fbfc-49af-ad9a-48265a07fefb
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968553(v=office.12)
ms:contentKeyID: 16740224
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# MicrosoftProjectServerURL 要素

Microsoft Office Project Server の Windows 認証またはフォーム認証を使用するユーザーによってプロジェクトが作成されたかどうかを示します。

    <MicrosoftProjectServerURL>
      BooleanValue
    </MicrosoftProjectServerURL>

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
<td><p>最小 : 0</p>
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

**boolean** 型のテキスト値が必要です。

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
<td><p>False : プロジェクトはフォーム認証ユーザーによって作成されました。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True : プロジェクトは Windows 認証ユーザーによって作成されました。</p></td>
</tr>
</tbody>
</table>


## 備考

Microsoft Office Project Professional に対してのみ適用されます。

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)

