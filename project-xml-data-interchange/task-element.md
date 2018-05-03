---
title: Task 要素
TOCTitle: Task 要素
ms:assetid: 47e990dd-9bdc-4edc-b6e7-b1535afe1c6e
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968487(v=office.12)
ms:contentKeyID: 16736275
ms.date: 06/30/2008
mtps_version: v=office.12
dev_langs:
- xml
ms.translationtype: HT
---

# Task 要素

各 **Tasks** コレクションにはタスクが 1 つ以上なければなりません。

    <Task>
      ComplexTypeValue
    </Task>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="tasks-element.md">Tasks</a></p></td>
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
<td><p>タスクの一意の ID。</p></td>
</tr>
<tr class="even">
<td><p><a href="id-element.md">ID</a></p></td>
<td><p>オプション</p></td>
<td><p>タスク リストにおけるタスクの位置を示す ID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの名前です。</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの種類 (単位数固定、期間固定、または作業時間固定)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="isnull-element.md">IsNull</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが null であるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="createdate-element.md">CreateDate</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトにタスクが追加された日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="contact-element.md">Contact</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの担当者名。</p></td>
</tr>
<tr class="even">
<td><p><a href="wbs-element.md">WBS</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの階層構造における各タスクの位置を表す一意のコード (WBS)。</p></td>
</tr>
<tr class="odd">
<td><p><a href="wbslevel-element.md">WBSLevel</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの右端のレベル。たとえば、タスク WBS が A.01.03 の場合、右端のレベルは 03 です。</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinenumber-element.md">OutlineNumber</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクト アウトライン階層内のタスクのレベルを示す番号。</p></td>
</tr>
<tr class="odd">
<td><p><a href="outlinelevel-element.md">OutlineLevel</a></p></td>
<td><p>オプション</p></td>
<td><p>アウトライン内のタスクの正確な位置を示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="priority-element.md">Priority</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられた優先度を示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクを開始する予定の日時。</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクを終了する予定の日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="duration-element.md">Duration</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに対する作業時間の合計期間。</p></td>
</tr>
<tr class="even">
<td><p><a href="durationformat-element.md">DurationFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの期間を表す形式。</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたすべてのリソースが作業するように予定されている作業時間数の合計。</p></td>
</tr>
<tr class="even">
<td><p><a href="stop-element.md">Stop</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの実績期間の最後を示す日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="resume-element.md">Resume</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの残りの期間を再開するために予定されている日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="resumevalid-element.md">ResumeValid</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクを再開できるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="effortdriven-element.md">EffortDriven</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクのスケジュールが残存作業時間優先かどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="recurring-element.md">Recurring</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが定期タスクであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられているリソースに対して、通常の作業時間内に終了できる量を超える作業が割り当てられているかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="estimated-element.md">Estimated</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの期間が見積もりとしてフラグが設定されるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="milestone-element.md">Milestone</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクがマイルストーンであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="summary-element.md">Summary</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクがサマリー タスクであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="critical-element.md">Critical</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクのスケジュールに遅延できる余裕があるか、またはタスクがクリティカル パス上にあるかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="issubproject-element.md">IsSubproject</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが挿入プロジェクトであるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="issubprojectreadonly-element.md">IsSubprojectReadOnly</a></p></td>
<td><p>オプション</p></td>
<td><p>挿入プロジェクトが読み取り専用であるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="subprojectname-element.md">SubprojectName</a></p></td>
<td><p>オプション</p></td>
<td><p>挿入プロジェクトのソースの位置。</p></td>
</tr>
<tr class="odd">
<td><p><a href="externaltask-element.md">ExternalTask</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが別のプロジェクトにリンクしているか、または現在のプロジェクトに基づいているかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="externaltaskproject-element.md">ExternalTaskProject</a></p></td>
<td><p>オプション</p></td>
<td><p>外部タスクのソース。</p></td>
</tr>
<tr class="odd">
<td><p><a href="earlystart-element.md">EarlyStart</a></p></td>
<td><p>オプション</p></td>
<td><p>最も早くタスクを開始できる日付です。この日付は、先行タスクと後続タスクの最早開始日と、その他の制約に基づいて算出されます。</p></td>
</tr>
<tr class="even">
<td><p><a href="earlyfinish-element.md">EarlyFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>最も早くタスクを終了できる日付です。この日付は、先行タスクと後続タスクの最早終了日、その他の制約、および平準化による延期期間に基づいて算出されます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="latestart-element.md">LateStart</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの終了日を遅らせずに最も遅くタスクを開始できる日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="latefinish-element.md">LateFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの終了日を遅らせずにタスクを終了できる最も遅い日付です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="startvariance-element.md">StartVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準開始日と現在の予定開始日との差。</p></td>
</tr>
<tr class="even">
<td><p><a href="finishvariance-element.md">FinishVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準終了日とタスクの現在の終了日との差を示す時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準作業時間と現在の予定作業時間との差。</p></td>
</tr>
<tr class="even">
<td><p><a href="freeslack-element.md">FreeSlack</a></p></td>
<td><p>オプション</p></td>
<td><p>後続タスクを遅らせずにタスクを延期できる期間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="totalslack-element.md">TotalSlack</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの終了日を遅らせずにタスクを延期できる期間です。</p></td>
</tr>
<tr class="even">
<td><p><a href="fixedcost-element-baseline.md">FixedCost</a></p></td>
<td><p>オプション</p></td>
<td><p>リソース コストに関連しないタスクのコスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="fixedcostaccrual-element.md">FixedCostAccrual</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクのコストに対する固定コストの支払方法 (計上方法) を示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="percentcomplete-element.md">PercentComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの期間のうち、現在までに完了した期間の割合を示すタスクの進捗状況。</p></td>
</tr>
<tr class="odd">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>現在までにタスクに費やした作業時間の割合を示すタスクの進捗状況。</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの予定コストまたは計画コストの総額。</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの実績超過コストの総額。</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てたすべてのリソースが、通常の作業時間を超えて作業する予定の時間数。リソースの超過作業時間に対する支払いには、超過単価が適用されます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualstart-element.md">ActualStart</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが実際に開始した日時。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualfinish-element.md">ActualFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクが実際に終了した日時。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualduration-element.md">ActualDuration</a></p></td>
<td><p>オプション</p></td>
<td><p>予定の期間と現在の残存作業時間、または達成率に基づく、現在までのタスクの実績作業時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられているすべてのリソースが実際に作業した時間に発生したコスト、およびタスクに関連して報告されたその他のコスト。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>あるタスクで、割り当てられたすべてのリソースが通常の作業時間を超えて実際に作業した時間に発生したコスト。</p></td>
</tr>
<tr class="even">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたリソースが、その割り当てタスクで実際に作業した時間数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたすべてのリソースが、通常の作業時間を超えて実際に作業した時間数。</p></td>
</tr>
<tr class="even">
<td><p><a href="regularwork-element.md">RegularWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたすべてのリソースが実行するように予定されている、通常の作業時間内の作業時間数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingduration-element.md">RemainingDuration</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたすべてのリソースが実行するように予定されている、通常の作業時間内の作業時間数。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>オプション</p></td>
<td><p>まだ完了していないタスクを終了するのに必要な期間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに割り当てられたすべてのリソースが残りの予定作業を完了するために発生する残りの予定費用。</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに予定されている残りの超過作業の費用。</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>オプション</p></td>
<td><p>割り当てられているすべてのリソースがタスクを完了するために予定されている残存超過時間。</p></td>
</tr>
<tr class="even">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクで実際に作業した時間に発生したコスト。プロジェクトの状況報告日または今日の日付までの値が計算されます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの現在までの完了作業に対して、かかるはずだった予定のコストと実際にかかったコストとの差異。</p></td>
</tr>
<tr class="even">
<td><p><a href="constrainttype-element.md">ConstraintType</a></p></td>
<td><p>オプション</p></td>
<td><p>予定タスクの開始日または終了日に対する制約。</p></td>
</tr>
<tr class="odd">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクト カレンダー内の有効な UID を参照します。</p></td>
</tr>
<tr class="even">
<td><p><a href="constraintdate-element.md">ConstraintDate</a></p></td>
<td><p>オプション</p></td>
<td><p><strong>ConstraintType</strong> で定義された制約に対応する開始日または終了日を示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="deadline-element.md">Deadline</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの期限として入力された日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="levelassignments-element.md">LevelAssignments</a></p></td>
<td><p>オプション</p></td>
<td><p>平準化機能は個々の割り当て (タスク全体ではなく) を遅延および分割することで、割り当て超過を解消できるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingcansplit-element.md">LevelingCanSplit</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの平準化機能を使って、タスクの残存作業時間を分割できるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="levelingdelay-element.md">LevelingDelay</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースの平準化によって、タスクが開始日から遅れる時間。</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingdelayformat-element.md">LevelingDelayFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>延期の期間を表す形式。</p></td>
</tr>
<tr class="even">
<td><p><a href="preleveledstart-element.md">PreLeveledStart</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが平準化される前のタスクの開始日。</p></td>
</tr>
<tr class="odd">
<td><p><a href="preleveledfinish-element.md">PreLeveledFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>リソースが平準化される前のタスクの終了日。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関連付けられたハイパーリンクの名前や表記。</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関連付けられたハイパーリンクのアドレス。</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関連付けられたハイパーリンクの文書内の位置。</p></td>
</tr>
<tr class="odd">
<td><p><a href="ignoreresourcecalendar-element.md">IgnoreResourceCalendar</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクのスケジュールでタスクに割り当てられているリソースのカレンダーを考慮するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関して入力されたメモ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="hidebar-element.md">HideBar</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクのガント バーとカレンダー バーを非表示にするかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="rollup-element.md">Rollup</a></p></td>
<td><p>オプション</p></td>
<td><p>ガント チャートのサマリー タスクにサブタスクの情報を重ね合わせて表示するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日または今日の日付までに累積されたタイムスケール領域の基準コスト。BCWS (Budgeted Cost of Work Scheduled) ともいいます。</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>オプション</p></td>
<td><p>タイムスケール領域のタスクの基準計画コストに、それぞれの達成率を掛けた累積値。状況報告日または今日の日付までの値が計算されます。BCWP (Budgeted Cost of Work Performed) ともいいます。</p></td>
</tr>
<tr class="odd">
<td><p><a href="physicalpercentcomplete-element.md">PhysicalPercentComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>完了したタスクの合計作業時間の実際の達成率。</p></td>
</tr>
<tr class="even">
<td><p><a href="earnedvaluemethod-element.md">EarnedValueMethod</a></p></td>
<td><p>オプション</p></td>
<td><p>使用する達成額の計算方法を示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="predecessorlink-element.md">PredecessorLink</a></p></td>
<td><p>オプション</p></td>
<td><p>現在のタスクの先行タスクを指定します。</p></td>
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
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクの基準計画の値のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="ispublished-element.md">IsPublished</a></p></td>
<td><p>オプション</p></td>
<td><p>Microsoft Office Project 2007 の新しい要素。タスクが発行されたかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="statusmanager-element.md">StatusManager</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。タスクの状況管理者名。</p></td>
</tr>
<tr class="odd">
<td><p><a href="commitmentstart-element.md">CommitmentStart</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。成果物の開始日。</p></td>
</tr>
<tr class="even">
<td><p><a href="commitmentfinish-element.md">CommitmentFinish</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。成果物の終了日。</p></td>
</tr>
<tr class="odd">
<td><p><a href="commitmenttype-element.md">CommitmentType</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。タスクに、関連付けられた成果物または関連付けられた成果物に対する依存関係があるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="b408000-b417fff-elements.md">b408000 ～ b417fff</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。タスクレベルのエンタープライズ ユーザー設定フィールドの値。</p></td>
</tr>
<tr class="odd">
<td><p><a href="b608000-b617fff-elements.md">b608000 ～ b617fff</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。プロジェクトレベルのエンタープライズ ユーザー設定フィールドの値。</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>オプション</p></td>
<td><p>タスク ユーザー設定フィールドの値を指定します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
<td><p>オプション</p></td>
<td><p>タスク アウトライン コードの値を指定します。</p></td>
</tr>
<tr class="even">
<td><p><a href="timephaseddata-element.md">TimephasedData.</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関連付けられたタイムスケール領域のデータ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクがサブプロジェクトの場合は、挿入サブプロジェクト データを指定します。</p></td>
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

