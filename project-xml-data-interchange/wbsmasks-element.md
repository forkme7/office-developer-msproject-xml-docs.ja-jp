---
title: WBSMasks 要素
TOCTitle: WBSMasks 要素
ms:assetid: 8901ca64-c183-4be9-895a-53d25a9975c4
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968580(v=office.12)
ms:contentKeyID: 16741551
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WBSMasks 要素

WBS (Work Breakdown Structure) マスクを定義する要素のコレクション。

    <WBSMasks>
      ComplexTypeValue
    </WBSMasks>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
</tr>
</tbody>
</table>


## 子要素


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
<td><p><a href="verifyuniquecodes-element.md">VerifyUniqueCodes</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいタスクの WBS 番号が一意であるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="generatecodes-element.md">GenerateCodes</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいタスクの WBS 番号が生成されるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="prefix-element.md">Prefix</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての WBS 番号の接頭文字。</p></td>
</tr>
<tr class="even">
<td><p><a href="wbsmask-element.md">WBSMask</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのすべてのタスクに適用される WBS マスク。</p></td>
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


## 例

次の例では、WBS マスクに 2 つのユーザー設定 **WBSMask** レベルがあります。レベル 1 は 3 桁の数字、レベル 2 は 2 桁の小文字です。各タスク例の WBS 値を表に示します。**GenerateCodes** = 1 なので、Project はアウトライン レベル 1 および 2 の WBS 値を生成しました。タスクが削除されていますが (UID = 2 のタスク)、WBS 番号が一意である必要はなく、タスク T2 の WBS 値は 002、削除されたタスクの WBS 値も 002 です。

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>タスク</th>
<th>タスクのアウトライン レベル</th>
<th>WBS 値</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>T1</p></td>
<td><p>1</p></td>
<td><p>001</p></td>
</tr>
<tr class="even">
<td><p>st1</p></td>
<td><p>2</p></td>
<td><p>001.aa</p></td>
</tr>
<tr class="odd">
<td><p>st2</p></td>
<td><p>2</p></td>
<td><p>001.ab</p></td>
</tr>
<tr class="even">
<td><p>ss1</p></td>
<td><p>3</p></td>
<td><p>001.ab.1</p></td>
</tr>
<tr class="odd">
<td><p>ss2</p></td>
<td><p>3</p></td>
<td><p>001.ab.2</p></td>
</tr>
<tr class="even">
<td><p>T2</p></td>
<td><p>1</p></td>
<td><p>002</p></td>
</tr>
</tbody>
</table>


``` xml
<Project>
   . . .
   <WBSMasks>
      <VerifyUniqueCodes>0</VerifyUniqueCodes>
      <GenerateCodes>1</GenerateCodes>
      <Masks>
         <WBSMask>
            <Level>1</Level>
            <Type>0</Type>
            <Length>3</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>2</Level>
            <Type>2</Type>
            <Length>2</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
   </WBSMasks>
   . . .
   <Tasks>
      . . .
      <Task>
         <UID>1</UID>
         <ID>1</ID>
         <Name>T1</Name>
         <Type>1</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001</WBS>
         <WBSLevel>001</WBSLevel>
         <OutlineNumber>1</OutlineNumber>
         <OutlineLevel>1</OutlineLevel>
         . . .
      </Task>
      <Task>
         <UID>3</UID>
         <ID>2</ID>
         <Name>st1</Name>
         <Type>0</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001.aa</WBS>
         <WBSLevel>aa</WBSLevel>
         <OutlineNumber>1.1</OutlineNumber>
         <OutlineLevel>2</OutlineLevel>
         . . .
      </Task>
      <Task>
         <UID>4</UID>
         <ID>3</ID>
         <Name>st2</Name>
         <Type>1</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001.ab</WBS>
         <WBSLevel>ab</WBSLevel>
         <OutlineNumber>1.2</OutlineNumber>
         <OutlineLevel>2</OutlineLevel>
         . . .
      </Task>
      . . .
   </Tasks>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)  
[WBSMasks 要素の XML スキーマ](xml-schema-for-the-wbsmasks-element.md)

