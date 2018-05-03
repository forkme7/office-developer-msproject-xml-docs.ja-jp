---
title: GenerateCodes 要素
TOCTitle: GenerateCodes 要素
ms:assetid: dad4f0e1-faa8-43e3-9eec-ab7df41ddbb6
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968704(v=office.12)
ms:contentKeyID: 16748533
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# GenerateCodes 要素

新しいタスクの WBS 番号が生成されるかどうかを示します。

    <GenerateCodes>
      BooleanValue
    </GenerateCodes>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="wbsmasks-element.md">WBSMasks</a></p></td>
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

以下の例では、WBS マスク内の 3 つのレベルと、1 つのグローバル プレフィックスが存在します。レベル 1 は大文字の型で、レベル 2 は数値で、レベル 3 は任意の長さの順序付けされていない文字です。各タスク例の WBS 値を表に示します。ユーザーは WBS レベル 3 の値を入力しています。**GenerateCodes** = 1 であるため、Project はその他の WBS の値を生成しています。タスクは削除され、WBS コードは一意である必要があるため、タスク T2 には WBS 値 Test-AC があります。削除されたタスクの WBS 値は Test-AB でした。

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
<td><p>Test-AA</p></td>
</tr>
<tr class="even">
<td><p>st1</p></td>
<td><p>2</p></td>
<td><p>Test-AA.001</p></td>
</tr>
<tr class="odd">
<td><p>st2</p></td>
<td><p>2</p></td>
<td><p>Test-AA.002</p></td>
</tr>
<tr class="even">
<td><p>ss1</p></td>
<td><p>3</p></td>
<td><p>Test-AA.002.ThisIsATest</p></td>
</tr>
<tr class="odd">
<td><p>T2</p></td>
<td><p>1</p></td>
<td><p>Test-AC</p></td>
</tr>
</tbody>
</table>


``` xml
<Project>
   . . .
   <WBSMasks>
      <VerifyUniqueCodes>4</VerifyUniqueCodes>
      <GenerateCodes>1</GenerateCodes>
      <Prefix>Test-</Prefix>
      <Masks>
         <WBSMask>
            <Level>1</Level>
            <Type>1</Type>
            <Length>2</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>2</Level>
            <Type>0</Type>
            <Length>3</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>3</Level>
            <Type>3</Type>
            <Length>0</Length>
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
         <CreateDate>2007-11-13T13:34:00</CreateDate>
         <WBS>Test-AA</WBS>
         <WBSLevel>AA</WBSLevel>
         . . .
      </Task>
      . . .
   </Tasks>
   . . .
</Project>
```

## 参照

#### その他の技術情報

[WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)  
[WBSMasks 要素の XML スキーマ](xml-schema-for-the-wbsmasks-element.md)

