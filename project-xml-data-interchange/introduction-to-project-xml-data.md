---
title: Project XML データの概要
TOCTitle: Project XML データの概要
ms:assetid: b4d72252-5b88-4244-b350-8f026c3e60cf
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968652(v=office.12)
ms:contentKeyID: 16745088
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Project XML データの概要

Microsoft Office Project 2007 では、プロジェクト データを XML ファイル形式で保存およびインポートすることによって、他のアプリケーションとデータを交換できます。Project 2007 データを XML 形式で表すために使用される XML 要素は、Project 2007 の XML データ交換スキーマ (mspdi\_pj12.xsd) によって定義されています。

## このセクションの内容

  - 「[Project 2007 XML データ交換スキーマの変更点](changes-in-the-project-2007-xml-data-interchange-schema.md)」では、Project 2007 で新しく追加された XML 要素を示し、ユーザー設定フィールド用の XML データの変更点を説明します。

  - 「[Project XML データ交換ファイルを操作する](working-with-project-xml-data-interchange-files.md)」では、XML 形式のプロジェクトを保存する方法と開く方法について説明し、XSLT 変換を使用して Project XML データでレポートを作成する方法を示します。

  - 「[Project データ交換の要素](project-data-interchange-elements.md)」では、要素と型のアルファベット順の一覧と、Project 2007 XML データ交換スキーマの主なセクションごとのリファレンスを示します。

## Project データ交換スキーマ リファレンスの構造

Project XML データ交換スキーマ リファレンスは、次の主なセクションで構成されます。

  - [Project 要素と XML データ構造](project-elements-and-xml-structure.md)

  - [OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)

  - [WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)

  - [ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)

  - [Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)

  - [Task 要素と XML データ構造](task-elements-and-xml-structure.md)

  - [Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)

  - [Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)

  - [TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)

## データ型

Project データ交換スキーマで定義された XML 要素のテキスト値には、次のデータ型が使用されます。

**表 1. テキスト値のデータ型**

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>データ型</th>
<th>データ形式</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>boolean</strong></p></td>
<td><p>ブール値。有効な値は <strong>true</strong> (1) および <strong>false</strong> (0) です。</p></td>
</tr>
<tr class="even">
<td><p><strong>dateTime</strong></p></td>
<td><p>日付と時刻のデータ。YYYY-MM-DDTHH:MM:SS という形式です。</p></td>
</tr>
<tr class="odd">
<td><p><strong>decimal</strong></p></td>
<td><p>任意の精度の数値。</p></td>
</tr>
<tr class="even">
<td><p><strong>duration</strong></p></td>
<td><p>期間。PnYnMnDTnHnMnS という形式で示されます (<em>n</em>Y は年数、<em>n</em>M は月数、<em>n</em>D は日数、T は日と時刻の区切り文字、<em>n</em>H は時間数、<em>n</em>M は分数、および <em>n</em>S は秒数)。</p>
<p>たとえば、1 年 2 か月 3 日 10 時間 30 分という期間を表すには、P1Y2M3DT10H30M と記述します。また、マイナス 120 日間は -P120D で表すことができます。</p></td>
</tr>
<tr class="odd">
<td><p><strong>float</strong></p></td>
<td><p>単精度、32 ビット浮動小数点数。</p></td>
</tr>
<tr class="even">
<td><p><strong>integer</strong></p></td>
<td><p>10 進数。オプションで先頭に記号 (+ または -) を付けることができます。このデータ型は decimal から派生しています。</p></td>
</tr>
<tr class="odd">
<td><p><strong>string</strong></p></td>
<td><p>文字列。</p></td>
</tr>
<tr class="even">
<td><p><strong>time</strong></p></td>
<td><p>時刻データ。HH:MM:SS という形式です。</p></td>
</tr>
<tr class="odd">
<td><p><strong>TimephasedDataType</strong></p></td>
<td><p>ある期間にわたって分散しているタスク、リソース、または割り当てに関する情報を含む複合データ型。<strong>TimephasedData</strong> 要素はこの型です。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project データ交換の要素](project-data-interchange-elements.md)

