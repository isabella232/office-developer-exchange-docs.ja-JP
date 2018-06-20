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
description: SubscriptionStatus 要素では、プッシュ サブスクリプションの状態について説明します。
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839619"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

**SubscriptionStatus**要素では、プッシュ サブスクリプションの状態について説明します。 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **SubscriptionStatusType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[SendNotificationResult](sendnotificationresult.md) <br/> |クライアント アプリケーションの応答が含まれています ' プッシュ通知をします。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素の使用可能なテキスト値は、次のように。
  
- OK
    
- 登録を解除する
    
## <a name="remarks"></a>備考

この要素では、サブスクリプションの状態について説明します。 プッシュ サブスクリプションのクライアント アプリケーションは、プッシュ通知の後にインストールされているクライアント アクセス サーバーの役割を Exchange 2007 を実行しているコンピューターにステータスを送信します。 **SubscriptionStatus**の値には、**購読の取り消し**が等しくなると、クライアント アクセス サーバーは通知の送信を停止し、サブスクリプションを終了します。 **SubscriptionStatus**の値には、 **[ok]** が表示、クライアント アクセス サーバーの通知を送信する続けます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

