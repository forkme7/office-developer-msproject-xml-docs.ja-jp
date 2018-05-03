---
title: Resource 要素
TOCTitle: Resource 要素
ms:assetid: e67f9a03-2869-431d-8d48-353e3e15a896
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968715(v=office.12)
ms:contentKeyID: 16749401
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Resource 要素

プロジェクトのリソースです。各 **Resources** コレクションには少なくとも 1 つのリソースが存在する必要があります。

    <Resource>
      ComplexTypeValue
    </Resource>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="resources-element.md">Resources</a></p></td>
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
<td><p><a href="uid-element.md">UID 要素</a></p></td>
<td><p>必須</p></td>
<td><p>リソースの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="id-element.md">ID 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースのリスト内のリソースの位置を示す識別子。</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの名前。リソースがアクティブであるかどうかに関係なく、エンタープライズ内で一意である必要があります。</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの種類 (時間単価型または数量単価型)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="isnull-element.md">IsNull 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが null リソースであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="initials-element.md">Initials 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソース名の頭文字です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="phonetics-element.md">Phonetics 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソース名のふりがな情報をひらがなとカタカナのいずれかで格納します。Microsoft Office Project の日本語版のみで使用します。</p></td>
</tr>
<tr class="even">
<td><p><a href="ntaccount-element.md">NTAccount 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの Microsoft Windows NT Account 名。</p></td>
</tr>
<tr class="odd">
<td><p><a href="materiallabel-element.md">MaterialLabel 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>数量単価型リソースに対して入力される、トン、箱数、立方ヤードなどの測定単位。</p></td>
</tr>
<tr class="even">
<td><p><a href="code-element.md">Code 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの情報の一部として入力されたコード、省略形、または数値。</p></td>
</tr>
<tr class="odd">
<td><p><a href="group-element.md">Group 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが属するグループの名前。</p></td>
</tr>
<tr class="even">
<td><p><a href="workgroup-element.md">WorkGroup 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクト チームとの通信に使用されるメッセージ方式。</p></td>
</tr>
<tr class="odd">
<td><p><a href="emailaddress-element.md">EmailAddress 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの電子メール アドレス。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースと関連付けられたハイパーリンクのタイトルまたは説明テキスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースと関連付けられたハイパーリンクのアドレス。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースと関連付けられたハイパーリンク内のドキュメントの特定の位置。</p></td>
</tr>
<tr class="odd">
<td><p><a href="maxunits-element.md">MaxUnits 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクを実行するために現在の期間内にリソースを利用できる最大作業可能時間を表す、パーセントまたは単位数の最大値。</p></td>
</tr>
<tr class="even">
<td><p><a href="peakunits-element.md">PeakUnits 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられたすべてのタスクに対して、一度にリソースを割り当てることのできる最大使用率または最大使用数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての割り当てタスクでリソースの通常作業可能な量よりも多くの作業がリソースに割り当てられているかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="availablefrom-element.md">AvailableFrom 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>現在の期間に指定されている単位数でリソースを作業に使用できる期間の開始日です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="availableto-element.md">AvailableTo 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>現在の期間に指定されている単位数で、リソースを作業に利用できる期間の終了日です。</p></td>
</tr>
<tr class="even">
<td><p><a href="start-element.md">Start 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがすべての割り当てタスクで作業の開始を予定している日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="finish-element.md">Finish 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがすべての割り当てタスクで作業の終了を予定している日時。</p></td>
</tr>
<tr class="even">
<td><p><a href="canlevel-element.md">CanLevel 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの平準化がリソースに実行可能かどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="accrueat-element.md">AccrueAt 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの標準コストと超過コストをタスクのコストに計上する方法と時期を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="work-element.md">Work 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての割り当てタスクでリソースが行うスケジュールされた作業時間の合計。</p></td>
</tr>
<tr class="odd">
<td><p><a href="regularwork-element.md">RegularWork 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられたすべての割り当てに対して計画された超過作業時間でない予定作業の合計時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられたすべてのタスクで発生した超過作業の合計、およびリソースの超過単価での課金。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられたすべての割り当てに対して既に行った実績作業時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがすべての割り当てタスクを完了するために依然として必要な時間または 1 人あたりの作業時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられたすべての割り当てに対して既に行った、実績超過作業時間の合計。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての割り当てタスクを完了するためにリソースで必要な残存超過作業時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>完了したリソースの作業時間の割合として表現される、リソースに割り当てられたすべてのタスクの現在の進捗状況。</p></td>
</tr>
<tr class="even">
<td><p><a href="standardrate-element.md">StandardRate</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが実行する通常の作業時間内の作業に対して支払われる単価です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="standardrateformat-element.md">StandardRateFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>標準単価を表示するために使用される単位。</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての残存作業時間の計画コストに加えて、リソースがすべての割り当てタスクで既に終了したコストを元にした、リソースの割り当てタスクすべての計画コストの合計。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimerate-element.md">OvertimeRate</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースによって実行される超過作業に対して支払われる時間単価です。</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimerateformat-element.md">OvertimeRateFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>超過時間料金の表示に使用される単位。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースのすべての割り当てタスクに対する超過コストの合計。</p></td>
</tr>
<tr class="even">
<td><p><a href="costperuse-element.md">CostPerUse</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが使用されるたびに発生するコスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがすべての割り当てタスクで既に行った、作業時間に対する発生コストの総額。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがすべての割り当てタスクで既に行った、超過作業時間に対する発生コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに割り当てられている残存作業を完了するために発生する残りの予定費用。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての割り当てタスクに予定されている残存超過作業をリソースが完了するために発生する、リソースに対して計画された残存超過作業の費用。</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの基準作業時間の合計と現在スケジュールされている作業時間の差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="costvariance-element.md">CostVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>基準コストとリソースの総コストとの差異。</p></td>
</tr>
<tr class="odd">
<td><p><a href="sv-element.md">SV</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日または今日の日付までの、現在の進捗状況と、リソースの割り当てタスクすべての基準計画とのコストの差異。達成額のスケジュールの差異とも呼ばれます。</p></td>
</tr>
<tr class="even">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>オプション</p></td>
<td><p>現行の完了レベルに達するためにリソースに対して必要なコストと、状況報告日または今日の日付までの期間で現行の完了レベルに達するために実際かかったコストとの差異。</p></td>
</tr>
<tr class="odd">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日または今日の日付までの、リソースの割り当てすべての終了した作業時間の実績コスト (ACWP) 値の合計。</p></td>
</tr>
<tr class="even">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>オプション</p></td>
<td><p>このリソースと関連づけられているカレンダーの一意の ID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに関するメモ。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての割り当てタスクに対するリソースの BCWS 値を重ね合わせたサマリー。予定作業時間とも呼ばれます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日または今日の日付までで計算された、すべての割り当てタスクに対するリソースの BCWP 値を重ね合わせたサマリー。実際作業時間とも呼ばれます。</p></td>
</tr>
<tr class="even">
<td><p><a href="isgeneric-element.md">IsGeneric</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがエンタープライズレベルの標準リソースであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="isinactive-element.md">IsInactive</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがアクティブ (有効) なユーザーであるか、または非アクティブなユーザーであるかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="isenterprise-element.md">IsEnterprise</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがエンタープライズ リソースであるかどうかを指定します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bookingtype-element.md">BookingType</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの予約の種類 (コミット済みの予約または提案された予約) を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualworkprotected-element.md">ActualWorkProtected</a></p></td>
<td><p>オプション</p></td>
<td><p>実績作業時間が保護される期間を指定します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimeworkprotected-element.md">ActualOvertimeWorkProtected</a></p></td>
<td><p>オプション</p></td>
<td><p>実績超過作業時間が保護される期間を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="activedirectoryguid-element.md">ActiveDirectoryGUID</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの Active Directory GUID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクト、リソース、または割り当てが作成された日付です。</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースと関連付けられているユーザー設定フィールド定義。</p></td>
</tr>
<tr class="odd">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>オプション</p></td>
<td><p>進捗管理目的に使用されるプロジェクト見積もりのセット。</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
<td><p>オプション</p></td>
<td><p>代替プロジェクト構造を有効にするリソースに対して定義されるカスタム タグ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="iscostresource-element.md">IsCostResource</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。リソースがコスト リソースであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="assnowner-element.md">AssnOwner</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。割り当て所有者の名前。</p></td>
</tr>
<tr class="odd">
<td><p><a href="assnownerguid-element.md">AssnOwnerGuid</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。割り当て所有者の GUID。</p></td>
</tr>
<tr class="even">
<td><p><a href="isbudget-element.md">IsBudget</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。リソースが予算リソースであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="availabilityperiods-element.md">AvailabilityPeriods</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが使用可能である日付のコレクション。</p></td>
</tr>
<tr class="even">
<td><p><a href="rates-element.md">Rates</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの支払い単価のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="c408000-c417fff-elements.md">c408000 ～ c417fff</a></p></td>
<td><p>オプション</p></td>
<td><p>エンタープライズ リソースのユーザー設定フィールド データ。</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>オプション</p></td>
<td><p>ローカル リソースのユーザー設定フィールド データ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースに関連付けられたタイムスケール データ ブロック。</p></td>
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


## 参照

#### その他の技術情報

[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)

