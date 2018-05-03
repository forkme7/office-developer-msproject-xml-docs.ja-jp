---
title: ValueGUID 要素
TOCTitle: ValueGUID 要素
ms:assetid: 8478818f-6da6-431f-b4d0-d2113329a476
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968572(v=office.12)
ms:contentKeyID: 16741168
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# ValueGUID 要素

リソースまたはタスクのアウトライン コードまたはユーザー設定フィールドの値のグローバル一意識別子 (GUID)。

    <ValueGUID>
      StringValue
    </ValueGUID>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a>、<a href="outlinecode-element.md">OutlineCode</a></p></td>
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
<td><p>最小 : 1</p>
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

**string** 型のテキスト値が必要です。この **string** は、"HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" の形式 ("H" は 0 ～ F の 16 進数を表します) になっている必要があります。

## 備考

リソースまたはタスクのアウトライン コード値の **ValueGUID** は、アウトライン コード定義の **FieldGUID** の値に対応します。

タスクまたはリソースのユーザー設定フィールドを割り当てにロールダウンした場合、**Assignment** 要素には、**ValueGUID** の **ExtendedAttribute** が含まれます。

## 例

次の例では、タスクのアウトライン コードの **ValueGUID** と **ValueID** はどちらも、*Task Simple OC* という名前のアウトライン コードの *Simple 2* の値に対応します。

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

[OutlineCode 要素](outlinecode-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

