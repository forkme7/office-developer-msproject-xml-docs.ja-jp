---
title: " Project XML データ交換ファイルで XSLT 変換を使用する"
TOCTitle: " Project XML データ交換ファイルで XSLT 変換を使用する"
ms:assetid: 66d1ac85-7ec8-44b8-a73f-3e4d6b148219
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968529(v=office.12)
ms:contentKeyID: 16738748
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Project XML データ交換ファイルで XSLT 変換を使用する

Extensible Stylesheet Language Transformation (XSLT) 標準では、XML データ変換のための言語定義が指定されています。XSLT は、XML ドキュメントを XHTML ドキュメントまたは他の XML ドキュメントに変換するために使用します。この記事では、Microsoft Office Project 2007 XML データ交換ファイルで XSLT を使用して、プロジェクトの情報をフィルタ処理および表示する方法について説明します (この記事の内容については、Microsoft Corporation の Jessica Britton の協力を得ました)。

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
<td><p>プロジェクトを Project XML データ交換ファイルとして保存する方法の詳細については、「<a href="saving-and-opening-projects-in-xml-format.md">XML 形式でプロジェクトを保存および開く</a>」を参照してください。</p></td>
</tr>
</tbody>
</table>


XSLT スタイルシートは、連携して機能する XHTML マークアップ、XSLT テンプレート ルール、および XPath ステートメントの組み合わせで構成される XML ドキュメントです。

  - XHTML マークアップは、XML データが表示される環境を定義します。

  - XSLT テンプレート ルールは、ソース XML 要素を変換する特定の方法を指定します。

  - XPath ステートメントは、XML ドキュメント内の特定の要素を示します。

XML 要素が XPath のパターンと一致すると、関連付けられている XSLT テンプレート ルールが呼び出されます。その後、変換されたデータが、XHTML マークアップで指定されている表示フレームワークに表示されます。

XSLT テンプレート ルールおよび XPath ステートメントの詳細については、この記事の最後にあるリンクを参照してください。

## XSLT 変換を使用してプロジェクトの情報を表示する

### 手順 1. XSLT スタイルシートを作成するには

1.  スタイルシート用の XSLT ファイルを作成します。Microsoft Visual Studio 2005 で作業している場合は、XSLT File テンプレートを使用できます (Visual Studio で、\[ファイル\] をクリックし、\[新規作成\] をポイントして、\[ファイル\] をクリックします)。このテンプレートには、次の例で示すような XML コードがあらかじめ記述されています。別のテキスト エディタまたは XML エディタを使用している場合は、このテンプレート XML をコピーし、XSLT ファイルに貼り付けてください。
    
    ``` xml
    <?xml version="1.0" encoding="utf-8"?>
    
    <xsl:stylesheet version="1.0"
        xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
    
    <xsl:template match="/">
        <html>
        <body>
        <!--
            This is an XSLT template file. Fill in this area with the
            XSL elements which will transform your XML to XHTML.
        -->
        </body>
        </html>
    </xsl:template>
    
    </xsl:stylesheet>
    ```

2.  次の XML コード コメントを削除します。ここに、実際の XSLT コードを記述します。
    
    ``` xml
        <!--
            This is an XSLT template file. Fill in this area with the
            XSL elements that will transform your XML to XHTML.
        -->
    ```

