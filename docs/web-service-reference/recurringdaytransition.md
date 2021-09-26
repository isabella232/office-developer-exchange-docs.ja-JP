---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: RecurringDayTransition 要素は、毎年同じ日に発生するタイム ゾーン遷移を表します。
ms.openlocfilehash: 3b567e5b906ec00bd71deb1c85f8049bb6de8e3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542884"
---
# <a name="recurringdaytransition"></a>RecurringDayTransition

**RecurringDayTransition 要素** は、毎年同じ日に発生するタイム ゾーン遷移を表します。 
  
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
|[To](to.md) <br/> |タイム ゾーン遷移 [の](period.md) ターゲットである Period または [TransitionsGroup](transitionsgroup.md) を指定します。  <br/> |
|[TimeOffset](timeoffset.md) <br/> |タイム ゾーン遷移の協定世界時 (UTC) からの期間オフセットを表します。  <br/> |
|[Month (タイム ゾーン切り替え)](month-time-zone-transition.md) <br/> |タイム ゾーンの移行が発生する月を表します。  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |タイム ゾーンの切り替えが発生する週の日を表します。  <br/> |
|[Occurrence (タイム ゾーン切り替え)](occurrence-time-zone-transition.md) <br/> |タイム ゾーンの切り替えが発生する月の週の日の発生を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |タイム ゾーンの切り替えのコレクションを表します。  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |タイム ゾーンの切り替えのコレクションを表します。  <br/> |
   
## <a name="remarks"></a>注釈

[RecurringDayTransition](recurringdaytransition.md)要素で表される可能性があるタイム ゾーン遷移の例は、毎年 2 月の第 2 火曜日に発生する遷移です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

