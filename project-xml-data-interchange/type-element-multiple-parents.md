---
title: Type 要素 (複数の親)
TOCTitle: Type 要素
ms:assetid: 222dd5ab-8885-4858-b5c3-87f0d1636d2d
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968434(v=office.12)
ms:contentKeyID: 16733203
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# Type 要素 (複数の親)

**Mask** または ** WBSMask ** 要素の子の場合、** Type ** は第 1 レベルのタスクのコード文字列 (数字、文字、または順序付けされていない文字) です。

** Task** 要素では、** Type ** はタスクの種類 (単位数固定、期間固定、または作業時間固定) です。

** PredecessorLink** 要素では、**Type ** はタスク リンクの種類 (FF、FS、SF、または SS) です。

** Resource** 要素では、**Type ** はリソースの種類 (数量単価型または時間単価型) です。

**Exception** 要素では、**Type** はカレンダーの例外の種類 (毎日、毎週など) です。

**Value** 要素では、**Type** はアウトライン コードの種類 (日付、期間、テキストなど) です。

** TimephasedData** 要素では、**Type ** は 76 種類の時間配分されたデータの 1 つです。

    <Type>
      IntegerValue
    </Type>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="mask-element.md">Mask</a>、<a href="wbsmask-element.md">WBSMask</a>、<a href="task-element.md">Task</a>、<a href="predecessorlink-element.md">PredecessorLink</a>、<a href="resource-element.md">Resource</a>、<a href="exception-element.md">Exception 要素</a>、<a href="value-element.md">Value 要素</a>、<a href="timephaseddata-element.md">TimephasedData</a></p></td>
</tr>
</tbody>
</table>


### Mask または WBSMask の要素のプロパティ :

**Type** 要素は、第 1 レベルのタスクのコード文字列の種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>数字 (順序付けあり)。このレベルの数値の WBS コード (既定)。</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>大文字 (順序付けあり)。大文字のアルファベットの WBS コード (たとえば、プロジェクト内の最初の 3 つのサマリー タスクの場合は A、B、および C)。</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>小文字 (順序付けあり)。小文字のアルファベットの WBS コード (たとえば、プロジェクト内の最初の 3 つのサマリー タスクの場合は a、b、および c)。</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>文字 (順序付けなし)。数字、大文字、または小文字の任意の組み合わせ。たとえば、プロジェクトの最初の 3 つのサマリー タスクについて、Arch1、Const1、または Insp1 などです。Project 2007 では、コードの文字列を入力するまでは、ユーザー設定アウトライン フィールドにアスタリスク (*) が表示されます。</p></td>
</tr>
</tbody>
</table>


### Task の要素のプロパティ :

**Type** 要素は、タスクの種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>単位数固定</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>期間固定</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>作業時間固定</p></td>
</tr>
</tbody>
</table>


### PredecessorLink の要素のプロパティ :

**Type** 要素は、タスク リンクの種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>FF (終了-終了)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>FS (終了-開始)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>SF (開始-終了)</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>SS (開始-開始)</p></td>
</tr>
</tbody>
</table>


### Resource の要素のプロパティ :

**Type** 要素は、リソースの種類 (時間単価型、数量単価型、またはコスト型) を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>数量単価型 (鋼鉄、コンクリート、土などの消耗物資)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>時間単価型 (人および機材)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>コスト型リソース</p></td>
</tr>
</tbody>
</table>


### Exception の要素のプロパティ :

**Type** 要素は、カレンダーの例外の種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>1</p></td>
<td><p>毎日</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>月の日付で年に 1 回</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>位置で年に 1 回</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>月の日付で月に 1 回</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>位置で月に 1 回</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>毎週</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>日数</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>稼働日の日数</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>例外の種類なし</p></td>
</tr>
</tbody>
</table>


### Value の要素のプロパティ :

