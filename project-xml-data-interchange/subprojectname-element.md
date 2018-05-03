---
title: SubprojectName 要素
TOCTitle: SubprojectName 要素
ms:assetid: ba94763e-8c0a-4fe2-997c-cd85f5352ca3
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968656(v=office.12)
ms:contentKeyID: 16745571
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# SubprojectName 要素

挿入プロジェクトのソースの場所です。

    <SubprojectName>
      String(512)Value
    </SubprojectName>

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


## 備考

サブプロジェクトのソースには、Project Server 内のファイルやプロジェクトを使用できます。

## 例

以下の例では、マスタ プロジェクトにタスク ID 3 として挿入されたローカル プロジェクト ファイルを `C:\Project\P12\XML\Samples\SubProj.mpp` というフルパス名で示します。マスタ プロジェクトの XML ファイルには、挿入プロジェクトの完全な **Project** 要素が、タスク ID 3 の子として含まれます。

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

