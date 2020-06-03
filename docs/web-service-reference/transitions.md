---
title: 切り替わる
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: トランジションビュー要素は、タイムゾーンの遷移の配列を表します。
ms.openlocfilehash: d48fb8872b2f7e052f733c32e5dd1c9b4d04d898
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467439"
---
# <a name="transitions"></a>切り替わる

**トランジションビュー**要素は、タイムゾーンの遷移の配列を表します。 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 **Arrayofstype Tionstype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |タイムゾーン定義の一意識別子を表します。  <br/> |
   
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |特定の日付および特定の時刻に発生するタイムゾーンの切り替えを表します。  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイムゾーンの切り替えを表します。  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |指定した日に発生するタイムゾーンの切り替えを表します。  <br/> |
|[Transition](transition.md) <br/> |タイムゾーンの切り替えを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[Calendaritem](calendaritem.md)または[会議要求](meetingrequest.md)の開始時刻のタイムゾーンを定義します。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[Calendaritem](calendaritem.md)または[会議の要求](meetingrequest.md)の終了時刻のタイムゾーンを定義します。  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |タイムゾーンを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

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

