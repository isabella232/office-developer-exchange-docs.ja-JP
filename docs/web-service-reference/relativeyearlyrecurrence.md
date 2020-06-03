---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: RelativeYearlyRecurrence 要素は、相対的な年単位の定期的なパターンを記述します。
ms.openlocfilehash: 2abe09ddfe52c24211ef5d0a392ddecaf15bf7bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456735"
---
# <a name="relativeyearlyrecurrence"></a>RelativeYearlyRecurrence

**RelativeYearlyRecurrence**要素は、相対的な年単位の定期的なパターンを記述します。 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 **RelativeYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |アイテムの定期的なパターンで使用される曜日を表します。  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |1月の週が、相対的な年単位の定期的なパターンで使用されることを説明します。  <br/> |
|[月 (アイテムの定期的な予定)](month-item-recurrence.md) <br/> |年単位の定期的なアイテムが発生する月を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[定期的なアイテム (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的なアイテムの情報が含まれています。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンを含みます。  <br/> |
|[Standard](standard.md) <br/> |夏時間から標準時までの時刻が変更された日付と時刻を表します。  <br/> |
|[日光](daylight.md) <br/> |時刻が標準時から夏時間に変更された日付と時刻を表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

