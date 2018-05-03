---
title: Project データ交換の要素
TOCTitle: Project データ交換の要素
ms:assetid: c0382453-e552-402c-be05-fa50af11e71d
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968664(v=office.12)
ms:contentKeyID: 16746007
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Project データ交換の要素

このセクションでは、Project XML データ交換スキーマによって定義される要素と、ユーザー設定フィールド値を表すために Microsoft Office Project 2007 で使用されるその他の XML 要素について説明します。

このトピックには、以下のセクションが含まれます。

  - Project データ交換 XML 要素の構造
    
      - 一般的な要素の構造
    
      - 詳細な要素の構造

## Project データ交換 XML 要素の構造

Project データ交換スキーマは、Project 2007 SDK ダウンロードに含まれています。Project 2007 SDK ダウンロードへのリンクについては、「[Microsoft Office Project 2007 SDK へようこそ](https://msdn.microsoft.com/ja-jp/library/ms512767\(v=office.12\))」を参照してください。

スキーマに含まれるすべての要素の一覧については、「[要素と型のアルファベット順の一覧](alphabetical-list-of-elements-and-types.md)」を参照してください。

Project データ交換スキーマ内の多くの要素は、Microsoft Office Project Professional 2007 のデータ フィールドを表しています。Project Professional 2007 と Project Standard 2007 のフィールドの詳細については、「[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)」を参照してください。

### 一般的な要素の構造

次のアウトラインは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) の高レベル XML 要素の構造を示しています。アウトライン内のリンクをクリックすると、各要素の説明ページにジャンプします。次の各要素の XML データ構造については、「詳細な要素の構造」を参照してください。

\<[Project](project-element.md)\>

    \<\!-- … Project の子要素 --\>

    \<[OutlineCodes](outlinecodes-element.md)\> … \</OutlineCodes\>

    \<[WBSMasks](wbsmasks-element.md)\> … \</WBSMasks\>

    \<[ExtendedAttributes](extendedattributes-element.md)\> … \</ExtendedAttributes\>

    \<[Calendars](calendars-element.md)\> … \</Calendars\>

    \<[Tasks](tasks-element.md)\> … \</Tasks\>

    \<[Resources](resources-element.md)\> … \</Resources\>

    \<[Assignments](assignments-element.md)\> … \</Assignments\>

\</Project\>

### 詳細な要素の構造

それぞれの主要要素の XML データ構造の詳細については、以下のトピックを参照してください。

  - [Project 要素と XML データ構造](project-elements-and-xml-structure.md)

  - [OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)

  - [WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)

  - [ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)

  - [Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)

  - [Task 要素と XML データ構造](task-elements-and-xml-structure.md)

  - [Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)

  - [Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)

  - [TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Project 2007 XML データ交換スキーマの変更点](changes-in-the-project-2007-xml-data-interchange-schema.md)  
[Project XML データ交換ファイルを操作する](working-with-project-xml-data-interchange-files.md)  
[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)

