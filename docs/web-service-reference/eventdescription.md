---
title: EventDescription
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventDescription
api_type:
- schema
ms.assetid: 7642cb03-71b1-4773-9508-4fbe3a5dcdf4
description: EventDescription 要素
ms.openlocfilehash: d496e6d2a61b4a72954b25fe3c5362f82aabf143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760340"
---
# <a name="eventdescription"></a>EventDescription

**EventDescription**要素 
  
```xml
<EventDescription/>
```

 **MessageTrackingEventDescriptionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> ||
   
## <a name="text-value"></a>テキスト値

次の表は、 **EventDescription**要素の値を一覧します。 
  
**EventDescription 要素の値**

|**値**|**説明**|
|:-----|:-----|
|Submitted  <br/> ||
|解決  <br/> ||
|Expanded  <br/> ||
|配信  <br/> ||
|MovedToFolderByInboxRule  <br/> ||
|RulesCc  <br/> ||
|FailedGeneral  <br/> ||
|FailedModeration  <br/> ||
|FailedTransportRules  <br/> ||
|SmtpSend  <br/> ||
|SmtpSendCrossSite  <br/> ||
|SmtpSendCrossForest  <br/> ||
|SmtpReceive  <br/> ||
|転送  <br/> ||
|Pending  <br/> ||
|PendingModeration  <br/> ||
|ApprovedModeration  <br/> ||
|QueueRetry  <br/> ||
|QueueRetryNoRetryTime  <br/> ||
|MessageDefer  <br/> ||
|TransferredToForeignOrg  <br/> ||
|TransferredToPartnerOrg  <br/> ||
|TransferredToLegacyExchangeServer  <br/> ||
|DelayedAfterTransferToPartnerOrg  <br/> ||
|読み取り  <br/> ||
|NotRead  <br/> ||
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

