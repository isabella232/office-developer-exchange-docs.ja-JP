---
title: Transitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: Transitions 要素は、タイム ゾーン遷移の配列を表します。
ms.openlocfilehash: 7756878ed21bbe778bf51e99ade212f53414f998
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520312"
---
# <a name="transitions"></a>Transitions

**Transitions 要素** は、タイム ゾーン遷移の配列を表します。 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 **ArrayOfTransitionsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |タイム ゾーン定義の一意の識別子を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |特定の日付と特定の時刻に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーン遷移を表します。  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |指定した年の日に発生するタイム ゾーンの遷移を表します。  <br/> |
|[Transition](transition.md) <br/> |タイム ゾーンの切り替えを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の開始時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の終了時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |タイム ゾーンを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

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

