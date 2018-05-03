---
title: BaseCalendarUID 要素
TOCTitle: BaseCalendarUID 要素
ms:assetid: f82f2ed0-9c87-4d05-940d-7fe6ef02f09c
ms:mtpsurl: https://msdn.microsoft.com/ja-jp/library/Bb968744(v=office.12)
ms:contentKeyID: 16750866
ms.date: 06/30/2008
mtps_version: v=office.12
ms.translationtype: HT
---

# BaseCalendarUID 要素

このカレンダーが依存する基本カレンダーの一意の ID。このカレンダーが基本カレンダーではない場合にのみ使用されます。

    <BaseCalendarUID>
        IntegerValue
    </BaseCalendarUID>

## 親要素

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="calendar-element.md">Calendar</a></p></td>
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


## 備考

値 `<BaseCalendarUID>-1</BaseCalendarUID>` の場合、カレンダーは基本カレンダーです。

## 参照

#### その他の技術情報

[Calendar 要素と XML データ構造](calendar-elements-and-xml-structure.md)  
[Calendars 要素の XML スキーマ](xml-schema-for-the-calendars-element.md)

