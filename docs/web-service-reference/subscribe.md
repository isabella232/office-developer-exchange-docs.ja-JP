---
title: Subscribe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: Subscribe 要素には、サブスクリプションの作成に使用されるプロパティが含まれる。
ms.openlocfilehash: 172539f8d9644db39f8b9b3c60cbb6717afae1dd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517673"
---
# <a name="subscribe"></a>Subscribe

**Subscribe 要素** には、サブスクリプションの作成に使用されるプロパティが含まれる。 
  
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
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |プル ベースのイベント通知のサブスクリプションを表します。  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |プッシュ ベースのイベント通知のサブスクリプションを表します。  <br/> |
|[StreamingSubscriptionRequest](streamingsubscriptionrequest.md) <br/> |ストリーミング イベント通知のサブスクリプションを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

