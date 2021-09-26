---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: SubscriptionStatus 要素は、プッシュ サブスクリプションの状態を表します。
ms.openlocfilehash: 6918a4965da2c075341c99581c3bd06c93da35fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546932"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

**SubscriptionStatus 要素** は、プッシュ サブスクリプションの状態を表します。 
  
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
|[SendNotificationResult](sendnotificationresult.md) <br/> |プッシュ通知に対するクライアント アプリケーションの応答を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素で使用できるテキスト値を次に示します。
  
- OK
    
- Unsubscribe
    
## <a name="remarks"></a>注釈

この要素は、サブスクリプションの状態を説明します。 プッシュ サブスクリプション クライアント アプリケーションは、プッシュ通知の後にクライアント アクセス サーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターに状態を戻します。 **SubscriptionStatus 値が** Unsubscribeと等しい場合、クライアント アクセス サーバーは通知の送信を停止し、サブスクリプションを終了します。 **SubscriptionStatus の値が** **OK** の場合、クライアント アクセス サーバーは引き続き通知を送信します。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

