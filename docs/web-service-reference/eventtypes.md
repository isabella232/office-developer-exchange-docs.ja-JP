---
title: EventTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: EventTypes 要素には、サブスクリプションの作成に使用されるイベント通知の種類のコレクションが含まれています。
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530629"
---
# <a name="eventtypes"></a>EventTypes

**Eventtypes**要素には、サブスクリプションの作成に使用されるイベント通知の種類のコレクションが含まれています。 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 **非 Emptyarrayofnotificationeventtypest/型**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[EventType](eventtype.md) <br/> |サブスクリプションの作成に使用される要求されたイベント通知の種類を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プルベースのイベント通知サブスクリプションに対するサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュベースのイベント通知サブスクリプションのサブスクリプションを表します。  <br/> |
|[StreamingSubscriptionRequest](streamingsubscriptionrequest.md) <br/> |ストリーミングイベント通知サブスクリプションへのサブスクリプションを表します。  <br/> |
   
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



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

