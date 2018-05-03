---
title: WBSMask 要素
TOCTitle: WBSMask 要素
ms:assetid: ae403c08-a9a6-4116-933f-aaa6202ffda9
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968641(v=office.12)
ms:contentKeyID: 16744553
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WBSMask 要素

プロジェクト内のすべてのタスクに適用される Work Breakdown Structure (WBS) マスクです。

    <WBSMask>
      ComplexTypeValue
    </WBSMask>

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
<td><p><a href="level-element.md">Level</a></p></td>
<td><p>必須</p></td>
<td><p>1 から始まる WBS レベルの番号です。</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>必須</p></td>
<td><p>最初のレベルのタスクのコード文字列の種類です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="length-element.md">Length</a></p></td>
<td><p>必須</p></td>
<td><p>WBS マスク値に必要な文字の数 (1 ～ 255) です。任意の数の文字を使用できる場合、<strong>Length</strong> はゼロです。</p></td>
</tr>
<tr class="even">
<td><p><a href="separator-element.md">Separator</a></p></td>
<td><p>必須</p></td>
<td><p>WBS マスク レベルを区切るために使用される文字です。</p></td>
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


## 例

以下の例では、WBS マスク内の 3 つのレベルと、1 つのグローバル プレフィックスが存在します。レベル 1 は大文字の型で、レベル 2 は数値で、レベル 3 は任意の長さの順序付けされていない文字です。各タスク例の WBS 値を表に示します。ユーザーは WBS レベル 3 の値を入力しています。Project は他の WBS 値を生成しています。タスクは削除され、WBS コードは一意である必要があるため、タスク T2 には WBS 値 Test-AC があります。削除されたタスクの WBS 値は Test-AB でした。


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

