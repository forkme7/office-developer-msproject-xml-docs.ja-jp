---
title: Project 要素
TOCTitle: Project 要素
ms:assetid: d6c47ee7-56f0-480f-940c-a7b715e6c1c3
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968701(v=office.12)
ms:contentKeyID: 16748193
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Project 要素

**Project** はドキュメントのトップレベルの要素です。**Project** の子要素には、カレンダー、割り当て、タスク、リソース、拡張属性 (ユーザー設定フィールド)、work breakdown structure (WBS コード)、カスタム アウトライン コードなど、各プロジェクトのすべてのデータが含まれています。

    <Project>
      ComplexTypeValue
    </Project>

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
<td><p><a href="saveversion-element.md">SaveVersion</a></p></td>
<td><p>必須</p></td>
<td><p>新規。プロジェクト XML ファイルを保存した Project のバージョン。Microsoft Office Project 2007 では <strong>SaveVersion</strong> = 12 です。</p></td>
</tr>
<tr class="even">
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの一意の ID 文字列。Project 2007 では使用しないでください。</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>オプション</p></td>
<td><p>ProjectName.xml などのプロジェクト ファイル名</p></td>
</tr>
<tr class="even">
<td><p><a href="title-element-project.md">Title</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのタイトル。Project 2007 では使用しないでください。</p></td>
</tr>
<tr class="odd">
<td><p><a href="subject-element.md">Subject</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのサブジェクト。</p></td>
</tr>
<tr class="even">
<td><p><a href="category-element.md">Category</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが属するカテゴリ。</p></td>
</tr>
<tr class="odd">
<td><p><a href="company-element.md">Company</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトを作成した企業の名前。</p></td>
</tr>
<tr class="even">
<td><p><a href="manager-element.md">Manager</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの管理者。</p></td>
</tr>
<tr class="odd">
<td><p><a href="author-element.md">Author</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの作成者。</p></td>
</tr>
<tr class="even">
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが作成された日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="revision-element.md">Revision</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが保存された回数。</p></td>
</tr>
<tr class="even">
<td><p><a href="lastsaved-element.md">LastSaved</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが最後に保存された日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="schedulefromstart-element.md">ScheduleFromStart</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが開始日付と終了日付のどちらからスケジュールされたかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="startdate-element.md">StartDate</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの開始がスケジュールされている日付と時刻。<strong>ScheduleFromStart</strong> が true である場合は必須。</p></td>
</tr>
<tr class="odd">
<td><p><a href="finishdate-element.md">FinishDate</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの終了がスケジュールされている日付と時刻。<strong>ScheduleFromStart</strong> が false である場合は必須。</p></td>
</tr>
<tr class="even">
<td><p><a href="fystartdate-element.md">FYStartDate</a></p></td>
<td><p>オプション</p></td>
<td><p>会計年度が始まる月。</p></td>
</tr>
<tr class="odd">
<td><p><a href="criticalslacklimit-element.md">CriticalSlackLimit</a></p></td>
<td><p>オプション</p></td>
<td><p>Project がタスクをクリティカル タスクとしてマークする前に終了日付を超えてタスクが継続できる日数。</p></td>
</tr>
<tr class="even">
<td><p><a href="currencydigits-element.md">CurrencyDigits</a></p></td>
<td><p>オプション</p></td>
<td><p>Project が通貨の値を表示する場合に小数点の後に表示される桁数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="currencysymbol-element.md">CurrencySymbol</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトで使用される通貨の種類を表すために使用される通貨記号。</p></td>
</tr>
<tr class="even">
<td><p><a href="currencycode-element.md">CurrencyCode</a></p></td>
<td><p>オプション</p></td>
<td><p>Project 2007 の新しい要素。ユーロを表す EUR など、ISO 4217 で定義されている 3 文字の通貨文字コード。</p></td>
</tr>
<tr class="odd">
<td><p><a href="currencysymbolposition-element.md">CurrencySymbolPosition</a></p></td>
<td><p>オプション</p></td>
<td><p>通貨値に対する通貨記号の配置を示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトで使用されるカレンダーの一意の ID。</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultstarttime-element.md">DefaultStartTime</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての新規タスクの既定の開始時刻。</p></td>
</tr>
<tr class="even">
<td><p><a href="defaultfinishtime-element.md">DefaultFinishTime</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての新規タスクの既定の終了時刻。</p></td>
</tr>
<tr class="odd">
<td><p><a href="minutesperday-element.md">MinutesPerDay</a></p></td>
<td><p>オプション</p></td>
<td><p>1 日ごとの既定の分の数。</p></td>
</tr>
<tr class="even">
<td><p><a href="minutesperweek-element.md">MinutesPerWeek</a></p></td>
<td><p>オプション</p></td>
<td><p>1 週ごとの既定の分の数。</p></td>
</tr>
<tr class="odd">
<td><p><a href="dayspermonth-element.md">DaysPerMonth</a></p></td>
<td><p>オプション</p></td>
<td><p>1 月ごとの既定の稼働日の数。</p></td>
</tr>
<tr class="even">
<td><p><a href="defaulttasktype-element.md">DefaultTaskType</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのすべての新規タスクの既定の型。</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultfixedcostaccrual-element.md">DefaultFixedCostAccrual</a></p></td>
<td><p>オプション</p></td>
<td><p>固定コストが蓄積した (開始、割り当て済み、終了) 場合のプロジェクトの既定の部分。</p></td>
</tr>
<tr class="even">
<td><p><a href="defaultstandardrate-element.md">DefaultStandardRate</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいリソースの既定の標準レート。</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultovertimerate-element.md">DefaultOvertimeRate</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいリソースの既定の超過レート。</p></td>
</tr>
<tr class="even">
<td><p><a href="durationformat-element.md">DurationFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのすべての期間の既定の形式</p></td>
</tr>
<tr class="odd">
<td><p><a href="workformat-element.md">WorkFormat</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのすべての作業期間の既定の形式。</p></td>
</tr>
<tr class="even">
<td><p><a href="editableactualcosts-element.md">EditableActualCosts</a></p></td>
<td><p>オプション</p></td>
<td><p>Project が自動的に実際のコストを計算するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="honorconstraints-element.md">HonorConstraints</a></p></td>
<td><p>オプション</p></td>
<td><p>Project が、タスクの依存関係ではなく、制約日付に従ってタスクをスケジュールするかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="earnedvaluemethod-element.md">EarnedValueMethod</a></p></td>
<td><p>オプション</p></td>
<td><p>達成額を計算するための既定の方式。</p></td>
</tr>
<tr class="odd">
<td><p><a href="insertedprojectslikesummary-element.md">InsertedProjectsLikeSummary</a></p></td>
<td><p>オプション</p></td>
<td><p>挿入されたプロジェクトが、スケジュール計算用の独立したプロジェクトとしてではなく、サマリー タスクとして扱われるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="multiplecriticalpaths-element.md">MultipleCriticalPaths</a></p></td>
<td><p>オプション</p></td>
<td><p>Project がプロジェクト内のタスクの独立した各ネットワークのクリティカル パスを計算および表示するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="newtaskseffortdriven-element.md">NewTasksEffortDriven</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいタスクは残存作業時間を優先するかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="newtasksestimated-element.md">NewTasksEstimated</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいタスクに見積もり期間を設定するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="splitsinprogresstasks-element.md">SplitsInProgressTasks</a></p></td>
<td><p>オプション</p></td>
<td><p>進行中のタスクを分割できるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="spreadactualcost-element.md">SpreadActualCost</a></p></td>
<td><p>オプション</p></td>
<td><p>実績コストが状況報告日まで及んでいるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="spreadpercentcomplete-element.md">SpreadPercentComplete</a></p></td>
<td><p>オプション</p></td>
<td><p>達成率が状況報告日にまで広がるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="taskupdatesresource-element.md">TaskUpdatesResource</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに対する更新がリソースを更新するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="fiscalyearstart-element.md">FiscalYearStart</a></p></td>
<td><p>オプション</p></td>
<td><p>会計年度の番号が使用されるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="weekstartday-element.md">WeekStartDay</a></p></td>
<td><p>オプション</p></td>
<td><p>週の開始日。</p></td>
</tr>
<tr class="odd">
<td><p><a href="movecompletedendsback-element.md">MoveCompletedEndsBack</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日の後に始まるようにスケジュールされているが、早く始まったタスクの完了部分の終わりを状況報告日に戻す必要があるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="moveremainingstartsback-element.md">MoveRemainingStartsBack</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日の後に始まるようにスケジュールされているが、早く始まったタスクの残り部分を状況報告日に戻す必要があるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="moveremainingstartsforward-element.md">MoveRemainingStartsForward</a></p></td>
<td><p>オプション</p></td>
<td><p>遅く始まるようにスケジュールされているタスクの残り部分を、状況報告日に移動する必要があるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="movecompletedendsforward-element.md">MoveCompletedEndsForward</a></p></td>
<td><p>オプション</p></td>
<td><p>状況報告日の前に完了するようにスケジュールされているが、遅く始まったタスクの完了部分を状況報告日に移動する必要があるかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="baselineforearnedvalue-element.md">BaselineForEarnedValue</a></p></td>
<td><p>オプション</p></td>
<td><p>分散値を計算するために使用される固有の基準。</p></td>
</tr>
<tr class="even">
<td><p><a href="autoaddnewresourcesandtasks-element.md">AutoAddNewResourcesAndTasks</a></p></td>
<td><p>オプション</p></td>
<td><p>新しいリソースをリソース プールに自動的に追加するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="statusdate-element.md">StatusDate</a></p></td>
<td><p>オプション</p></td>
<td><p>計算と報告に使用される日付です。</p></td>
</tr>
<tr class="even">
<td><p><a href="currentdate-element.md">CurrentDate</a></p></td>
<td><p>オプション</p></td>
<td><p>Project が XML ファイルを生成したシステム日付。</p></td>
</tr>
<tr class="odd">
<td><p><a href="microsoftprojectserverurl-element.md">MicrosoftProjectServerURL</a></p></td>
<td><p>オプション</p></td>
<td><p>Windows 認証とフォーム認証のどちらを使用してログオンしたユーザーによってプロジェクトが作成されたかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="autolink-element.md">Autolink</a></p></td>
<td><p>オプション</p></td>
<td><p>挿入または移動されたタスクを自動的にリンクするかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="newtaskstartdate-element.md">NewTaskStartDate</a></p></td>
<td><p>オプション</p></td>
<td><p>新規タスクの既定の開始日付。</p></td>
</tr>
<tr class="even">
<td><p><a href="defaulttaskevmethod-element.md">DefaultTaskEVMethod</a></p></td>
<td><p>オプション</p></td>
<td><p>タスクに関する既定の達成額の方式。</p></td>
</tr>
<tr class="odd">
<td><p><a href="projectexternallyedited-element.md">ProjectExternallyEdited</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが外部で編集されたかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedcreationdate-element.md">ExtendedCreationDate</a></p></td>
<td><p>オプション</p></td>
<td><p>計算と報告に使用される日付です。</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualsinsync-element.md">ActualsInSync</a></p></td>
<td><p>オプション</p></td>
<td><p>すべての実績作業時間をプロジェクトと同期させるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="removefileproperties-element.md">RemoveFileProperties</a></p></td>
<td><p>オプション</p></td>
<td><p><strong>Author</strong>、<strong>Manager</strong>、および <strong>Company</strong> などの一部のファイル プロパティを保存時に削除するかどうかを示します。</p></td>
</tr>
<tr class="odd">
<td><p><a href="adminproject-element.md">AdminProject</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトが管理用プロジェクトであるかどうかを示します。</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinecodes-element.md">OutlineCodes</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトのローカルなアウトライン コード定義のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="wbsmasks-element.md">WBSMasks</a></p></td>
<td><p>オプション</p></td>
<td><p>work breakdown structure (WBS) マスクを定義するエントリのテーブル。</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattributes-element.md">ExtendedAttributes</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの拡張属性 (ユーザー設定フィールド) 定義のコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="calendars-element.md">Calendars</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトと関連付けられているカレンダーのコレクション。</p></td>
</tr>
<tr class="even">
<td><p><a href="tasks-element.md">Tasks</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトを構成するタスクのコレクション。</p></td>
</tr>
<tr class="odd">
<td><p><a href="resources-element.md">Resources</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトを構成するリソースのコレクション。</p></td>
</tr>
<tr class="even">
<td><p><a href="assignments-element.md">Assignments</a></p></td>
<td><p>オプション</p></td>
<td><p>プロジェクトの割り当てのコレクション。</p></td>
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
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## 備考

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
<td><p><strong>MoveCompletedEndsBack</strong>、<strong>MoveRemainingStartsBack</strong>、<strong>MoveRemainingStartsForward</strong>、および <strong>MoveCompletedEndsForward</strong> 要素には丸めエラーがあります。これらの要素の内部での作業時間の値は 8 桁です。これらの値は 1 分ごとに .001 秒を失うため、丸めエラーの原因になります。</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[Project 要素と XML データ構造](project-elements-and-xml-structure.md)  
[Project 要素の XML スキーマ](xml-schema-for-the-project-element.md)  
[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)  
[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)  
[WBSMasks 要素の XML スキーマ](xml-schema-for-the-wbsmasks-element.md)  
[ExtendedAttribute 要素と XML データ構造](extendedattribute-elements-and-xml-structure.md)  
[ExtendedAttributes 要素の XML スキーマ](xml-schema-for-the-extendedattributes-element.md)  
[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Resource 要素と XML データ構造](resource-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Assignments 要素の XML スキーマ](xml-schema-for-the-assignments-element.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)  
[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)

