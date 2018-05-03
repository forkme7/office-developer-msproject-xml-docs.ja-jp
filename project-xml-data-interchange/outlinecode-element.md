---
title: OutlineCode 要素
TOCTitle: OutlineCode 要素
ms:assetid: 0dc0478b-4281-4e0e-86c0-3fdea445e6d0
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968410(v=office.12)
ms:contentKeyID: 16731650
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# OutlineCode 要素

プロジェクト内のアウトライン コードおよび関連する値リストを定義するか、リソースまたはタスクのアウトライン コード要素の値を指定します。

    <OutlineCode>
      ComplexTypeValue
    </OutlineCode>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="outlinecodes-element.md">OutlineCodes</a>、<a href="resource-element.md">Resource</a>、<a href="task-element.md">Task</a></p></td>
</tr>
</tbody>
</table>


## プロジェクト レベルの子要素


<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="guid-element-multiple-parents.md">Guid</a></p></td>
<td><p>必須</p></td>
<td><p>Microsoft Office Project 2007 の新しい要素。アウトライン コードのグローバル一意識別子 (GUID)。関連付けられた <strong>ExtendedAttribute</strong> 値の <strong>Ltuid</strong> 要素に対応します。</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードのフィールド ID 番号。フィールド番号は、リソースおよびタスクのアウトライン コード 1、アウトラインコード 2、. . . アウトライン コード 10 に対応します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="fieldname-element.md">FieldName</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定のアウトライン コードの名前。</p></td>
</tr>
<tr class="even">
<td><p><a href="alias-element.md">Alias</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードのエイリアス。</p></td>
</tr>
<tr class="odd">
<td><p><a href="phoneticalias-element.md">PhoneticAlias</a></p></td>
<td><p>オプション</p></td>
<td><p>ユーザー設定のアウトライン コードのひらがなまたはカタカナでの読みを格納します。日本語版の Project でのみ使用されます。</p></td>
</tr>
<tr class="even">
<td><p><a href="values-element.md">Values</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードの値定義のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="enterprise-element.md">Enterprise</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードがエンタープライズ ユーザー設定フィールドであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="enterpriseoutlinecodealias-element.md">EnterpriseOutlineCodeAlias</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードがエイリアスであるエンタープライズ ユーザー設定フィールドを参照します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="resourcesubstitutionenabled-element.md">ResourceSubstitutionEnabled</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コードが Project のリソースの切り替えウィザードで使用されるかどうかを示します。リソースの切り替えウィザードは、エンタープライズ ユーザー設定フィールドについてのみ使用されます。</p></td>
</tr>
<tr class="even">
<td><p><a href="leafonly-element.md">LeafOnly</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースまたはタスクのアウトライン コードに指定されている値がリーフ値である必要があるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="alllevelsrequired-element.md">AllLevelsRequired</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいコードにすべてのレベルが存在している必要があるかどうかを示します。エンタープライズ ユーザー設定フィールドでは使用されません。</p></td>
</tr>
<tr class="even">
<td><p><a href="onlytablevaluesallowed-element.md">OnlyTableValuesAllowed</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コード値が関連付けられた参照テーブルから取得される必要があるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="masks-element.md">Masks</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コード値リストのコード マスクのコレクション。</p></td>
</tr>
</tbody>
</table>


## タスクおよびリソース レベルの子要素

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>要素</th>
<th>必須/オプション</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>必須</p></td>
<td><p>アウトライン コードのフィールド ID 番号。フィールド番号は、リソースおよびタスクのアウトライン コード 1、アウトラインコード 2、. . . アウトライン コード 10 に対応します。</p></td>
</tr>
<tr class="even">
<td><p><a href="valueid-element.md">ValueID</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン コード定義に関連付けられた <strong>Value</strong> リストのローカル ID 番号。Project 2007 で保存された XML ファイルを Project 2003 で読み取るために必要です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="valueguid-element.md">ValueGUID</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。アウトライン コード値リストでの値の GUID。<strong>ValueGUID</strong> は、<strong>Value</strong> 要素の <strong>FieldGUID</strong> と一致します。</p></td>
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
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 備考

