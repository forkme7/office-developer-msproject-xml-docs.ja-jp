---
title: Project 要素と XML データ構造
TOCTitle: Project 要素と XML データ構造
ms:assetid: 23b2326a-66cf-4978-a982-48567ded715b
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968439(v=office.12)
ms:contentKeyID: 16733324
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Project 要素と XML データ構造

このセクションには、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **Project** 要素と **Project** 要素の子に関する情報が含まれます。これらの要素は、プロジェクトを XML 形式で保存するときのプロジェクト データを表します。

## Project 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **Project** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素の有効なテキスト値の詳細については、[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)に埋め込まれているドキュメントの注釈を参照してください。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Bb968475.note(ja-jp,office.12).gif" alt="Note" class="note" />メモ :</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>  <strong>OutlineCodes</strong>、<strong>WBSMasks</strong>、<strong>ExtendedAttributes</strong>、<strong>Calendars</strong>、<strong>Tasks</strong>、<strong>Resources</strong>、および <strong>Assignments</strong> 要素の構造の詳細については、このスキーマ リファレンスの個々のトピックを参照してください。</p></td>
</tr>
</tbody>
</table>


\<[Project](project-element.md)\>

    \<[SaveVersion](saveversion-element.md)\>**integer**\</SaveVersion\>

    \<[UID](uid-element.md) \>**string**\</UID\>

    \<[Name](name-element.md)\>**string**\</Name\>

    \<[Title](title-element-project.md)\>**string**\</Title\>

    \<[Subject](subject-element.md)\>**string**\</Subject\>

    \<[Category](category-element.md)\>**string**\</Category\>

    \<[Company](company-element.md)\>**string**\</Company\>

    \<[Manager](manager-element.md)\>**string**\</Manager\>

    \<[Author](author-element.md)\>**string**\</Author\>

    \<[CreationDate](creationdate-element.md)\>**dateTime**\</CreationDate\>

    \<[Revision](revision-element.md)\>**integer**\</Revision\>

    \<[LastSaved](lastsaved-element.md)\>**dateTime**\</LastSaved\>

    \<[ScheduleFromStart](schedulefromstart-element.md)\>**boolean**\</ScheduleFromStart\>

    \<[StartDate](startdate-element.md)\>**dateTime**\</StartDate\>

    \<[FinishDate](finishdate-element.md)\>**dateTime**\</FinishDate\>

    \<[FYStartDate](fystartdate-element.md)\>**integer**\</FYStartDate\>

    \<[CriticalSlackLimit](criticalslacklimit-element.md)\>**integer**\</CriticalSlackLimit\>

    \<[CurrencyDigits](currencydigits-element.md)\>**integer**\</CurrencyDigits\>

    \<[CurrencySymbol](currencysymbol-element.md)\>**string**\</CurrencySymbol\>

    \<[CurrencyCode](currencycode-element.md) \>**string**\</CurrencyCode\>

    \<[CurrencySymbolPosition](currencysymbolposition-element.md)\>**integer**\</CurrencySymbolPosition\>

    \<[CalendarUID](calendaruid-element.md)\>**integer**\</CalendarUID\>

    \<[DefaultStartTime](defaultstarttime-element.md)\>**time**\</DefaultStartTime\>

    \<[DefaultFinishTime](defaultfinishtime-element.md)\>**time**\</DefaultFinishTime\>

    \<[MinutesPerDay](minutesperday-element.md)\>**integer**\</MinutesPerDay\>

    \<[MinutesPerWeek](minutesperweek-element.md)\>**integer**\</MinutesPerWeek\>

    \<[DaysPerMonth](dayspermonth-element.md)\>**integer**\</DaysPerMonth\>

    \<[DefaultTaskType](defaulttasktype-element.md)\>**integer**\</DefaultTaskType\>

    \<[DefaultFixedCostAccrual](defaultfixedcostaccrual-element.md)\>**integer**\</DefaultFixedCostAccrual\>

    \<[DefaultStandardRate](defaultstandardrate-element.md)\>**float**\</DefaultStandardRate\>

    \<[DefaultOvertimeRate](defaultovertimerate-element.md)\>**float**\</DefaultOvertimeRate\>

    \<[DurationFormat](durationformat-element.md)\>**integer**\</DurationFormat\>

    \<[WorkFormat](workformat-element.md)\>**integer**\</WorkFormat\>

    \<[EditableActualCosts](editableactualcosts-element.md)\>**boolean**\</EditableActualCosts\>

    \<[HonorConstraints](honorconstraints-element.md)\>**boolean**\</HonorConstraints\>

    \<[EarnedValueMethod](earnedvaluemethod-element.md)\>**integer**\</EarnedValueMethod\>

    \<[InsertedProjectsLikeSummary](insertedprojectslikesummary-element.md)\>**boolean**\</InsertedProjectsLikeSummary\>

    \<[MultipleCriticalPaths](multiplecriticalpaths-element.md)\>**boolean**\</MultipleCriticalPaths\>

    \<[NewTasksEffortDriven](newtaskseffortdriven-element.md)\>**boolean**\</NewTasksEffortDriven\>

    \<[NewTasksEstimated](newtasksestimated-element.md)\>**boolean**\</NewTasksEstimated\>

    \<[SplitsInProgressTasks](splitsinprogresstasks-element.md)\>**boolean**\</SplitsInProgressTasks\>

    \<[SpreadActualCost](spreadactualcost-element.md)\>**boolean**\</SpreadActualCost\>

    \<[SpreadPercentComplete](spreadpercentcomplete-element.md)\>**boolean**\</SpreadPercentComplete\>

    \<[TaskUpdatesResource](taskupdatesresource-element.md)\>**boolean**\</TaskUpdatesResource\>

    \<[FiscalYearStart](fiscalyearstart-element.md)\>**boolean**\</FiscalYearStart\>

    \<[WeekStartDay](weekstartday-element.md)\>**integer**\</WeekStartDay\>

    \<[MoveCompletedEndsBack](movecompletedendsback-element.md)\>**boolean**\</MoveCompletedEndsBack\>

    \<[MoveRemainingStartsBack](moveremainingstartsback-element.md)\>**boolean**\</MoveRemainingStartsBack\>

    \<[MoveRemainingStartsForward](moveremainingstartsforward-element.md)\>**boolean**\</MoveRemainingStartsForward\>

    \<[MoveCompletedEndsForward](movecompletedendsforward-element.md)\>**boolean**\</MoveCompletedEndsForward\>

    \<[BaselineForEarnedValue](baselineforearnedvalue-element.md)\>**integer**\</BaselineForEarnedValue\>

    \<[AutoAddNewResourcesAndTasks](autoaddnewresourcesandtasks-element.md)\>**boolean**\</AutoAddNewResourcesAndTasks\>

    \<[StatusDate](statusdate-element.md)\>**dateTime**\</StatusDate\>

    \<[CurrentDate](currentdate-element.md)\>**dateTime**\</CurrentDate\>

    \<[MicrosoftProjectServerURL](microsoftprojectserverurl-element.md)\>**boolean**\</MicrosoftProjectServerURL\>

    \<[Autolink](autolink-element.md)\>**boolean**\</Autolink\>

    \<[NewTaskStartDate](newtaskstartdate-element.md)\>**integer**\</NewTaskStartDate\>

    \<[DefaultTaskEVMethod](defaulttaskevmethod-element.md)\>**integer**\</DefaultTaskEVMethod\>

    \<[ProjectExternallyEdited](projectexternallyedited-element.md)\>**boolean**\</ProjectExternallyEdited\>

    \<[ExtendedCreationDate](extendedcreationdate-element.md)\>**dateTime**\</ExtendedCreationDate\>

    \<[ActualsInSync](actualsinsync-element.md)\>**boolean**\</ActualsInSync\>

    \<[RemoveFileProperties](removefileproperties-element.md)\>**boolean**\</RemoveFileProperties\>

    \<[AdminProject](adminproject-element.md)\>**boolean**\</AdminProject\>

    \<[OutlineCodes](outlinecode-elements-and-xml-structure.md)\> . . . \</OutlineCodes\>

    \<[WBSMasks](wbsmask-elements-and-xml-structure.md)\> . . . \</WBSMasks\>

    \<[ExtendedAttributes](extendedattribute-elements-and-xml-structure.md)...\</ExtendedAttributes\>

    \<[Calendars](calendar-elements-and-xml-structure.md)\> . . . \</Calendars\>

    \<[Tasks](task-elements-and-xml-structure.md)\> . . . \</Tasks\>

    \<[Resources](resource-elements-and-xml-structure.md)\> . . . \</Resources\>

    \<[Assignments](assignment-elements-and-xml-structure.md)\> . . . \</Assignments\>

\</Project\>

## 参照

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)

