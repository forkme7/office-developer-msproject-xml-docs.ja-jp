---
title: Resource 要素と XML データ構造
TOCTitle: Resource 要素と XML データ構造
ms:assetid: 26f69c99-50e8-49c5-80cf-1c81c0abefbd
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968445(v=office.12)
ms:contentKeyID: 16733598
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Resource 要素と XML データ構造

このセクションでは、Microsoft Office Project 2007 XML データ交換スキーマ (mspdi\_pj12.xsd) で定義されている **Resources** 要素の子について説明します。この XML 要素は、プロジェクトを XML 形式で保存するときのリソース データを表します。

**Resources** は **Project** 要素の子です。詳細については、「[Project 要素と XML データ構造](project-elements-and-xml-structure.md)」を参照してください。

## Resource 要素の XML データ構造

mspdi\_pj12.xsd の **Resource** スキーマ セクションで定義されている要素の XML データ構造を以下に示します。データ型は、テキスト値を必要とする要素として示されています。各要素の有効なテキスト値の詳細については、[Resource スキーマ](xml-schema-for-the-resources-element.md)に埋め込まれているドキュメントの注釈を参照してください。

Project 2007 XML データ交換スキーマで使用されるデータ型の詳細については、「[Project XML データの概要](introduction-to-project-xml-data.md)」を参照してください。

**Resource** 要素の多くは、Microsoft Office Project のデータ フィールドを表します。Project Professional 2007 と Project Standard 2007 のフィールドの詳細については、「[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)」を参照してください。

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


