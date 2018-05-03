---
title: Assignment 要素と XML データ構造
TOCTitle: Assignment 要素と XML データ構造
ms:assetid: f74cca91-ea2a-478d-b935-528b25dddaa8
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968738(v=office.12)
ms:contentKeyID: 16750797
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Assignment 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **Assignments** 要素の子について説明します。これらの要素は、プロジェクトを XML 形式で保存するときの割り当てデータを表します。

**Assignments** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## Assignment 要素の XML データ構造

以下に、mspdi\_pj12.xsd の **Assignment** スキーマ セクションで定義されている要素の XML データ構造を示します。データ型は、テキスト値を必要とする要素として示されています。埋め込まれるドキュメント注釈ごとの有効なテキスト値の詳細については、「[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)」で確認できます。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

**Assignment** 要素の多くは、Microsoft Office Project Professional 2007 のデータ フィールドを表します。Project Professional 2007 および Project Standard 2007 のフィールドの詳細については、「[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)」を参照してください。

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
<td><p>   <strong>TimephasedData</strong> 要素のデータ構造の詳細については、このスキーマ リファレンスの「TimephasedDataType 要素と XML データ構造」を参照してください。</p></td>
</tr>
</tbody>
</table>


\<[Assignments](assignments-element.md)\>

    \<[Assignment](assignment-element.md)\>

        \<[UID](uid-element.md)\>**integer**\</UID\>

        \<[TaskUID](taskuid-element.md)\>**integer**\</TaskUID\>

        \<[ResourceUID](resourceuid-element.md)\>**integer**\</ResourceUID\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>**integer**\</PercentWorkComplete\>

        \<[ActualCost](actualcost-element.md)\>**decimal**\</ActualCost\>

        \<[ActualFinish](actualfinish-element.md)\>**dateTime**\</ActualFinish\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>**decimal**\</ActualOvertimeCost\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>**duration**\</ActualOvertimeWork\>

        \<[ActualStart](actualstart-element.md)\>**dateTime**\</ActualStart\>

        \<[ActualWork](actualwork-element.md)\>**duration**\</ActualWork\>

        \<[ACWP](acwp-element.md)\>**float**\</ACWP\>

        \<[Confirmed](confirmed-element.md)\>**boolean**\</Confirmed\>

        \<[Cost](cost-element.md)\>**decimal**\</Cost\>

        \<[CostRateTable](costratetable-element.md)\>**integer**\</CostRateTable\>

        \<[CostVariance](costvariance-element.md)\>**float**\</CostVariance\>

        \<[CV](cv-element.md)\>**float**\</CV\>

        \<[Delay](delay-element.md)\>**integer**\</Delay\>

        \<[Finish](finish-element.md)\>**dateTime**\</Finish\>

        \<[FinishVariance](finishvariance-element.md)\>**integer**\</FinishVariance\>

        \<[Hyperlink](hyperlink-element.md)\>**string**\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>**string**\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>**string**\</HyperlinkSubAddress\>

        \<[WorkVariance](workvariance-element.md)\>**float**\</WorkVariance\>

        \<[HasFixedRateUnits](hasfixedrateunits-element.md)\>**boolean**\</HasFixedRateUnits\>

        \<[FixedMaterial](fixedmaterial-element.md)\>**boolean**\</FixedMaterial\>

        \<[LevelingDelay](levelingdelay-element.md)\>**integer**\</LevelingDelay\>

        \<[LevelingDelayFormat](levelingdelayformat-element.md)\>**integer**\</LevelingDelayFormat\>

        \<[LinkedFields](linkedfields-element.md)\>**boolean**\</LinkedFields\>

        \<[Milestone](milestone-element.md)\>**boolean**\</Milestone\>

        \<[Notes](notes-element.md)\>**string**\</Notes\>

        \<[OverAllocated](overallocated-element.md)\>**boolean**\</Overallocated\>

        \<[OvertimeCost](overtimecost-element.md)\>**decimal**\</OvertimeCost\>

        \<[OvertimeWork](overtimework-element.md)\>**duration**\</OvertimeWork\>

        \<[PeakUnits](peakunits-element.md)\>**float**\</PeakUnits\>

        \<[RegularWork](regularwork-element.md)\>**duration**\</RegularWork\>

        \<[RemainingCost](remainingcost-element.md)\>**decimal**\</RemainingCost\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>**decimal**\</RemainingOvertimeCost\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>**duration**\</RemainingOvertimeWork\>

        \<[RemainingWork](remainingwork-element.md)\>**duration**\</RemainingWork\>

        \<[ResponsePending](responsepending-element.md)\>**boolean**\</ResponsePending\>

        \<[Start](start-element.md)\>**dateTime**\</Start\>

        \<[Stop](stop-element.md)\>**dateTime**\</Stop\>

        \<[Resume](resume-element.md)\>**dateTime**\</Resume\>

        \<[StartVariance](startvariance-element.md)\>**integer**\</StartVariance\>

        \<[Summary](summary-element.md)\>**boolean**\</Summary\>

        \<[SV](sv-element.md)\>**float**\</SV\>

        \<[Units](units-element.md)\>**float**\</Units\>

        \<[UpdateNeeded](updateneeded-element.md)\>**boolean**\</UpdateNeeded\>

        \<[VAC](vac-element.md)\>**float**\</VAC\>

        \<[Work](work-element.md)\>**duration**\</Work\>

        \<[WorkContour](workcontour-element.md)\>**integer**\</WorkContour\>

        \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

        \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

        \<[BookingType](bookingtype-element.md)\>**integer**\</BookingType\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>**duration**\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>**duration**\</ActualOvertimeWorkProtected\>

        \<[CreationDate](creationdate-element.md)\>**dateTime**\</CreationDate\>

        \<[AssnOwner](assnowner-element.md)\>**string**\</AssnOwner\>

        \<[AssnOwnerGuid](assnownerguid-element.md)\>**string**\</AssnOwnerGuid\>

        \<[BudgetCost](budgetcost-element.md)\>**decimal**\</BudgetCost\>

        \<[BudgetWork](budgetwork-element.md)\>**duration**\</BudgetWork\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[Value](value-element.md)\>**string**\</ValueID\>

            \<[ValueGUID](valueguid-element.md)\>**string**\</UID\>

            \<[DurationFormat](durationformat-element.md)\>**integer**\</ValueID\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            [\<TimephasedData\>](timephaseddatatype-elements-and-xml-structure.md)...\</TimephasedData\>        

            \<[Number](number-element.md)\>**string**\</Number\>

            \<[Start](start-element.md)\>**string**\</Start\>

            \<[Finish](finish-element.md)\>**string**\</Finish\>

            \<[Work](work-element.md)\>**duration**\</Work\>

            \<[Cost](cost-element.md)\>**string**\</Cost\>

            \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

            \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

        \</Baseline\>    

        \<\!-- \#\#新しい Project 2007 割り当てエンタープライズ ユーザー設定フィールド要素をここに示します。詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。--\>    

        \<f404000\>変数データ型\</f404000\>        \<\!-- 「[f404000 ～ f4040c8 要素](f404000-f4040c8-elements.md)」を参照 --\>

        . . .

        \<f4040c8\>変数データ型\</f4040c8\>

        \<f408000\>変数データ型\</f408000\>        \<\!-- 「[f408000 ～ f417fff 要素](f408000-f417fff-elements.md)」を参照 --\>

        . . .

        \<f417fff\>変数データ型\</f417fff\>

        \<[TimephasedData](timephaseddata-element.md)\>. . .\</TimephasedData\>

    \</Assignment\>

\</Assignments\>

## 参照

#### リファレンス

TimephasedDataType 要素と XML データ構造  

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)