次の例では、タスク **ID** は 3 ですが、タスク **UID** は 4 です。これは、タスク T3 が作成される前にタスクが削除されたからです。**UID** 値は、プロジェクト内で一意である必要があります。ユーザー設定の **WBSMask** が定義されていないので、タスクの **WBS** 値は、**OutlineNumber** と同じです。

``` xml
<Task>
   <UID>4</UID>
   <ID>3</ID>
   <Name>T3</Name>
   <Type>1</Type>
   <IsNull>0</IsNull>
   <CreateDate>2007-11-13T14:33:00</CreateDate>
   <WBS>1.2</WBS>
   <WBSLevel>2</WBSLevel>
   <OutlineNumber>1.2</OutlineNumber>
   <OutlineLevel>2</OutlineLevel>
   <Priority>500</Priority>
   <Start>2007-11-14T08:00:00</Start>
   <Finish>2007-11-15T17:00:00</Finish>
   <Duration>PT16H0M0S</Duration>
   <DurationFormat>53</DurationFormat>
   <Work>PT0H0M0S</Work>
   <ResumeValid>0</ResumeValid>
   <EffortDriven>0</EffortDriven>
   <Recurring>0</Recurring>
   <OverAllocated>0</OverAllocated>
   <Estimated>1</Estimated>
   <Milestone>0</Milestone>
   <Summary>1</Summary>
   <Critical>1</Critical>
   <IsSubproject>0</IsSubproject>
   <IsSubprojectReadOnly>0</IsSubprojectReadOnly>
   <ExternalTask>0</ExternalTask>
   <EarlyStart>2007-11-14T08:00:00</EarlyStart>
   <EarlyFinish>2007-11-15T17:00:00</EarlyFinish>
   <LateStart>2007-11-14T08:00:00</LateStart>
   <LateFinish>2007-11-15T17:00:00</LateFinish>
   <StartVariance>0</StartVariance>
   <FinishVariance>0</FinishVariance>
   <WorkVariance>0</WorkVariance>
   <FreeSlack>0</FreeSlack>
   <TotalSlack>0</TotalSlack>
   <FixedCost>0</FixedCost>
   <FixedCostAccrual>3</FixedCostAccrual>
   <PercentComplete>0</PercentComplete>
   <PercentWorkComplete>0</PercentWorkComplete>
   <Cost>0</Cost>
   <OvertimeCost>0</OvertimeCost>
   <OvertimeWork>PT0H0M0S</OvertimeWork>
   <ActualDuration>PT0H0M0S</ActualDuration>
   <ActualCost>0</ActualCost>
   <ActualOvertimeCost>0</ActualOvertimeCost>
   <ActualWork>PT0H0M0S</ActualWork>
   <ActualOvertimeWork>PT0H0M0S</ActualOvertimeWork>
   <RegularWork>PT0H0M0S</RegularWork>
   <RemainingDuration>PT16H0M0S</RemainingDuration>
   <RemainingCost>0</RemainingCost>
   <RemainingWork>PT0H0M0S</RemainingWork>
   <RemainingOvertimeCost>0</RemainingOvertimeCost>
   <RemainingOvertimeWork>PT0H0M0S</RemainingOvertimeWork>
   <ACWP>0</ACWP>
   <CV>0</CV>
   <ConstraintType>0</ConstraintType>
   <CalendarUID>-1</CalendarUID>
   <LevelAssignments>1</LevelAssignments>
   <LevelingCanSplit>1</LevelingCanSplit>
   <LevelingDelay>0</LevelingDelay>
   <LevelingDelayFormat>8</LevelingDelayFormat>
   <IgnoreResourceCalendar>0</IgnoreResourceCalendar>
   <HideBar>0</HideBar>
   <Rollup>1</Rollup>
   <BCWS>0</BCWS>
   <BCWP>0</BCWP>
   <PhysicalPercentComplete>0</PhysicalPercentComplete>
   <EarnedValueMethod>0</EarnedValueMethod>
   <IsPublished>1</IsPublished>
   <CommitmentType>0</CommitmentType>
</Task>
```

## 参照

#### その他の技術情報

[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)