\<[Resources](resources-element.md)\>

    \<[Resource](resource-element.md)\>

        \<[UID](uid-element.md)\>**integer**\</UID\>

        \<[ID](id-element.md)\>**integer**\</ID\>

        \<[Name](name-element.md)\>**string**\</Name\>

        \<[Type](type-element-multiple-parents.md)\>**integer**\</Type\>

        \<[IsNull](isnull-element.md)\>**boolean**\</IsNull\>

        \<[Initials](initials-element.md)\>**string**\</Initials\>

        \<[Phonetics](phonetics-element.md)\>**string**\</Phonetics\>

        \<[NTAccount](ntaccount-element.md)\>**string**\</NTAccount\>

        \<[MaterialLabel](materiallabel-element.md)\>**string**\</MaterialLabel\>

        \<[Code](code-element.md)\>**string**\</Code\>

        \<[Group](group-element.md)\>**string**\</Group\>

        \<[WorkGroup](workgroup-element.md)\>**integer**\</WorkGroup\>

        \<[EmailAddress](emailaddress-element.md)\>**string**\</EmailAddress\>

        \<[Hyperlink](hyperlink-element.md)\>**string**\</Hyperlink\>

        \<[HyperlinkAddress](hyperlinkaddress-element.md)\>**string**\</HyperlinkAddress\>

        \<[HyperlinkSubAddress](hyperlinksubaddress-element.md)\>**string**\</HyperlinkSubAddress\>

        \<[MaxUnits](maxunits-element.md)\>**float**\</MaxUnits\>

        \<[PeakUnits](peakunits-element.md)\>**float**\</PeakUnits\>

        \<[OverAllocated](overallocated-element.md)\>**boolean**\</OverAllocated\>

        \<[AvailableFrom](availablefrom-element.md)\>**dateTime**\</AvailableFrom\>

        \<[AvailableTo](availableto-element.md)\>**dateTime**\</AvailableTo\>

        \<[Start](start-element.md)\>**dateTime**\</Start\>

        \<[Finish](finish-element.md)\>**dateTime**\</Finish\>

        \<[CanLevel](canlevel-element.md)\>**boolean**\</CanLevel\>

        \<[AccrueAt](accrueat-element.md)\>**integer**\</AccrueAt\>

        \<[Work](work-element.md)\>**duration**\</Work\>

        \<[RegularWork](regularwork-element.md)\>**duration**\</RegularWork\>

        \<[OvertimeWork](overtimework-element.md)\>**duration**\</OvertimeWork\>

        \<[ActualWork](actualwork-element.md)\>**duration**\</ActualWork\>

        \<[RemainingWork](remainingwork-element.md)\>**duration**\</RemainingWork\>

        \<[ActualOvertimeWork](actualovertimework-element.md)\>**duration**\</ActualOvertimeWork\>

        \<[RemainingOvertimeWork](remainingovertimework-element.md)\>**duration**\</RemainingOvertimeWork\>

        \<[PercentWorkComplete](percentworkcomplete-element.md)\>**integer**\</PercentWorkComplete\>

        \<[StandardRate](standardrate-element.md)\>**decimal**\</StandardRate\>

        \<[StandardRateFormat](standardrateformat-element.md)\>**integer**\</StandardRateFormat\>

        \<[Cost](cost-element.md)\>**decimal**\</Cost\>

        \<[OvertimeRate](overtimerate-element.md)\>**decimal**\</OvertimeRate\>

        \<[OvertimeRateFormat](overtimerateformat-element.md)\>**integer**\</OvertimeRateFormat\>

        \<[OvertimeCost](overtimecost-element.md)\>**decimal**\</OvertimeCost\>

        \<[CostPerUse](costperuse-element.md)\>**decimal**\</CostPerUse\>

        \<[ActualCost](actualcost-element.md)\>**decimal**\</ActualCost\>

        \<[ActualOvertimeCost](actualovertimecost-element.md)\>**decimal**\</ActualOvertimeCost\>

        \<[RemainingCost](remainingcost-element.md)\>**decimal**\</RemainingCost\>

        \<[RemainingOvertimeCost](remainingovertimecost-element.md)\>**decimal**\</RemainingOvertimeCost\>

        \<[WorkVariance](workvariance-element.md)\>**float**\</WorkVariance\>

        \<[CostVariance](costvariance-element.md)\>**float**\</CostVariance\>

        \<[SV](sv-element.md)\>**float**\</SV\>

        \<[CV](cv-element.md)\>**float**\</CV\>

        \<[ACWP](acwp-element.md)\>**float**\</ACWP\>

        \<[CalendarUID](calendaruid-element.md)\>**integer**\</CalendarUID\>

        \<[Notes](notes-element.md)\>**string**\</Notes\>

        \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

        \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

        \<[IsGeneric](isgeneric-element.md)\>**boolean**\</IsGeneric\>

        \<[IsInactive](isinactive-element.md)\>**boolean**\</IsInactive\>

        \<[IsEnterprise](isenterprise-element.md)\>**boolean**\</IsEnterprise\>

        \<[BookingType](bookingtype-element.md)\>**integer**\</BookingType\>

        \<[ActualWorkProtected](actualworkprotected-element.md)\>**duration**\</ActualWorkProtected\>

        \<[ActualOvertimeWorkProtected](actualovertimeworkprotected-element.md)\>**duration**\</ActualOvertimeWorkProtected\>

        \<[ActiveDirectoryGUID](activedirectoryguid-element.md)\>**string**\</ActiveDirectoryGUID\>

        \<[CreationDate](creationdate-element.md)\>**dateTime**\</CreationDate\>

        \<[ExtendedAttribute](extendedattribute-element.md)\>

            \<[UID](uid-element.md)\>**integer**\</UID\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[Value](value-element.md)\>**string**\</Value\>

            \<[ValueID](valueid-element.md)\>**integer**\</ValueID\>

            \<[DurationFormat](durationformat-element.md)\>**integer**\</DurationFormat\>

        \</ExtendedAttribute\>

        \<[Baseline](baseline-element.md)\>

            \<[Number](number-element.md)\>**integer**\</Number\>

            \<[Work](work-element.md)\>**duration**\</Work\>

            \<[Cost](cost-element.md)\>**float**\</Cost\>

            \<[BCWS](bcws-element.md)\>**float**\</BCWS\>

            \<[BCWP](bcwp-element.md)\>**float**\</BCWP\>

        \</Baseline\>

        \<[OutlineCode](outlinecode-element.md)\>

            \<[UID](uid-element.md)\>**integer**\</UID\>

            \<[FieldID](fieldid-element.md)\>**string**\</FieldID\>

            \<[ValueID](valueid-element.md)\>**integer**\</ValueID\>

        \</OutlineCode\>

        \<[IsCostResource](iscostresource-element.md)\>**boolean**\</IsCostResource\>

        \<[AssnOwner](assnowner-element.md)\>**string**\</AssnOwner\>

        \<[AssnOwnerGuid](assnownerguid-element.md)\>**string**\</AssnOwnerGuid\>

        \<[IsBudget](isbudget-element.md)\>**boolean**\</IsBudget\>

        \<[AvailabilityPeriods](availabilityperiods-element.md)\>

            \<[AvailabilityPeriod](availabilityperiod-element.md)\>

                \<[AvailableFrom](availablefrom-element.md)\>**dateTime**\</AvailableFrom\>

                \<[AvailableTo](availableto-element.md)\>**dateTime**\</AvailableTo\>

                \<[AvailableUnits](availableunits-element.md)\>**float**\</AvailableUnits\>

            \</AvailabilityPeriod\>

        \</AvailablilityPeriods\>

        \<[Rates](rates-element.md)\>

            \<[Rate](rate-element.md)\>

                \<[RatesFrom](ratesfrom-element.md)\>**dateTime**\</RatesFrom\>

                \<[RatesTo](ratesto-element.md)\>**dateTime**\</RatesTo\>

                \<[RateTable](ratetable-element.md)\>**integer**\</RateTable\>

                \<[StandardRate](standardrate-element.md)\>**decimal**\</StandardRate\>

                \<[StandardRateFormat](standardrateformat-element.md)\>**integer**\</StandardRateFormat\>

                \<[OvertimeRate](overtimerate-element.md)\>**decimal**\</OvertimeRate\>

                \<[OvertimeRateFormat](overtimerateformat-element.md)\>**integer**\</OvertimeRateFormat\>

                \<[CostPerUse](costperuse-element.md)\>**decimal**\</CostPerUse\>

            \</Rate\>

        \</Rates\>

        \<[c408000 ～ c417fff](c408000-c417fff-elements.md)\>

                \<\!-- \#\#新しい Project 2007 のエンタープライズ リソース ユーザー設定フィールドのデータ。

                                詳細については、「[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)」を参照してください。--\>

        \</c408000 ～ c417fff\>

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

    \</Resource\>

\</Resources\>

## 参照

#### リファレンス

TimephasedDataType 要素と XML データ構造  

#### その他の技術情報

[Project XML データの概要](introduction-to-project-xml-data.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[XML のユーザー設定フィールド データ](custom-field-data-in-xml.md)  
[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[フィールド リファレンス](http://office.microsoft.com/ja-jp/project/ch100788901041.aspx)

