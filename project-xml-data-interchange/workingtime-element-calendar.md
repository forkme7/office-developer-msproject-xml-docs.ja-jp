---
title: WorkingTime 要素 (Calendar)
TOCTitle: WorkingTime 要素
ms:assetid: 8df6f9e2-701d-4ea4-87a9-8b3e6debd4b7
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968585(v=office.12)
ms:contentKeyID: 16741989
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WorkingTime 要素 (Calendar)

稼働日の作業の期間、またはカレンダーの例外の期間を、最大 5 つ定義します。

    <WorkingTime>
      ComplexTypeValue
    </WorkingTime>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workingtimes-element-calendar.md">WorkingTimes</a></p></td>
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
<td><p><a href="fromtime-element-calendar.md">FromTime</a></p></td>
<td><p>オプション</p></td>
<td><p>稼働開始時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="totime-element-calendar.md">ToTime</a></p></td>
<td><p>オプション</p></td>
<td><p>稼働終了時間。</p></td>
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
<p>最大 : 5</p></td>
</tr>
</tbody>
</table>


## 備考

**WorkingTimes** コレクションには、**WorkingTime** が少なくとも 1 つ指定されている必要があります。また、**WorkingTime** 要素は 5 つまでしか指定できません。

## 例

次の例では、1 日の 2 つの **WorkingTime** 期間を指定しています。

``` xml
<WorkingTimes>
   <WorkingTime>
      <FromTime>09:00:00</FromTime>
      <ToTime>12:00:00</ToTime>
   </WorkingTime>
   <WorkingTime>
      <FromTime>13:00:00</FromTime>
      <ToTime>17:00:00</ToTime>
   </WorkingTime>
</WorkingTimes>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

