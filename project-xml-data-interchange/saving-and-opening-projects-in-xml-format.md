---
title: XML 形式でプロジェクトを保存および開く
TOCTitle: XML 形式でプロジェクトを保存および開く
ms:assetid: a18319b3-7884-48bf-b45d-cecd756cc350
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968621(v=office.12)
ms:contentKeyID: 16743581
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# XML 形式でプロジェクトを保存および開く

Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) は、Project 2007 がプロジェクト データを XML 形式で読み書きする方法を定義します。ここでは、Project 2007 XML データ交換ファイルを操作する方法について説明します。内容は以下のとおりです。

  - Project Professional 2007 を使用して Project ファイルを XML として保存する

  - Project Professional 2007 を使用して Project XML ファイルを開く

## プロジェクト ファイルを XML として保存する

Project Standard 2007 および Project Professional 2007 では、すべてのプロジェクトを Project XML データ交換ファイルとして保存できます。手順 1. のステップは、Project Professional に適用されます。

Project XML ファイルに格納されたプロジェクト データは、XSLT 変換を使用してフィルタ処理したり、表示したりすることができます。詳細については、「[\[方法\] Project XML データ交換ファイルで XSLT 変換を使用する](how-to-use-xslt-transformations-with-project-xml-data-interchange-files.md)」を参照してください。

### 手順 1. Project Professional を使用してプロジェクト ファイルを XML として保存するには

1.  Project Professional で、\[ファイル\] メニューの \[名前を付けて保存\] をクリックします。

2.  \[Project Server に保存\] ダイアログ ボックス (図 1) で、\[ファイルとして保存\] をクリックします。
    
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
    <td><p>Project Professional 2007 をスタンドアロン環境で操作している場合、[Project Server に保存] ダイアログ ボックス (図 1) や [ファイルとして保存] ダイアログ ボックス (図 2) は表示されません。[名前を付けて保存] ダイアログ ボックスだけが表示されます。</p></td>
    </tr>
    </tbody>
    </table>
    
    
    図 1. \[Project Server に保存\] ダイアログ ボックス (画面は英語版のものです)
    
      
    
    ![\[Project Server に保存\] ダイアログ ボックス](images/Bb968621.0b5b6b1e-a165-4f9b-a916-af139c2ce94c(ja-jp,office.12).gif)

3.  \[ファイルとして保存\] ダイアログ ボックスでは、ファイルを現在読み込まれているエンタープライズ アイテムのみと共に保存するか、またはすべてのエンタープライズ アイテムと共に保存することができます。現在読み込まれているエンタープライズ アイテムのみを保存するオプションを選択すると、プロジェクトの構成によっては、ファイルが小さくなることがあります。
    
    オプションを選択したら、\[OK\] をクリックします。
    
    
    図 2. \[ファイルとして保存\] ダイアログ ボックス (画面は英語版のものです)
    
      
    
    ![\[ファイルに保存\] ダイアログ ボックス](images/Bb968621.abe3829c-e8fd-4983-b175-5a93c4625d40(ja-jp,office.12).gif)

4.  \[名前を付けて保存\] ダイアログ ボックスで、ファイルを保存する場所に移動します。

5.  \[ファイルの種類\] の一覧で、\[XML 形式 (\*.xml)\] を手動で選択し、\[保存\] をクリックします。\*.xml オプションを選択しない場合、プロジェクトは既定の Project ファイル形式 (.mpp) を使用して保存されます。

## Project XML ファイルを開く

Project Standard 2007 および Project Professional 2007 では、任意の有効な Project 2007 データ交換ファイルを開くことができます。Project Standard は、エンタープライズ プロジェクトのみに適用される XML データを無視します。開いた Project XML ファイルは、他のプロジェクトと同じように機能します。

### 手順 2. Project XML ファイルを開くには

1.  Project Professional 2007 で、\[ファイル\] メニューの \[開く\] をクリックします。
    
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
    <td><p>Windows Explorer ウィンドウを使用し、Project XML ファイルを右クリックし、[次のプログラムで開く] メニューの [Microsoft Office Project] を選択することにより、Project XML ファイルを開くこともできます。この方法を使用して Project XML ファイルを開くと、図 4 に示す [インポート ウィザード] ウィザードが直ちに表示されます。</p></td>
    </tr>
    </tbody>
    </table>


