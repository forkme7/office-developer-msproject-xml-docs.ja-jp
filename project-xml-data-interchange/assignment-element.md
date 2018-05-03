---
title: Assignment 要素
TOCTitle: Assignment 要素
ms:assetid: 9e3ad85f-0226-4c99-8d3e-93c217f95308
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968611(v=office.12)
ms:contentKeyID: 16743322
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Assignment 要素

各 ** Assignments ** コレクションには、少なくとも 1 つの割り当てが必要です。

    <Assignment>
      ComplexTypeValue
    </Assignment>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="assignments-element.md">Assignments</a></p></td>
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
<td><p>割り当ての一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="taskuid-element.md">TaskUID</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの一意の ID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="resourceuid-element.md">ResourceUID</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>完了した割り当ての作業時間の割合を示す、割り当ての現在の進捗状況。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがタスクについて既に行った作業のコスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualfinish-element.md">ActualFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てを実際に完了した日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがタスクについて既に行った超過作業のコスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが割り当てタスクについて既に行った超過作業の実績時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualstart-element.md">ActualStart</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てを実際に開始した日時。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがタスクについて既に行った作業の時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの状況報告日または今日の日付までに、リソースがタスクについて既に行った作業のコスト。完了作業の実績コストとも呼ばれます。</p></td>
</tr>
<tr class="even">
<td><p><a href="confirmed-element.md">Confirmed</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てたリソースが、タスク割り当てを承諾しているか、却下しているかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての総予定 (予測) コスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="costratetable-element.md">CostRateTable</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てのリソースに使用するコスト単価表を示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="costvariance-element.md">CostVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての基準コストと総コストとの差額。</p></td>
</tr>
<tr class="even">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てについて現行の完了レベルに達するためにかかる予定であったコストと、実際にかかったコストとの差額。</p></td>
</tr>
<tr class="odd">
<td><p><a href="delay-element.md">Delay</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの開始日以降、割り当ての作業を開始するまでの、リソースの待機時間です。</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てられたリソースがタスクの作業を完了する予定の日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="finishvariance-element.md">FinishVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての基準終了日と予定終了日との差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関連するハイパーリンクのタイトルまたは説明テキスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関連するハイパーリンクのアドレス。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関連するハイパーリンク内のドキュメントの特定の位置。</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての基準作業時間と現在の予定作業時間との差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="hasfixedrateunits-element.md">HasFixedRateUnits</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての作業時間が固定であるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="fixedmaterial-element.md">FixedMaterial</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てられた数量単価型リソースの使用が、単一の固定量で発生するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="levelingdelay-element.md">LevelingDelay</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの平準化の結果、割り当てが予定開始日から遅延されることになる時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingdelayformat-element.md">LevelingDelayFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>延期の期間を表現する形式。</p></td>
</tr>
<tr class="even">
<td><p><a href="linkedfields-element.md">LinkedFields</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てへの OLE リンクがあるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="milestone-element.md">Milestone</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てタスクがマイルストーンであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関するメモ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated</a></p></td>
<td><p>オプション</p></td>
<td><p>特定のタスクについてリソースに割り当てられている作業量が、リソースが通常作業可能な量を超えているかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソース割り当ての超過作業の総コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースがタスクについて行い、リソースの超過単価で課金される、超過作業の時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="regularwork-element.md">RegularWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたリソースが行う予定の超過作業でない作業の総時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>オプション</p></td>
<td><p>特定のタスクの予定残存作業を、いずれかのリソースがすべて完了するためにかかるコスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての予定超過作業の残存コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てについて残っている超過作業の時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたリソースが割り当てを完了するためにかかる時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="responsepending-element.md">ResponsePending</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたリソースに送信した、リソースに割り当てを通知するメッセージに対して、回答を受信したかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てられたリソースがタスクの作業を開始する予定の日時。</p></td>
</tr>
<tr class="odd">
<td><p>Stop</p></td>
<td><p>オプション</p></td>
<td><p>割り当てを中断した日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="resume-element.md">Resume</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てを再開した日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="startvariance-element.md">StartVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての基準開始日と現在の予定開始日との差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="summary-element.md">Summary</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。サマリー タスクへの割り当てであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="sv-element.md">SV</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの状況報告日を通じた、達成額スケジュールの差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="units-element.md">Units</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクにリソースを割り当てる単位数を、パーセントで表したもの。</p></td>
</tr>
<tr class="odd">
<td><p><a href="updateneeded-element.md">UpdateNeeded</a></p></td>
<td><p>オプション</p></td>
<td><p>開始日、終了日、またはリソース割り当てが変更されたため、タスクに割り当てられたリソースにタスクの更新依頼を送信する必要があるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="vac-element.md">VAC</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクへの割り当ての基準コストと総コストとの完了時における差異 (VAC)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクについてリソースが行う予定の作業の総時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="workcontour-element.md">WorkContour</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての作業時間を、割り当ての期間内でどのように配分するかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての予定作業時間の予算コスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てについて現在までに行われた作業の予算コスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bookingtype-element.md">BookingType</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当ての予約の種類 (本予約または仮予約) を指定します。</p></td>
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
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てを作成した日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="assnowner-element.md">AssnOwner</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。割り当て所有者の名前です。</p></td>
</tr>
<tr class="even">
<td><p><a href="assnownerguid-element.md">AssnOwnerGuid</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。割り当て所有者の GUID です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="budgetcost-element.md">BudgetCost</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。この割り当てのコスト型リソースに対する予算コスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="budgetwork-element.md">BudgetWork</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。この割り当ての時間単価型リソースまたは数量単価型リソースに対する予算作業量。</p></td>
</tr>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>オプション</p></td>
<td><p>拡張属性の値 (ユーザー設定フィールド)。</p></td>
</tr>
<tr class="even">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関連付けられた基準値のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="f404000-f4040c8-elements.md">f404000 ～ f4040c8 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。割り当てレベルのローカル ユーザー設定フィールドの値です。</p></td>
</tr>
<tr class="even">
<td><p><a href="f408000-f417fff-elements.md">f408000 ～ f417fff 要素</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 で新たに加わった要素。割り当てレベルのエンタープライズ ユーザー設定フィールドの値です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てに関する、時間の経過と共に変化する情報。</p></td>
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

[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)

