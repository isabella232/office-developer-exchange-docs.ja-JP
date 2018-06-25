---
title: 通知
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: 通知の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報が含まれています。
ms.openlocfilehash: a769d8988eb68d0fa0b02f3838cd891e714571b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832547"
---
# <a name="notification"></a>通知

**通知**の要素には、サブスクリプション、および最後の通知以降に発生したイベントに関する情報が含まれています。 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

 **NotificationType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[サブスクリプション Id (GetEvents)](subscriptionid-getevents.md) <br/> |サブスクリプションの識別子を表します。  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |サブスクリプションでクライアントに正常に通信された最新イベントのウォーターマークを表します。  <br/> |
|[イベント](moreevents.md) <br/> |クライアントに配信するキューにその他のイベントがあるかどうかを示します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーのコピー先のイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されているイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されるイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによって発生するイベントを表します。  <br/> |
|[StatusEvent](statusevent.md) <br/> |通知メールボックスに新しいアクティビティが発生していないことを表します。  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |アイテムの空き時間情報が変更されたイベントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |状態および 1 つの GetEvents 要求の結果が含まれています。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |状態および 1 つの SendNotification 要求の結果が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

