---
title: サブスクリプション Id (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: サブスクリプション Id 要素は、サブスクリプションの識別子を表します。
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833622"
---
# <a name="subscriptionid-getevents"></a>サブスクリプション Id (GetEvents)

**サブスクリプション Id**要素は、サブスクリプションの識別子を表します。 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |プル クライアントがサーバーからの通知を要求に使用する操作を表します。  <br/> |
|[通知](notification-ex15websvcsotherref.md) <br/> |サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Subscribe 要求の結果ステータスを格納します。  <br/> |
|[購読の取り消し](unsubscribe.md) <br/> |サブスクリプションの購読を解除するためのプロパティが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、GUID です。
  
## <a name="remarks"></a>備考

サブスクリプションの識別子を表す GUID は、サブスクリプションが作成されると、クライアント アクセス サーバーによって生成されます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[サブスクライブ操作](subscribe-operation.md)
  
[GetEvents 操作](getevents-operation.md)
  
[Unsubscribe 操作](unsubscribe-operation.md)

