---
title: IsSubproject 要素
TOCTitle: IsSubproject 要素
ms:assetid: a7dcc251-f796-4d75-8146-040fe30c066b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968630(v=office.12)
ms:contentKeyID: 16744058
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# IsSubproject 要素

タスクが挿入プロジェクトであるかどうかを示します。

    <IsSubproject>
      BooleanValue
    </IsSubproject>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## テキスト値

**boolean** 型のテキスト値が必要です。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>値</th>
<th>説明</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>


## 例

以下の例は、タスク ID 3 としてマスタ プロジェクトに挿入されたローカル プロジェクト ファイルを示しています。マスタ プロジェクトの XML ファイルには、挿入プロジェクトの完全な **Project** 要素が、タスク ID 3 の子として含まれます。

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <Tasks>
      . . .
      <Task>
         <UID>4</UID>
         <ID>3</ID>
         <Name>SubProj</Name>
         <Type>1</Type>
         . . .
         <Summary>1</Summary>
         <Critical>1</Critical>
         <IsSubproject>1</IsSubproject>
         <IsSubprojectReadOnly>0</IsSubprojectReadOnly>
         <SubprojectName>C:\Project\P12\XML\Samples\SubProj.mpp</SubprojectName>
         <ExternalTask>0</ExternalTask>
         . . .
         <Project xmlns="http://schemas.microsoft.com/project">
            . . .
            <Tasks>
               <Task>
                  . . .
               </Task>
               . . .
            </Tasks>
            . . .
         </Project>
      </Task>
   </Tasks>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

