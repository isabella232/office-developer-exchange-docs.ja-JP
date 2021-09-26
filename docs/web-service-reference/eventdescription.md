---
title: EventDescription
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EventDescription
api_type:
- schema
ms.assetid: 7642cb03-71b1-4773-9508-4fbe3a5dcdf4
description: EventDescription 要素
ms.openlocfilehash: 324bf763575c551d594873052c37335de63325e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546554"
---
# <a name="eventdescription"></a>EventDescription

**EventDescription** 要素 
  
```xml
<EventDescription/>
```

 **MessageTrackingEventDescriptionType**
## <a name="attributes-and-elements"></a>属性と要素

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

次の表に **、EventDescription 要素に使用できる値を示** します。 
  
**EventDescription 要素の値**

|**値**|**説明**|
|:-----|:-----|
|Submitted  <br/> ||
|Resolved  <br/> ||
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
|Forwarded  <br/> ||
|保留中  <br/> ||
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
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

