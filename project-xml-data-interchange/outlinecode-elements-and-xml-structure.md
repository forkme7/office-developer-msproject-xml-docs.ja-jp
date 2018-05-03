---
title: OutlineCode 要素と XML データ構造
TOCTitle: OutlineCode 要素と XML データ構造
ms:assetid: 9765ae1e-5f80-4932-a576-467833fbc42b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968596(v=office.12)
ms:contentKeyID: 16742757
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# OutlineCode 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **OutlineCodes** 要素の子について説明します。この要素は、プロジェクトを XML 形式で保存するときのアウトライン コード データを表します。

**OutlineCodes** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## OutlineCode 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **OutlineCode** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素に対して有効なテキスト値は、「[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)」に埋め込まれたドキュメント注釈に詳しく記載されています。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

\<[OutlineCodes](outlinecodes-element.md)\>

    \<[OutlineCode](outlinecode-element.md)\>

        \<[Guid](guid-element-multiple-parents.md)\>**string**\</Guid\>

        \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

        \<[FieldName](fieldname-element.md)\>**string**\</FieldName\>

        \<[Alias](alias-element.md)\>**string**\</Alias\>

        \<[PhoneticAlias](phoneticalias-element.md)\>**string**\</PhoneticAlias\>

        \<[Values](values-element.md)\>

            \<[Value](value-element.md)\>

                \<[ValueID](valueid-element.md)\>**integer**\</ValueID\>

                \<[FieldGUID](fieldguid-element.md)\>**string**\</FieldGUID\>

                \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

                \<[ParentValueID](parentvalueid-element.md)\>**integer**\</ParentValueID\>

                \<[Value](value-element.md)\>**string**\</Value\>

                \<[Description](description-element.md)\>**string**\</Description\>

            \</Value\>

        \</Values\>

        \<[Enterprise](enterprise-element.md)\>**boolean**\</Enterprise\>

        \<[EnterpriseOutlineCodeAlias](enterpriseoutlinecodealias-element.md)\>**integer**\</EnterpriseOutlineCodeAlias\>

        \<[ResourceSubstitutionEnabled](resourcesubstitutionenabled-element.md)\>**boolean**\</ResourceSubstitutionEnabled\>

        \<[LeafOnly](leafonly-element.md)\>**boolean**\</LeafOnly\>

        \<[AllLevelsRequired](alllevelsrequired-element.md)\>**boolean**\</AllLevelsRequired\>

        \<[OnlyTableValuesAllowed](onlytablevaluesallowed-element.md)\>**boolean**\</OnlyTableValuesAllowed\>

        \<[Masks](masks-element.md)\>

            \<[Mask](mask-element.md)\>

                \<[Level](level-element.md)\>**integer**\</Level\>

                \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

                \<[Length](length-element.md)\>**integer**\</Length\>

                \<[Separator](separator-element.md)\>**string**\</Separator\>

            \</Mask\>

        \</Masks\>

    \</OutlineCode\>

\</OutlineCodes\>

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)

