---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: SubscriptionStatus 要素は、プッシュサブスクリプションの状態を表します。
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530945"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

**Subscriptionstatus**要素は、プッシュサブスクリプションの状態を表します。 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **SubscriptionStatusType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SendNotificationResult](sendnotificationresult.md) <br/> |プッシュ通知に対するクライアントアプリケーションの応答を含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素に使用できるテキスト値は次のとおりです。
  
- OK
    
- Unsubscribe
    
## <a name="remarks"></a>注釈

この要素は、サブスクリプションの状態を表します。 プッシュサブスクリプションクライアントアプリケーションは、各プッシュ通知の後にクライアントアクセスサーバーの役割がインストールされている、Exchange 2007 を実行しているコンピューターにステータスを送り返します。 **Subscriptionstatus**の値が**購読の取り消し**に等しい場合、クライアントアクセスサーバーは通知の送信を停止し、サブスクリプションを終了します。 **Subscriptionstatus**の値が**OK**の場合、クライアントアクセスサーバーは引き続き通知を送信します。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

