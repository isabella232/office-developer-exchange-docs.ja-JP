---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: SubscriptionId 要素は、サブスクリプションの識別子を表します。
ms.openlocfilehash: c24ae8dc61fa98716efc38d7a2500cab503760b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522587"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (GetEvents)

**SubscriptionId 要素** は、サブスクリプションの識別子を表します。 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |プル クライアントがサーバーから通知を要求するために使用する操作を表します。  <br/> |
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションと、前回の通知以降に発生したイベントに関する情報が格納されます。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |サブスクライブ要求の状態と結果を格納します。  <br/> |
|[登録を解除する](unsubscribe.md) <br/> |サブスクリプションの購読解除に使用するプロパティを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は GUID です。
  
## <a name="remarks"></a>注釈

サブスクリプション識別子を表す GUID は、サブスクリプションの作成時にクライアント アクセス サーバーによって生成されます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