2.  \[開く\] ダイアログ ボックス (図 3) で、\[開く\] ダイアログ ボックスの左側に表示される \[探す場所\] ウィンドウのオプション (たとえば、\[マイ ドキュメント\]) を選択し、開く XML ファイルの場所に移動します。
    
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
    <td><p>[開く] ダイアログ ボックスで XML ファイルを表示するには、[ファイルの種類] の一覧で [XML 形式 (*.xml)] または [すべてのファイル (*.*)] を手動で選択する必要があります。図 3 に、Project Professional の [開く] ダイアログ ボックスを示します。</p></td>
    </tr>
    </tbody>
    </table>
    
    開く XML ファイルを選択し、\[開く\] をクリックします。または、開く XML ファイルをダブルクリックします。
    
    
    図 3. \[開く\] ダイアログ ボックス (画面は英語版のものです)
    
      
    
    ![\[開く\] ダイアログ ボックス](images/Bb968621.47e92179-d5b6-4b1b-8a28-68efb43aaf66(ja-jp,office.12).gif)

3.  \[インポート ウィザード\] ウィザードが起動します (図 4)。
    
    
    図 4. インポート ウィザード (画面は英語版のものです)
    
      
    
    ![インポート ウィザード](images/Bb968621.59cec313-e2fe-4c16-8ae0-d013ce2dfc07(ja-jp,office.12).gif)
    
    XML ファイルのインポート方法を選択し、\[完了\] をクリックします。
    
      - **新しいプロジェクトとしてインポートする**  XML ファイルから新しいプロジェクトを作成します。
    
      - **作業中のプロジェクトにデータを追加する**  Project Professional で現在作業中の既存のプロジェクトに、XML ファイル内のプロジェクト データを追加します。
        
        Project 2007 が既存のプロジェクトに XML データを追加すると、追加されるサマリー タスクの一意の ID が、0 から次に使用可能な整数にインクリメントされます。たとえば、XML データを追加しているプロジェクトに一意の ID が 1、2、および 3 である 3 つのタスクが含まれる場合、追加されるサマリー タスクには一意の ID 4 が与えられます。その後、Project は追加されるプロジェクト内のすべてのタスクの一意の ID をインクリメントします。同じ例を使用すると、追加されるプロジェクト内のタスク 1 およびタスク 2 には、次に使用可能な一意の ID である 5 および 6 が割り当てられます。
        
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
        <td><p>このプロセスにより、割り当て、タスク、リソース、およびプロジェクト間のリンクと、元のデータの関連付けが解除されることがあります。データの関連付けが解除されないようにするには、このデータを可能な限り小さなコンポーネント (タスク、リソース、割り当てなど) に分離してから、追加作業を行います。</p></td>
        </tr>
        </tbody>
        </table>
    
      - **作業中のプロジェクトにデータを結合する**  Project Professional で現在作業中のプロジェクトに XML ファイル内のプロジェクト データを結合します。
        
        Project 2007 が既存のプロジェクトに XML データを結合すると、Project Professional で現在作業中のプロジェクト ファイル内のタスクは、同じ一意の ID を共有する XML ファイル内のタスクによって上書きされます。
        
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
        <td><p>XML データを作業中のプロジェクトに結合するときは、データが失われることがあるので、注意が必要です。</p></td>
        </tr>
        </tbody>
        </table>
        
        XML ファイルが Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) に照らして有効ではない場合、Project は図 5 に示すようなエラー メッセージを表示します。
        
        
        図 5. Project のエラー メッセージ (画面は英語版のものです)
        
          
        
        ![MIcrosoft Office Project のエラー メッセージ](images/Bb968621.f9b52597-9fd8-4baa-a870-97a5049d9316(ja-jp,office.12).gif)

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project データ交換の要素](project-data-interchange-elements.md)  
[\[方法\] Project XML データ交換ファイルで XSLT 変換を使用する](how-to-use-xslt-transformations-with-project-xml-data-interchange-files.md)

