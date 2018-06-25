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
description: RecurringDayTransition 要素は、毎年同じ日に発生するタイム ゾーンの移行を表します。
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833012"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

**RecurringDayTransition**要素は、毎年同じ日に発生するタイム ゾーンの移行を表します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[To](to.md) <br/> |[TransitionsGroup](transitionsgroup.md)タイム ゾーンの移行の対象となる[期間](period.md)を指定します。  <br/> |
|[TimeOffset](timeoffset.md) <br/> |タイム ゾーンの移行の世界協定時刻 (UTC) からの期間のオフセットを表します。  <br/> |
|[月 (タイム ゾーンの切り替え)](month-time-zone-transition.md) <br/> |タイム ゾーンの切り替えが発生する月を表します。  <br/> |
|[DayOfWeek (タイムゾーン)](dayofweek-timezone.md) <br/> |タイム ゾーンの切り替えが発生する曜日を表します。  <br/> |
|[発生 (タイム ゾーンの切り替え)](occurrence-time-zone-transition.md) <br/> |タイム ゾーンの切り替えが発生する月の週の日の発生を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[遷移](transitions.md) <br/> |タイム ゾーンの切り替え効果のコレクションを表します。  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |タイム ゾーンの切り替え効果のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>備考

[RecurringDayTransition](recurringdaytransition.md)要素によって表すことができるタイム ゾーンの切り替えの例としては毎年 2 月の第 2 火曜日に移行します。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

