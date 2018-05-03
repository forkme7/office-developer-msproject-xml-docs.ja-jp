---
title: WeekDay 要素
TOCTitle: WeekDay 要素
ms:assetid: 20e6a844-282c-4007-b7e6-414d2d402ac1
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968433(v=office.12)
ms:contentKeyID: 16733118
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# WeekDay 要素

稼働日は、週の曜日またはカレンダーの例外日を定義します。

    <WeekDay>
      ComplexTypeValue
    </WeekDay>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="weekdays-element.md">WeekDays</a></p></td>
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
<td><p><a href="daytype-element.md">DayType</a></p></td>
<td><p>必須</p></td>
<td><p>稼働日の種類 (例外、または月曜日～日曜日)。</p></td>
</tr>
<tr class="even">
<td><p><a href="dayworking-element-calendar.md">DayWorking</a></p></td>
<td><p>オプション</p></td>
<td><p>指定された日付または日付の種類が稼働日であるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="timeperiod-element-calendar.md">TimePeriod</a></p></td>
<td><p>オプション</p></td>
<td><p>一連の例外日を定義します。</p></td>
</tr>
<tr class="even">
<td><p><a href="workingtimes-element-calendar.md">WorkingTime</a></p></td>
<td><p>オプション</p></td>
<td><p>作業した時間を定義する稼働時間のコレクション。</p></td>
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

以下の例では、土曜日 (**DayType** = 7) および日曜日 (**DayType** = 1) は非稼働日です。

``` xml
<WeekDays>
   <WeekDay>
      <DayType>1</DayType>
      <DayWorking>0</DayWorking>
   </WeekDay>
   <WeekDay>
      <DayType>2</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>3</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>4</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>5</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>6</DayType>
      <DayWorking>1</DayWorking>
      <WorkingTimes>
         <WorkingTime>
            <FromTime>08:00:00</FromTime>
            <ToTime>12:00:00</ToTime>
         </WorkingTime>
         <WorkingTime>
            <FromTime>13:00:00</FromTime>
            <ToTime>17:00:00</ToTime>
         </WorkingTime>
      </WorkingTimes>
   </WeekDay>
   <WeekDay>
      <DayType>7</DayType>
      <DayWorking>0</DayWorking>
   </WeekDay>
</WeekDays>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

