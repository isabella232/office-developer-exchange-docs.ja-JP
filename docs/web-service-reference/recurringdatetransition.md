---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: RecurringDateTransition 要素は、毎年特定の日に発生するタイム ゾーンの移行を表します。
ms.openlocfilehash: 7cd8f3452a744e0c9a98fd3698dffb9ed8721a6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833014"
---
# <a name="recurringdatetransition"></a>RecurringDateTransition

**RecurringDateTransition**要素は、毎年特定の日に発生するタイム ゾーンの移行を表します。 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 **RecurringDateTransitionType**
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
|[日](day.md) <br/> |タイム ゾーンの切り替えが発生する月の日を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[遷移](transitions.md) <br/> |タイム ゾーンの切り替え効果のコレクションを表します。  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |タイム ゾーンの切り替え効果のコレクションを表します。  <br/> |
   
## <a name="remarks"></a>備考

[RecurringDateTransition](recurringdatetransition.md)要素によって表すことができるタイム ゾーンの切り替えの例としては毎年 3 月 15 日に移行します。 
  
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

