---
title: 定期的なアイテム (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: 定期的なアイテムの要素には、予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833004"
---
# <a name="recurrence-recurrencetype"></a>定期的なアイテム (RecurrenceType)

**定期的なアイテム**の要素には、予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 **RecurrenceType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |相対年間の定期的なパターンをについて説明します。  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |1 年ごと。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |定期的な予定表アイテムの相対的な毎月定期的なパターンをについて説明します。  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |1 か月ごと。  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |週、および定期的に繰り返されるタスクの予定表アイテムで、頻度を説明します。  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |日単位での周波数を表すタスクの予定表アイテムが再発するのです。  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |定義された終了日がない定期的なパターンをについて説明します。  <br/> この要素の使用は、 [EndDateRecurrence](enddaterecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |開始日と終了日の項目の定期的なパターンについて説明します。  <br/> この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |開始日と定期的なアイテムの出現回数を説明します。  <br/> この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[EndDateRecurrence](enddaterecurrence.md)の要素の使用を除外します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は、 [CalendarItemType](calendaritemtype.md)に RecurringMaster の値が設定されている場合に有効です。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