アウトライン コードは、対応するコード マスクおよび値のテーブルと共に、プロジェクト内の **OutlineCodes** のコレクションで定義されます。各アウトライン コードには、関連付けられた **ExtendedAttribute** があり、アウトライン コードのフィールド型とエイリアスを指定します。

アウトライン コード値を格納するリソースまたはタスクには、各値の **OutlineCode** 要素が含まれます。リソースまたはタスクで **OutlineCode** 要素の値を指定するには、以下の 2 つのデータが必要です。

  - **FieldID** 要素で指定されるアウトライン コード定義へのポインタ。

  - 値リスト内の **Value** 要素への **ValueID** および **ValueGUID** ポインタによって指定されるアウトライン コード値。**ValueGUID** は、値リストの **FieldGUID** と一致します。Project 2007 では、**ValueID** は無視され、**ValueGUID** が使用されます。

## 例

次の例では、アウトライン コード定義の **Guid** 値が、関連付けられた **ExtendedAttribute** の **Ltuid** 値に対応します。アウトライン コード エイリアスは、*アウトライン コード 6* フィールド名の *Task Simple OC* です。**FieldID** 188744106 は、「[PjCustomField Enumeration (英語)](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)」に示されている **pjCustomTaskOutlineCode6** 列挙値と一致します。Project の Visual Basic Editor (VBE) でオブジェクト ブラウザを使用して、**PjCustomField** 列挙型の値を検索することもできます。

アウトライン コード マスクは、任意の長さ (**Length** = 3) の 1 レベルの文字 (**Type** = 0) を定義します。

タスクのアウトライン コードの **ValueGUID** および **ValueID** はいずれも、*Task Simple OC* アウトライン コードの *Simple 2* の値に対応します。

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <OutlineCodes>
      <OutlineCode>
         <Guid>26F0CA77-38CC-40C7-933D-15F839F7DB82</Guid>
         <Enterprise>0</Enterprise>
         <ResourceSubstitutionEnabled>0</ResourceSubstitutionEnabled>
         <LeafOnly>0</LeafOnly>
         <AllLevelsRequired>0</AllLevelsRequired>
         <OnlyTableValuesAllowed>0</OnlyTableValuesAllowed>
         <Masks>
            <Mask>
               <Level>1</Level>
               <Type>3</Type>
               <Length>0</Length>
               <Separator>.</Separator>
            </Mask>
         </Masks>
         <Values>
            <Value>
               <ValueID>16</ValueID>
               <FieldGUID>985194AB-77BA-4545-BCE8-99761B5538D9</FieldGUID>
               <ParentValueID>0</ParentValueID>
               <Type>21</Type>
               <Value>Simple 1</Value>
            </Value>
            <Value>
               <ValueID>17</ValueID>
               <FieldGUID>6B0CC455-EE19-416A-8FD9-6209590B3ED7</FieldGUID>
               <ParentValueID>0</ParentValueID>
               <Type>21</Type>
               <Value>Simple 2</Value>
            </Value>
         </Values>
      </OutlineCode>
   </OutlineCodes>
   . . .
   <ExtendedAttributes>
      <ExtendedAttribute>
         <FieldID>188744106</FieldID>
         <FieldName>Outline Code6</FieldName>
         <Alias>Task Simple OC</Alias>
         <Ltuid>26F0CA77-38CC-40C7-933D-15F839F7DB82</Ltuid>
         <SecondaryPID>255869013</SecondaryPID>
      </ExtendedAttribute>
   </ExtendedAttributes>
   . . .
   <Tasks>
      <Task>
         . . .
         <OutlineCode>
            <FieldID>188744106</FieldID>
            <ValueID>17</ValueID>
            <ValueGUID>6B0CC455-EE19-416A-8FD9-6209590B3ED7</ValueGUID>
         </OutlineCode>
         . . .
      </Task>
   </Tasks>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[Ltuid 要素](ltuid-element.md)  
[ExtendedAttribute 要素](extendedattribute-element.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[PjCustomField Enumeration (英語)](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)

