---
title: WBSMask 要素と XML データ構造
TOCTitle: WBSMask 要素と XML データ構造
ms:assetid: 101c3fa6-ccbf-4b34-ac5a-584c12fabbbd
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968416(v=office.12)
ms:contentKeyID: 16731855
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# WBSMask 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **WBSMasks** 要素の子について説明します。この XML 要素は、プロジェクトを XML 形式で保存するときの作業分割構造 (WBS) コード マスク データを表します。

**WBSMasks** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## WBSMasks 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **WBSMask** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素の有効なテキスト値の詳細については、[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)に埋め込まれているドキュメント注釈を参照してください。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

\<[WBSMasks](wbsmasks-element.md)\>

    \<[VerifyUniqueCodes](verifyuniquecodes-element.md)\>**boolean**\</VerifyUniqueCodes\>

    \<[GenerateCodes](generatecodes-element.md)\>**boolean**\</GenerateCodes\>

    \<[Prefix](prefix-element.md)\>**string**\<Prefix\>

    \<[WBSMask](wbsmask-element.md)\>

        \<[Level](level-element.md)\>**integer**\</Level\>

        \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

        \<[Length](length-element.md)\>**string**\</Length\>

        \<[Separator](separator-element.md)\>**string**\</Separator\>

    \</WBSMask\>

\</WBSMasks\>

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[WBSMasks 要素の XML スキーマ](xml-schema-for-the-wbsmasks-element.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)

