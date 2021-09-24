---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: WeeklyRecurrence 要素は、毎週の定期的なパターンを表します。
ms.openlocfilehash: 408116dd85fb31fce8f5f3b5b4cde92945783f5d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509337"
---
# <a name="weeklyrecurrence"></a>WeeklyRecurrence

**WeeklyRecurrence 要素は**、毎週の定期的なパターンを表します。 
  
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
|[間隔](interval.md) <br/> |週に 2 つの連続する定期的なパターンアイテム間の間隔を週単位で定義します。 値の範囲は 1 ~ 99 です。  <br/> |
|[DaysOfWeek (DaysOfWeekType)](daysofweek-daysofweektype.md) <br/> |週ごとの繰り返しパターンに含める週の日数を示します。  <br/> |
|[FirstDayOfWeek](firstdayofweek.md) <br/> |週の最初の日を指定します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的な情報が含まれています。  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンが含まれます。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

タイム ゾーン のオフセット情報は、[](start.md)定期的な[](end-ex15websvcsotherref.md)マスター アイテムの開始日と終了日に、週ごとの定期的なパターンの最初の出現日付と等しくない場合に失われます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

