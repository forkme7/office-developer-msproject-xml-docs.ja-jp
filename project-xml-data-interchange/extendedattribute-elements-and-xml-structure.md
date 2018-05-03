---
title: ExtendedAttribute 要素と XML データ構造
TOCTitle: ExtendedAttribute 要素と XML データ構造
ms:assetid: 88acf5ad-cdb2-4fda-b178-ad43dc572684
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968579(v=office.12)
ms:contentKeyID: 16741519
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# ExtendedAttribute 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **ExtendedAttributes** 要素の子について説明します。**ExtendedAttribute** 内の XML 要素は、ユーザー設定フィールドのデータを表します。

**ExtendedAttributes** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。**Task**、**Resource**、または **Assignment** 要素に、個々の **ExtendedAttribute** 要素を格納することもできます。詳細については、「[Task 要素と XML データ構造](task-elements-and-xml-structure.md)」、「[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)」、および「[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)」を参照してください。

## ExtendedAttributes の XML データ構造

以下に、mspdi\_pj12.xsd の **ExtendedAttribute** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素に対して有効なテキスト値は、「[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)」に埋め込まれたドキュメント注釈に詳しく記載されています。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

\<[ExtendedAttributes](extendedattributes-element.md)\>

    \<[ExtendedAttribute](extendedattribute-element.md)\>

        \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

        \<[FieldName](fieldname-element.md)\>**string**\</FieldName\>

        \<[CFType](cftype-element.md)\>**integer**\</CFType\>

        \<[Guid](guid-element-multiple-parents.md)\>**string**\</Guid\>

        \<[ElemType](elemtype-element.md)\>**integer**\</ElemType\>

        \<[MaxMultiValues](maxmultivalues-element.md)\>**integer**\</MaxMultiValues\>

        \<[UserDef](userdef-element.md)\>**boolean**\</UserDef\>

        \<[Alias](alias-element.md)\>**string**\</Alias\>

        \<[SecondaryPID](secondarypid-element.md)\>**string**\</SecondaryPID\>

        \<[AutoRollDown](autorolldown-element.md)\>**boolean**\</AutoRollDown\>

        \<[DefaultGuid](defaultguid-element.md)\>**string**\</DefaultGuid\>

        \<[Ltuid](ltuid-element.md)\>**string**\</Ltuid\>

        \<[PhoneticAlias](phoneticalias-element.md)\>**string**\</PhoneticAlias\>

        \<[RollupType](rolluptype-element.md)\>**integer**\</RollupType\>

        \<[CalculationType](calculationtype-element.md)\>**integer**\</CalculationType\>

        \<[Formula](formula-element.md)\>**string**\</Formula\>

        \<[RestrictValues](restrictvalues-element.md)\>**boolean**\</RestrictValues\>

        \<[ValuelistSortOrder](valuelistsortorder-element.md)\>**integer**\</ValuelistSortOrder\>

        \<[AppendNewValues](appendnewvalues-element.md)\>**boolean**\</AppendNewValues\>

        \<[Default](default-element-extendedattribute.md)\>**string**\</Default\>

        \<[ValueList](valuelist-element.md)\>

            \<[Value](value-element.md)\>

                \<[ID](id-element.md)\>**integer**\</ID\>

                \<[Value](value-element.md)\>**string**\</Value\>

                \<[Description](description-element.md)\>**string**\</Description\>

                \<[Phonetic](phonetic-element.md)\>**string**\</Phonetic\>

            \</Value\>

        \</ValueList\>

    \</ExtendedAttribute\>

\</ExtendedAttributes\>

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)