3.  XSLT コードを作成します。この例で示す XSLT コードは、次のことを行います。
    
      - ヘッダーの **Project** 要素の子 **Name** のテキスト値を表示します。
    
      - 各 **Task** 要素の子 **Summary** をテストして、値が 0 (false) かどうかを確認します。
    
      - 各 **Task** 要素の子 **Critical** をテストして、値が 1 (true) かどうかを確認します。
    
      - サマリー タスクではない重要なタスクのデータを太字で表示します。
    
      - サマリー タスクではなく重要ではないタスクのデータを表示します。
    
      - 各 **Resource** 要素の子 **Name** のテキスト値で、リソース情報をアルファベット順に並べ替えます。
    
      - 各 **Resource** 要素の子 **Overallocated** をテストして、値が 1 (true) かどうかを確認します。
    
      - 割り当て超過のリソースについてのみ、並べ替えたリソース データを表示します。
    
    <!-- end list -->
    
    ``` xml
    <!-- Define a table to display data in. -->
          <table border="1" cellpadding="3">
            <tr>
              <td colspan="5" align="center">
                <!-- Filter for the project name and display it in a header.  -->
                <h2>
                  <font face="tahoma" size="5">
                    Status for: <xsl:value-of select="Project/Name" />
                  </font>
                </h2>
              </td>
            </tr>
            <!-- Define headers for task information. -->
            <tr>
              <td colspan="5" align="center">
                Tasks:
              </td>
            </tr>
            <tr>
              <th>
                <font color="black">ID</font>
              </th>
              <th>
                <font color="black">Name</font>
              </th>
              <th>
                <font color="black">Priority</font>
              </th>
              <th>
                <font color="black">Start</font>
              </th>
              <th>
                <font color="black">Finish</font>
              </th>
            </tr>
            <!-- Filter for tasks -->
            <xsl:for-each select="Project/Tasks/Task">
              <!-- Exclude summary tasks -->
              <xsl:if test="Summary[.=0]">
                <xsl:choose>
                  <!-- Display information for critical tasks with a colored background. -->
                  <xsl:when test="Critical[.=1]">
                    <tr>
                      <td>
                        <xsl:value-of select="ID"/>
                      </td>
                      <td>
                        <b>
                          <xsl:value-of select="Name"/>
                        </b>
                      </td>
                      <td>
                        <b>
                          <xsl:value-of select="Priority"/>
                        </b>
                      </td>
                      <td>
                        <b>
                          <xsl:value-of select="Start"/>
                        </b>
                      </td>
                      <td>
                        <b>
                          <xsl:value-of select="Finish"/>
                        </b>
                      </td>
                    </tr>
                  </xsl:when>
                  <!-- Display information for noncritical tasks with a white background. -->
                  <xsl:otherwise>
                    <tr>
                      <td>
                        <xsl:value-of select="ID"/>
                      </td>
                      <td>
                        <xsl:value-of select="Name"/>
                      </td>
                      <td>
                        <xsl:value-of select="Priority"/>
                      </td>
                      <td>
                        <xsl:value-of select="Start"/>
                      </td>
                      <td>
                        <xsl:value-of select="Finish"/>
                      </td>
                    </tr>
                  </xsl:otherwise>
                </xsl:choose>
              </xsl:if>
            </xsl:for-each>
            <!-- Define headers for overallocated resource information. -->
            <tr>
              <td colspan="5" align="center">
                Overallocated Resources:
              </td>
            </tr>
            <tr>
              <th>
                <font color="black">ID</font>
              </th>
              <th colspan="2">
                <font color="black">Name</font>
              </th>
              <th colspan="2">
                <font color="black">Overtime Rate</font>
              </th>
            </tr>
            <!-- Filter for resources -->
            <xsl:for-each select="Project/Resources/Resource">
              <!-- Sort resources alphabetically by name -->
              <xsl:sort select="Name" />
              <!-- Display information for only resources that are overallocated. -->
              <xsl:if test="OverAllocated[.=1]">
                <tr>
                  <td>
                    <xsl:value-of select="ID"/>
                  </td>
                  <td  colspan="2">
                    <xsl:value-of select="Name"/>
                  </td>
                  <td  colspan="2" align="center">
                    $<xsl:value-of select="OvertimeRate"/>.00
                  </td>
                </tr>
              </xsl:if>
            </xsl:for-each>
          </table>

    ```

4.  ファイルを **ProjectTransform.xslt** として保存します。

XSLT スタイルシートを作成した後、処理命令を追加することで Project XML ファイルをスタイルシートにリンクする必要があります。手順 2. では、手順 1. で作成した ProjectTransform.xslt ファイルを Project XML ファイルにリンクする方法を示します。

### 手順 2. XSLT スタイルシートを使用するように Project XML ファイルを変更するには

1.  Visual Studio またはその他のテキスト エディタか XML エディタで、Project XML ファイルを開きます。

2.  Project XML ファイルの先頭の行である XML 宣言の後に、次のコード行を挿入します。
    
    ``` xml
    <?xml-stylesheet type="text/xsl" href="ProjectTransform.xslt"?>
    ```

3.  Project XML ファイルのルート要素である **Project** 要素の内側から、XML 名前空間の宣言を削除します。**Project** 要素に埋め込まれている名前空間宣言を削除しないと、XPath ステートメントが Project XML ファイル内の要素と一致しなくなります。
    
    ステップ 2. および 3. を行った後、Project XML ファイルの最初の 3 行は次のコード例のようになります。
    
    ``` xml
    <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
    <?xml-stylesheet type="text/xsl" href=" ProjectTransform.xslt"?>
    <Project>
    ```

4.  Project XML ファイルを保存します。
    
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
    <td><p>ステップ 3. で行った変更により Project XML ファイルは Project XML データ交換スキーマとの関連づけがなくなっているので、元の Project XML ファイル名とは異なるファイル名を使用して、ファイルを保存することをお勧めします。</p></td>
    </tr>
    </tbody>
    </table>


5.  変換された Project XML ファイルを表示します。Visual Studio では、Project XML ファイルの Stylesheet プロパティを ProjectTransform.xslt に設定した後、\[XML\] メニューの \[XSLT の出力を表示\] を選択することで、XSLT の変換を実行できます。
    
    Project XML ファイルは、Internet Explorer 7、Microsoft Office Word 2007、または XSLT をサポートする他のアプリケーションで開くこともできます。

図 1 は、Project XML ファイルの変換された出力を Word 2007 で表示したものです。Project XML ファイルを開くと、既定で \[データのみ\] データ ビューが表示されます。変換後の出力を表示するには、\[XML ドキュメント\] ウィンドウで ProjectTransform.xslt データ ビューを選択する必要があります。


図 1. 変換された Project XML ファイル (画面は英語版のものです)

  

![変換されたプロジェクト XML ファイル](images/Bb968529.61e5a9b7-d538-4b07-941f-9df8a4da2a4e(ja-jp,office.12).gif)

## 参照

#### その他の技術情報

[XML 形式でプロジェクトを保存および開く](saving-and-opening-projects-in-xml-format.md)  
[What is XSLT? (英語)](http://msdn2.microsoft.com/en-us/library/ms759096.aspx)  
[XSLT リファレンス](http://msdn2.microsoft.com/ja-jp/library/ms256069.aspx)  
[XPath リファレンス](http://msdn2.microsoft.com/ja-jp/library/ms256115.aspx)

