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
description: Notification 要素には、サブスクリプションに関する情報と、最後の通知以降に発生したイベントが含まれます。
ms.openlocfilehash: c4a5206c14985ec46cf40162a9ce4eaec68242ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530388"
---
# <a name="notification"></a>通知

**Notification**要素には、サブスクリプションに関する情報と、最後の通知以降に発生したイベントが含まれます。 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

**NotificationType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |サブスクリプションの識別子を表します。  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |サブスクリプションのためにクライアントに正常に伝達された最新のイベントのウォーターマークを表します。  <br/> |
|[その他のイベント](moreevents.md) <br/> |クライアントに配信されるキューに、さらにイベントがあるかどうかを示します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[対する createdevent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されるイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[対する modifiedevent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されるイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。  <br/> |
|[StatusEvent](statusevent.md) <br/> |メールボックス内で新しいアクティビティが発生していないことを示す通知を表します。  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |アイテムの空き時間情報が変更されたイベントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |単一の GetEvents 要求の状態と結果を格納します。  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |1回の SendNotification 要求の状態と結果を格納します。  <br/> |
   
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

- [サブスクライブ操作](subscribe-operation.md) 
- [GetEvents 操作](getevents-operation.md) 
- [GetStreamingEvents の操作](getstreamingevents-operation.md) 
- [Unsubscribe 操作](unsubscribe-operation.md)

