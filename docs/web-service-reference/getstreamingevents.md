---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: GetStreamingEvents 要素は、クライアントがサーバーからストリーミング通知を要求するために使用する操作を表します。
ms.openlocfilehash: 8a68b3edbb53b623e4dc709e0128c5b3ebc94f91
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523053"
---
# <a name="getstreamingevents"></a>GetStreamingEvents

**GetStreamingEvents** 要素は、クライアントがサーバーからストリーミング通知を要求するために使用する操作を表します。 
  
[GetStreamingEvents](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 **GetStreamingEventsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) <br/> |イベントに対してクエリを実行するサブスクリプションの識別子を表します。  <br/> |
|[ConnectionTimeout](connectiontimeout.md) <br/> |接続を開いた状態に保つ時間 (分) を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

