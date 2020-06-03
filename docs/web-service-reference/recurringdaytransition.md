---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: RecurringDayTransition 要素は、毎年同じ日に発生するタイムゾーンの切り替えを表します。
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468468"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

**RecurringDayTransition**要素は、毎年同じ日に発生するタイムゾーンの切り替えを表します。 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 **RecurringDayTransitionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[To](to.md) <br/> |タイムゾーンの遷移のターゲットである[期間](period.md)[または時間を指定](transitionsgroup.md)します。  <br/> |
|[TimeOffset](timeoffset.md) <br/> |タイムゾーンの切り替えについて、世界協定時刻 (UTC) からの時間オフセットを表します。  <br/> |
|[月 (タイムゾーン切り替え)](month-time-zone-transition.md) <br/> |タイムゾーンの切り替えが行われる月を表します。  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |タイムゾーンの切り替えが行われる曜日を表します。  <br/> |
|[発生 (タイムゾーンの切り替え)](occurrence-time-zone-transition.md) <br/> |タイムゾーンの切り替えが行われる月の曜日の発生を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[切り替わる](transitions.md) <br/> |タイムゾーンの遷移のコレクションを表します。  <br/> |
|[遷移 Tionsgroup](transitionsgroup.md) <br/> |タイムゾーンの遷移のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

[RecurringDayTransition](recurringdaytransition.md)要素によって表される可能性があるタイムゾーンの遷移の例としては、各年2月2日の火曜日に発生する遷移があります。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

