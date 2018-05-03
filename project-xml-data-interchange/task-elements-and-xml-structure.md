---
title: Task 要素と XML データ構造
TOCTitle: Task 要素と XML データ構造
ms:assetid: 3fa5904f-841c-421b-bfdd-cb9531c8bdf7
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968475(v=office.12)
ms:contentKeyID: 16735621
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Task 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **Tasks** 要素の子について説明します。この要素は、プロジェクトを XML 形式で保存するときのタスク データを表します。

**Tasks** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## Task 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **Task** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。各要素の有効なテキスト値の詳細については、「[Task スキーマ](xml-schema-for-the-tasks-element.md)」に埋め込まれているドキュメント注釈を参照してください。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

**Task** 要素の多くは、Microsoft Office Project のデータ フィールドを表します。Project Professional 2007 と Project Standard 2007 のフィールドの詳細については、「[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)」を参照してください。

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
<td><p><strong>TimephasedData</strong> 要素のデータ構造の詳細については、このスキーマ リファレンスの「TimephasedDataType 要素と XML データ構造」を参照してください。</p></td>
</tr>
</tbody>
</table>


\<[Tasks](tasks-element.md)\>

    \<[Task](task-element.md)\>

        \<[UID](uid-element.md)\>**integer**\</UID\>

        \<[ID](id-element.md)\>**integer**\</ID\>

        \<[Name](name-element.md)\>**string**\</Name\>

        \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

        \<[IsNull](isnull-element.md)\>**boolean**\<IsNull\>

        \<[CreateDate](createdate-element.md)\>**dateTime**\</CreateDate\>

        \<[Contact](contact-element.md)\>**string**\</Contact\>

        \<[WBS](wbs-element.md)\>**string**\</WBS\>

        \<[WBSLevel](wbslevel-element.md)\>**string**\<WBSLevel\>

        \<[OutlineNumber](outlinenumber-element.md)\>**string**\</OutlineNumber\>

        \<[OutlineLevel](outlinelevel-element.md)\>**integer**\</OutlineLevel\>

        \<[Priority](priority-element.md)\>**integer**\</Priority\>

        \<[Start](start-element.md)\>**dateTime**\</Start\>

        \<[Finish](finish-element.md)\>**dateTime**\</Finish\>

        \<[Duration](duration-element.md)\>**duration**\</Duration\>

        \<[DurationFormat](durationformat-element.md)\>**integer**\</DurationFormat\>

        \<[Work](work-element.md)\>**duration**\</Work\>

        \<[Stop](stop-element.md)\>**dateTime**\</Stop\>

        \<[Resume](resume-element.md)\>**dateTime**\</Resume\>

        \<[ResumeValid](resumevalid-element.md)\>**boolean**\</ResumeValid\>

        \<[EffortDriven](effortdriven-element.md)\>**boolean**\</EffortDriven\>

        \<[Recurring](recurring-element.md)\>**boolean**\</Recurring\>

        \<[OverAllocated](overallocated-element.md)\>**boolean**\</OverAllocated\>

        \<[Estimated](estimated-element.md)\>**boolean**\</Estimated\>

        \<[Milestone](milestone-element.md)\>**boolean**\</Milestone\>

        \<[Summary](summary-element.md)\>**boolean**\</Summary\>

        \<[Critical](critical-element.md)\>**boolean**\</Critical\>

        \<[IsSubproject](issubproject-element.md)\>**boolean**\</IsSubproject\>

        \<[IsSubprojectReadOnly](issubprojectreadonly-element.md)\>**boolean**\</IsSubprojectReadOnly\>

        \<[SubprojectName](subprojectname-element.md)\>**string**\</SubprojectName\>

        \<[ExternalTask](externaltask-element.md)\>**boolean**\</ExternalTask\>

        \<[ExternalTaskProject](externaltaskproject-element.md)\>**string**\</ExternalTaskProject\>

        \<[EarlyStart](earlystart-element.md)\>**dateTime**\</EarlyStart\>

        \<[EarlyFinish](earlyfinish-element.md)\>**dateTime**\</EarlyFinish\>

        \<[LateStart](latestart-element.md)\>**dateTime**\</LateStart\>

        \<[LateFinish](latefinish-element.md)\>**dateTime**\</LateFinish\>

        \<[StartVariance](startvariance-element.md)\>**integer**\</StartVariance\>

        \<[FinishVariance](finishvariance-element.md)\>**integer**\</FinishVariance\>

        \<[WorkVariance](workvariance-element.md)\>**float**\</WorkVariance\>

        \<[FreeSlack](freeslack-element.md)\>**integer**\</FreeSlack\>

        \<[TotalSlack](totalslack-element.md)\>**integer**\</TotalSlack\>

        \<[FixedCost](fixedcost-element-baseline.md)\>**float**\</FixedCost\>

        \<[FixedCostAccrual](fixedcostaccrual-element.md)\>**string**\</FixedCostAccrual\>

        \<[PercentComplete](percentcomplete-element.md)\>**integer**\</PercentComplete\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>**integer**\</PercentWorkComplete\>

        \<[Cost](cost-element.md)\>**decimal**\</Cost\>

        \<[OvertimeCost](overtimecost-element.md)\>**decimal**\</OvertimeCost\>

        \<[OvertimeWork](overtimework-element.md)\>**duration**\</OvertimeWork\>

        \<[ActualStart](actualstart-element.md)\>**dateTime**\<ActualStart\>

        \<[ActualFinish](actualfinish-element.md)\>**dateTime**\</ActualFinish\>

        \<[ActualDuration](actualduration-element.md)\>**duration**\</ActualDuration\>

        \<[ActualCost](actualcost-element.md)\>**decimal**\</ActualCost\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>**decimal**\</ActualOvertimeCost\>

        \<[ActualWork](actualwork-element.md)\>**duration**\</ActualWork\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>**duration**\</ActualOvertimeWork\>

        \<[RegularWork](regularwork-element.md)\>**duration**\</RegularWork\>

        \<[RemainingDuration](remainingduration-element.md)\>**duration**\</RemainingDuration\>

        \<[RemainingCost](remainingcost-element.md)\>**decimal**\</RemainingCost\>

        \<[RemainingWork](remainingwork-element.md)\>**duration**\</RemainingWork\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>**decimal**\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>**duration**\</RemainingOvertimeWork\>

        \<[ACWP](acwp-element.md)\>**float**\</ACWP\>

        \<[CV](cv-element.md)\>**float**\</CV\>

        \<[ConstraintType](constrainttype-element.md)\>**integer**\</ConstraintType\>

        \<[CalendarUID](calendaruid-element.md)\>**integer**\</CalendarUID\>

        \<[ConstraintDate](constraintdate-element.md)\>**dateTime**\</ConstraintDate\>

        \<[Deadline](deadline-element.md)\>**dateTime**\</Deadline\>

        \<[LevelAssignments](levelassignments-element.md)\>**boolean**\</LevelAssignments\>

        \<[LevelingCanSplit](levelingcansplit-element.md)\>**boolean**\</LevelingCanSplit\>

        \<[LevelingDelay](levelingdelay-element.md)\>**integer**\</LevelingDelay\>

        \<[LevelingDelayFormat](levelingdelayformat-element.md)\>**integer**\</LevelingDelayFormat\>

        \<[PreLeveledStart](preleveledstart-element.md)\>**dateTime**\</PreLeveledStart\>

        \<[PreLeveledFinish](preleveledfinish-element.md)\>**dateTime**\</PreLeveledFinish\>

        \<[Hyperlink](hyperlink-element.md)\>**string**\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>**string**\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>**string**\</HyperlinkSubAddress\>

        \<[IgnoreResourceCalendar](ignoreresourcecalendar-element.md)\>**boolean**\</IgnoreResourceCalendar\>

        \<[Notes](notes-element.md)\>**string**\</Notes\>

        \<[HideBar](hidebar-element.md)\>**boolean**\</HideBar\>

        \<[Rollup](rollup-element.md)\>**boolean**\</Rollup\>

        \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

        \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

        \<[PhysicalPercentComplete](physicalpercentcomplete-element.md)\>**integer**\</PhysicalPercentComplete\>

        \<[EarnedValueMethod](earnedvaluemethod-element.md)\>**integer**\</EarnedValueMethod\>

        \<[PredecessorLink](predecessorlink-element.md)\>

            \<[PredecessorUID](predecessoruid-element.md)\>**integer**\</PredecessorUID\>

            \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

            \<[CrossProject](crossproject-element.md)\>**boolean**\</CrossProject\>

            \<[CrossProjectName](crossprojectname-element.md)\>**string**\</CrossProjectName\>

            \<[LinkLag](linklag-element.md)\>**integer**\</LinkLag\>

            \<[LagFormat](lagformat-element.md)\>**integer**\</LagFormat\>

        \</PredecessorLink\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>**duration**\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>**duration**\</ActualOvertimeWorkProtected\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[UID](uid-element.md)\>**integer**\</UID\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[Value](value-element.md)\>**string**\</Value\>

            \<[ValueID](valueid-element.md)\>**integer**\</ValueID\>

            \<[DurationFormat](durationformat-element.md)\>**integer**\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            [\<TimephasedData\>](timephaseddatatype-elements-and-xml-structure.md)...\</TimephasedData\>

            \<[Number](number-element.md)\>**integer**\</Number\>

            \<[Interim](interim-element.md)\>**boolean**\</Interim\>

            \<[Start](start-element.md)\>**dateTime**\</Start\>

            \<[Finish](finish-element.md)\>**dateTime**\</Finish\>

            \<[Duration](duration-element.md)\>**duration**\</Duration\>

            \<[DurationFormat](durationformat-element.md)\>**integer**\</DurationFormat\>

            \<[EstimatedDuration](estimatedduration-element.md)\>**boolean**\</EstimatedDuration\>

            \<[Work](work-element.md)\>**duration**\</Work\>

            \<[Cost](cost-element.md)\>**decimal**\</Cost\>

            \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

            \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

            \<[FixedCost](fixedcost-element-baseline.md)\>**float**\</FixedCost\>

        \</Baseline\>

        \<[IsPublished](ispublished-element.md)\>**boolean**\</IsPublished\>

        \<[StatusManager](statusmanager-element.md)\>**string**\</StatusManager\>

        \<[CommitmentStart](commitmentstart-element.md)\>**dateTime**\</CommitmentStart\>

        \<[CommitmentFinish](commitmentfinish-element.md)\>**dateTime**\</CommitmentFinish\>

        \<[CommitmentType](commitmenttype-element.md)\>**integer**\</CommitmentType\>

        \<[b408000 ～ b417fff](b408000-b417fff-elements.md)\>

                \<\!-- \#\#新しい Project 2007 エンタープライズ タスク ユーザー設定フィールド データ。

                        詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。--\>

        \</b408000 ～ b417fff\>

        \<[b608000 ～ b617fff](b608000-b617fff-elements.md)\>

                \<\!-- \#\#新しい Project 2007 エンタープライズ プロジェクト ユーザー設定フィールド データ。--\>

        \</b608000 ～ b617fff\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[Value](value-element.md)\>**string**\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>**string**\</UID\>

            \<[DurationFormat](durationformat-element.md)\>**integer**\</ValueID\>

        \</ExtendedAttribute\>

        \<[OutlineCode](outlinecode-element.md)\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[ValueID](valueid-element.md)\>**integer**\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>**string**\</UID\>

        \</OutlineCode\>

        \<[TimephasedData](timephaseddata-element.md)\>. . .\</TimephasedData\>

    \</Task\>

\</Tasks\>

## 参照

#### リファレンス

TimephasedDataType 要素と XML データ構造  

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)

