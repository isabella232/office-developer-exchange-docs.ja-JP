---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: GetEvents 要素では、プル クライアントがサーバーからの通知を要求に使用する操作を表します。
ms.openlocfilehash: e7b24207bff579a2f5230676d6520452f96fe0ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760704"
---
# <a name="getevents"></a>GetEvents

**GetEvents**要素では、プル クライアントがサーバーからの通知を要求に使用する操作を表します。 
  
[GetEvents](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 **GetEventsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[サブスクリプション Id (GetEvents)](subscriptionid-getevents.md) <br/> |イベントを照会するサブスクリプションの識別子を表します。  <br/> |
|[透かし](watermark.md) <br/> |クライアントに返される最新のウォーターマークを表します。 このサブスクリプションの GetEvents が呼び出されていない場合、クライアントは、Subscribe 要求から返された透かしを使用します。 それ以外の場合、最新の GetEvents 応答の最後のイベントからのウォーターマークが使用されます。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

