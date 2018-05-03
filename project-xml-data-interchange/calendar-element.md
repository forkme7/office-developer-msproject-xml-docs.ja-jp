---
title: Calendar 要素
TOCTitle: Calendar 要素
ms:assetid: 4232bf41-6652-4763-a885-ba0c1c520152
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968481(v=office.12)
ms:contentKeyID: 16735839
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Calendar 要素

Microsoft Office Project では、カレンダーは標準の稼働時間および非稼働時間を定義するために使用します。プロジェクトには、少なくとも 1 つの基本カレンダーが必要です。タスクおよびリソースには、基本カレンダーに基づいた独自のカレンダーを設定できます。

    <Calendar>
      ComplexTypeValue
    </Calendar>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendars-element.md">Calendars</a></p></td>
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
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>必須</p></td>
<td><p>カレンダーの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーの名前。</p></td>
</tr>
<tr class="odd">
<td><p><a href="isbasecalendar-element.md">IsBaseCalendar</a></p></td>
<td><p>オプション</p></td>
<td><p>カレンダーが基本カレンダーであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="basecalendaruid-element.md">BaseCalendarUID</a></p></td>
<td><p>オプション</p></td>
<td><p>このカレンダーが依存する基本カレンダーの一意の ID。このカレンダーが基本カレンダーではない場合にのみ使用されます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="weekdays-element.md">WeekDays</a></p></td>
<td><p>オプション</p></td>
<td><p>稼働日の種類 (曜日または例外)。</p></td>
</tr>
<tr class="even">
<td><p><a href="exceptions-element.md">Exceptions</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。カレンダーに関連付けられた例外のコレクションです。</p></td>
</tr>
<tr class="odd">
<td><p><a href="workweeks-element.md">WorkWeeks</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。稼働日の定義のコレクションです。</p></td>
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
<p>最大 : 制約なし</p></td>
</tr>
</tbody>
</table>


## 例

次の例は、Team Base Calendar という名前のローカルなカレンダーを示します。このカレンダーは、別のカレンダーのコピーではなく、基本カレンダーとして作成されます。

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968496.Caution(ja-jp,office.12).gif" alt="Caution note" class="note" />注意 :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>Project 2007 SP1 までのリリースでは、既定以外の稼働日を持つプロジェクトを XML として保存すると、<strong>WorkWeeks</strong> 要素名が失われます。XML ファイルを Project で開こうとすると、&quot;ファイルを読み込み中に予期しない問題が発生しました。このファイルは壊れている可能性があります。&quot;というエラー メッセージが表示されます。この回避策としては、XML ファイルを編集して、次の例に示すように <strong>WorkWeeks</strong> 要素名を追加します。これで、XML ファイルは正常に開きます。ただし、<strong>WorkWeek</strong> 要素には他のエラーも含まれているので、今後のサービス パックでエラーが修正されるまでは、稼働日を保存する場合は Project XML ファイルを使用しないことをお勧めします。他の稼働日要素の編集の詳細については、「<a href="workweek-element.md">WorkWeek 要素</a>」を参照してください。</p></td>
</tr>
</tbody>
</table>


``` xml
<Calendar>
   <UID>5</UID>
   <Name>Team Base Calendar</Name>
   <IsBaseCalendar>1</IsBaseCalendar>
   <BaseCalendarUID>-1</BaseCalendarUID>
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
      . . .
   </WeekDays>
   <Exceptions>
      <Exception>
         <EnteredByOccurrences>0</EnteredByOccurrences>
         <TimePeriod>
            <FromDate>2007-11-22T00:00:00</FromDate>
            <ToDate>2007-11-23T23:59:00</ToDate>
         </TimePeriod>
         <Occurrences>2</Occurrences>
         <Name>Thanksgiving holidays</Name>
         <Type>1</Type>
         <DayWorking>0</DayWorking>
      </Exception>
   </Exceptions>
   <WorkWeeks>
      <WorkWeek>
         <TimePeriod>
            <FromDate>2007-11-26T00:00:00</FromDate>
            <ToDate>2007-11-26T23:59:00</ToDate>
         </TimePeriod>
         <Name>Post-holiday working days</Name>
      </WorkWeek>
   </WorkWeeks>
</Calendar>
```

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

