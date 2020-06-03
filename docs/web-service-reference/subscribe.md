---
title: 登録
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: Subscribe 要素には、サブスクリプションの作成に使用されるプロパティが含まれています。
ms.openlocfilehash: f60e67654fb6af76e8081036a3463f5be401862d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530959"
---
# <a name="subscribe"></a>登録

**Subscribe**要素には、サブスクリプションの作成に使用されるプロパティが含まれています。 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 **SubscribeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プルベースのイベント通知のサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュベースのイベント通知のサブスクリプションを表します。  <br/> |
|[StreamingSubscriptionRequest](streamingsubscriptionrequest.md) <br/> |ストリーミングイベント通知のサブスクリプションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

