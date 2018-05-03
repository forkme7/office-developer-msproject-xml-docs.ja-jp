---
title: FieldGUID 要素
TOCTitle: FieldGUID 要素
ms:assetid: aa629c7c-8921-42c6-9f82-000baf39c3fa
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968634(v=office.12)
ms:contentKeyID: 16744242
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# FieldGUID 要素

アウトライン コード値のグローバル一意識別子 (GUID) です。

    <FieldGUID>
      StringValue
    </FieldGUID>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="value-element.md">Value</a></p></td>
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

**FieldGUID** は、タスクまたはリソースのアウトライン コード値の [ValueGUID](valueguid-element.md) 要素に対応します。

## 例

以下の例では、アウトライン コードが 2 つの値を持ちます。各値は、任意の数の文字に対するコード マスクを満たします (マスク **Type** は 3、マスク **Length** は 0 です)。

**ValueID** はオブジェクト内でのみ一意であり、**FieldGUID** はすべてのプロジェクトで一意です。**ValueID** は、Microsoft Office Project 2003 が Project 2007 から保存された XML ファイルを読み取るために必要です。Project 2007 は **ValueID** を無視し、**FieldGUID** を使用します。

``` xml
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
```

## 参照

#### その他の技術情報

[ValueID 要素](valueid-element.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)

