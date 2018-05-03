---
title: WorkingTimes 要素 (Calendar)
TOCTitle: WorkingTimes 要素
ms:assetid: 09d7e8d2-2573-4fed-9cc9-235bf1e1a3a2
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968403(v=office.12)
ms:contentKeyID: 16731361
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WorkingTimes 要素 (Calendar)

稼働日またはカレンダー例外の作業に使用された時間を定義する稼働時間のコレクションです。

    <WorkingTimes>
      ComplexTypeValue
    </WorkingTimes>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekday-element.md">WeekDay</a></p></td>
</tr>
</tbody>
</table>


## 子要素


<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="workingtime-element-calendar.md">WorkingTime</a></p></td>
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

**WorkingTimes** コレクションは少なくとも 1 つの **WorkingTime** 要素を含む必要があり、最大 5 つの **WorkingTime** 要素を含むことができます。

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