**Type** 要素は、アウトライン コードの種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>4</p></td>
<td><p>日付</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>期間</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>コスト</p></td>
</tr>
<tr class="even">
<td><p>15</p></td>
<td><p>数</p></td>
</tr>
<tr class="odd">
<td><p>17</p></td>
<td><p>フラグ</p></td>
</tr>
<tr class="even">
<td><p>21</p></td>
<td><p>テキスト</p></td>
</tr>
<tr class="odd">
<td><p>27</p></td>
<td><p>終了日</p></td>
</tr>
</tbody>
</table>


### TimephasedData の要素のプロパティ :

**Type** 要素は、時間配分されたデータの種類を表す整数値を含みます。

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><strong>値</strong></th>
<th><strong>説明</strong></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>1</p></td>
<td><p>割り当て残存作業時間</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>割り当て実績作業時間</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>割り当て実績超過作業時間</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>割り当て基準作業時間</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>割り当て基準コスト</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>割り当て実績コスト</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>リソース基準作業時間</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>リソース基準コスト</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>タスク基準作業時間</p></td>
</tr>
<tr class="even">
<td><p>10</p></td>
<td><p>タスク基準コスト</p></td>
</tr>
<tr class="odd">
<td><p>11</p></td>
<td><p>タスク達成率</p></td>
</tr>
<tr class="even">
<td><p>16</p></td>
<td><p>割り当て基準計画 1 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>17</p></td>
<td><p>割り当て基準計画 1 コスト</p></td>
</tr>
<tr class="even">
<td><p>18</p></td>
<td><p>タスク基準計画 1 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>19</p></td>
<td><p>タスク基準計画 1 コスト</p></td>
</tr>
<tr class="even">
<td><p>20</p></td>
<td><p>リソース基準計画 1 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>21</p></td>
<td><p>リソース基準計画 1 コスト</p></td>
</tr>
<tr class="even">
<td><p>22</p></td>
<td><p>割り当て基準計画 2 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>23</p></td>
<td><p>割り当て基準計画 2 コスト</p></td>
</tr>
<tr class="even">
<td><p>24</p></td>
<td><p>タスク基準計画 2 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>25</p></td>
<td><p>タスク基準計画 2 コスト</p></td>
</tr>
<tr class="even">
<td><p>26</p></td>
<td><p>リソース基準計画 2 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>27</p></td>
<td><p>リソース基準計画 2 コスト</p></td>
</tr>
<tr class="even">
<td><p>28</p></td>
<td><p>割り当て基準計画 3 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>29</p></td>
<td><p>割り当て基準計画 3 コスト</p></td>
</tr>
<tr class="even">
<td><p>30</p></td>
<td><p>タスク基準計画 3 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>31</p></td>
<td><p>タスク基準計画 3 コスト</p></td>
</tr>
<tr class="even">
<td><p>32</p></td>
<td><p>リソース基準計画 3 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>33</p></td>
<td><p>リソース基準計画 3 コスト</p></td>
</tr>
<tr class="even">
<td><p>34</p></td>
<td><p>割り当て基準計画 4 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>35</p></td>
<td><p>割り当て基準計画 4 コスト</p></td>
</tr>
<tr class="even">
<td><p>36</p></td>
<td><p>タスク基準計画 4 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>37</p></td>
<td><p>タスク基準計画 4 コスト</p></td>
</tr>
<tr class="even">
<td><p>38</p></td>
<td><p>リソース基準計画 4 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>39</p></td>
<td><p>リソース基準計画 4 コスト</p></td>
</tr>
<tr class="even">
<td><p>40</p></td>
<td><p>割り当て基準計画 5 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>41</p></td>
<td><p>割り当て基準計画 5 コスト</p></td>
</tr>
<tr class="even">
<td><p>42</p></td>
<td><p>タスク基準計画 5 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>43</p></td>
<td><p>タスク基準計画 5 コスト</p></td>
</tr>
<tr class="even">
<td><p>44</p></td>
<td><p>リソース基準計画 5 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>45</p></td>
<td><p>リソース基準計画 5 コスト</p></td>
</tr>
<tr class="even">
<td><p>46</p></td>
<td><p>割り当て基準計画 6 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>47</p></td>
<td><p>割り当て基準計画 6 コスト</p></td>
</tr>
<tr class="even">
<td><p>48</p></td>
<td><p>タスク基準計画 6 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>49</p></td>
<td><p>タスク基準計画 6 コスト</p></td>
</tr>
<tr class="even">
<td><p>50</p></td>
<td><p>リソース基準計画 6 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>51</p></td>
<td><p>リソース基準計画 6 コスト</p></td>
</tr>
<tr class="even">
<td><p>52</p></td>
<td><p>割り当て基準計画 7 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>53</p></td>
<td><p>割り当て基準計画 7 コスト</p></td>
</tr>
<tr class="even">
<td><p>54</p></td>
<td><p>タスク基準計画 7 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>55</p></td>
<td><p>タスク基準計画 7 コスト</p></td>
</tr>
<tr class="even">
<td><p>56</p></td>
<td><p>リソース基準計画 7 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>57</p></td>
<td><p>リソース基準計画 7 コスト</p></td>
</tr>
<tr class="even">
<td><p>58</p></td>
<td><p>割り当て基準計画 8 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>59</p></td>
<td><p>割り当て基準計画 8 コスト</p></td>
</tr>
<tr class="even">
<td><p>60</p></td>
<td><p>タスク基準計画 8 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>61</p></td>
<td><p>タスク基準計画 8 コスト</p></td>
</tr>
<tr class="even">
<td><p>62</p></td>
<td><p>リソース基準計画 8 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>63</p></td>
<td><p>リソース基準計画 8 コスト</p></td>
</tr>
<tr class="even">
<td><p>64</p></td>
<td><p>割り当て基準計画 9 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>65</p></td>
<td><p>割り当て基準計画 9 コスト</p></td>
</tr>
<tr class="even">
<td><p>66</p></td>
<td><p>タスク基準計画 9 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>67</p></td>
<td><p>タスク基準計画 9 コスト</p></td>
</tr>
<tr class="even">
<td><p>68</p></td>
<td><p>リソース基準計画 9 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>69</p></td>
<td><p>リソース基準計画 9 コスト</p></td>
</tr>
<tr class="even">
<td><p>70</p></td>
<td><p>割り当て基準計画 10 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>71</p></td>
<td><p>割り当て基準計画 10 コスト</p></td>
</tr>
<tr class="even">
<td><p>72</p></td>
<td><p>タスク基準計画 10 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>73</p></td>
<td><p>タスク基準計画 10 コスト</p></td>
</tr>
<tr class="even">
<td><p>74</p></td>
<td><p>リソース基準計画 10 作業時間</p></td>
</tr>
<tr class="odd">
<td><p>75</p></td>
<td><p>リソース基準計画 10 コスト</p></td>
</tr>
<tr class="even">
<td><p>76</p></td>
<td><p>実際の達成率</p></td>
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
<p>最大 : 1</p></td>
</tr>
</tbody>
</table>


## 参照

#### その他の技術情報

[OutlineCode 要素と XML データ構造](outlinecode-elements-and-xml-structure.md)  
[OutlineCodes 要素の XML スキーマ](xml-schema-for-the-outlinecodes-element.md)  
[WBSMask 要素と XML データ構造](wbsmask-elements-and-xml-structure.md)  
[WBSMasks 要素の XML スキーマ](xml-schema-for-the-wbsmasks-element.md)  
[Task 要素と XML データ構造](task-elements-and-xml-structure.md)  
[Tasks 要素の XML スキーマ](xml-schema-for-the-tasks-element.md)  
[Assignment 要素と XML データ構造](assignment-elements-and-xml-structure.md)  
[Resources 要素の XML スキーマ](xml-schema-for-the-resources-element.md)  
[TimephasedDataType 要素と XML データ構造](timephaseddatatype-elements-and-xml-structure.md)  
[TimephasedDataType 複合型の XML スキーマ](xml-schema-for-the-timephaseddatatype-complex-type.md)

