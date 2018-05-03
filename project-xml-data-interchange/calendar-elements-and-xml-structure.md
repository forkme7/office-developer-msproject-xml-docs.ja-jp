---
title: Calendar 要素と XML データ構造
TOCTitle: Calendar 要素と XML データ構造
ms:assetid: 8147b68c-654d-405e-9878-73548c661689
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968563(v=office.12)
ms:contentKeyID: 16740919
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Calendar 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **Calendars** 要素の子について説明します。この要素は、プロジェクトを XML 形式で保存するときのカレンダー データを表します。

**Calendars** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## Calendar 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **Calendar** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素の有効なテキスト値の詳細については、「[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)」に埋め込まれているドキュメント注釈を参照してください。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

\<[Calendars](calendars-element.md)\>

    \<[Calendar](calendar-element.md)\>

        \<[UID](uid-element.md)\>**integer**\</UID\>

        \<[Name](name-element.md)\>**string**\</Name\>

        \<[IsBaseCalendar](isbasecalendar-element.md)\>**boolean**\</IsBaseCalendar\>

        \<[BaseCalendarUID](basecalendaruid-element.md)\>**integer**\</BaseCalendarUID\>

        \<[WeekDays](weekdays-element.md)\>

            \<[WeekDay](weekday-element.md)\>

                \<[DayType](daytype-element.md)\>**integer**\</DayType\>

                \<[DayWorking](dayworking-element-calendar.md)\>**boolean**\</DayWorking\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>**dateTime**\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>**dateTime**\</ToDate\>

                \</TimePeriod\>

                \<[WorkingTimes](workingtimes-element-calendar.md)\>

                    \<[WorkingTime](workingtime-element-calendar.md)\>

                        \<[FromTime](fromtime-element-calendar.md)\>**time**\</FromTime\>

                        \<[ToTime](totime-element-calendar.md)\>**time**\</Time\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</WeekDay\>

        \</WeekDays\>

        \<[Exceptions](exceptions-element.md)\>

            \<[Exception](exception-element.md)\>

                \<[EnteredByOccurrences](enteredbyoccurrences-element.md)\>**boolean**\</EnteredByOccurrences\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>**dateTime**\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>**dateTime**\</ToDate\>

                \</TimePeriod\>

                \<[Occurrences](occurrences-element.md)\>**integer**\</Occurrences\>

                \<[Name](name-element.md)\>**string**\</Name\>

                \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

                \<[Period](period-element.md)\>**integer**\</Period\>

                \<[DaysOfWeek](daysofweek-element.md)\>**integer**\</DaysOfWeek\>

                \<[MonthItem](monthitem-element.md)\>**integer**\</MonthItem\>

                \<[MonthPosition](monthposition-element.md)\>**integer**\</MonthPosition\>

                \<[Month](month-element.md)\>**integer**\</Month\>

                \<[MonthDay](monthday-element.md)\>**integer**\</MonthDay\>

                \<[DayWorking](dayworking-element-calendar.md)\>**boolean**\</DayWorking\>

                \<[WorkingTimes](workingtimes-element-calendar.md)\>

                    \<[WorkingTime](workingtime-element-calendar.md)\>

                        \<[FromTime](fromtime-element-calendar.md)\>**time**\</FromTime\>

                        \<[ToTime](totime-element-calendar.md)\>**time**\</ToTime\>

                    \</WorkingTime\>

                \</WorkingTimes\>

            \</Exception\>

        \</Exceptions\>

        \<[WorkWeeks](workweeks-element.md)\>   \<\!-- 「**WorkWeeks**」トピックおよび「**WorkWeek**」トピックのメモを参照 --\>

            \<[WorkWeek](workweek-element.md)\>

                \<[TimePeriod](timeperiod-element-calendar.md)\>

                    \<[FromDate](fromdate-element-calendar.md)\>**dateTime**\</FromDate\>

                    \<[ToDate](todate-element-calendar.md)\>**dateTime**\</ToDate\>

                \</TimePeriod\>

                \<[Name](name-element.md)\>**string**\</Name\>

                \<[WeekDay](weekday-element.md)\>

                    \<[DayType](daytype-element.md)\>**integer**\</DayType\>

                    \<[DayWorking](dayworking-element-calendar.md)\>**boolean**\</DayWorking\>

                \</WeekDay\>

            \</WorkWeek\>

        \</WorkWeeks\>

    \</Calendar\>

\</Calendars\>

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)

