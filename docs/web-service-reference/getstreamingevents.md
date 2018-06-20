---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: GetStreamingEvents 要素は、サーバーからのストリーミングの通知を要求するクライアントによって使用される演算を表します。
ms.openlocfilehash: b07015541cf9c2fbbbc11ebc9f10421bdb9ee84f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831679"
---
# <a name="getstreamingevents"></a>GetStreamingEvents

**GetStreamingEvents**要素は、サーバーからのストリーミングの通知を要求するクライアントによって使用される演算を表します。 
  
[GetStreamingEvents](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 **GetStreamingEventsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[サブスクリプション Id (GetStreamingEvents)](subscriptionid-getstreamingevents.md) <br/> |イベントを照会するサブスクリプションの識別子を表します。  <br/> |
|[タイムアウト](connectiontimeout.md) <br/> |接続を開いたままにしておく秒数を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetStreamingEvents の操作](getstreamingevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

