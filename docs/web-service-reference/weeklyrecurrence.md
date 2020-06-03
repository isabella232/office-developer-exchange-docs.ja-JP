---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: WeeklyRecurrence 要素は、週単位の定期的なパターンを記述します。
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530367"
---
# <a name="weeklyrecurrence"></a>WeeklyRecurrence

**WeeklyRecurrence**要素は、週単位の定期的なパターンを記述します。 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 **WeeklyRecurrencePatternType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[間隔](interval.md) <br/> |週単位の定期的な繰り返しパターンアイテム間の間隔 (週単位) を定義します。 この値は 1 ~ 99 の範囲で指定できます。  <br/> |
|[DaysOfWeek (DaysOfWeekType)](daysofweek-daysofweektype.md) <br/> |毎週の定期的なパターンに含まれる曜日を指定します。  <br/> |
|[FirstDayOfWeek](firstdayofweek.md) <br/> |週の最初の曜日を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[定期的なアイテム (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的なアイテムの情報が含まれています。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンを含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

定期的なマスターアイテムの[開始](start.md)日と[終了](end-ex15websvcsotherref.md)日に、最初に週単位の定期的なパターンと同じ日付が設定されていない場合は、タイムゾーンのオフセット情報は失われます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

