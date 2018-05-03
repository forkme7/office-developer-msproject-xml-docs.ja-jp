---
title: TimephasedDataType 要素と XML データ構造
TOCTitle: TimephasedDataType 要素と XML データ構造
ms:assetid: ed317823-7111-4dfd-ae38-50a06c6cb70f
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968722(v=office.12)
ms:contentKeyID: 16749939
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# TimephasedDataType 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **TimephasedDataType** 複合型の要素を説明します。**TimephasedData** 要素は、ある日数の期間での 1 日あたりの作業時間数など、タイムスケール データを表現する **TimephasedDataType** 型です。**Task**、**Resource**、**Assignment**、および **Baseline** 要素には **TimephasedData** を格納できます。

## TimephasedData 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **TimephasedDataType** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。「[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)」にあるドキュメント注釈には、各要素の有効なテキスト値に関する詳細情報があります。

\<[TimephasedData](timephaseddata-element.md)\>

    \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

    \<[UID](uid-element.md)\>**integer**\</UID\>

    \<[Start](start-element.md) \>**dateTime**\</Start\>

    \<[Finish](finish-element.md)\>**dateTime**\</Finish\>

    \<[Unit](unit-element.md)\>**integer**\</Unit\>

    \<[Value](value-element.md)\>**string**\</Value\>

\</TimephasedData\>

Project 2007 XML データ交換スキーマで使用されているデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

## 参照

#### その他の技術情報

[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Baseline 要素](baseline-element.md)

