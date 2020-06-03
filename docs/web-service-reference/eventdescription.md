---
title: イベントの説明
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
ms.openlocfilehash: 5f61a4eea945193d672afbcd2c693502ccf3e4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530636"
---
# <a name="eventdescription"></a>イベントの説明

**Eventdescription**要素 
  
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
|[受信者 Trackingイベント](recipienttrackingevent.md) <br/> ||
   
## <a name="text-value"></a>テキスト値

次の表に、 **Eventdescription**要素に指定できる値を示します。 
  
**EventDescription 要素の値**

|**値**|**説明**|
|:-----|:-----|
|Submitted  <br/> ||
|Resolved  <br/> ||
|Expanded  <br/> ||
|届け  <br/> ||
|Movedtofolderby受信トレイルール  <br/> ||
|ルール Cc  <br/> ||
|失敗の一般的な  <br/> ||
|失敗モデレーション  <br/> ||
|FailedTransportRules  <br/> ||
|Transportroles\logs\frontend\protocollog\smtpsend  <br/> ||
|SmtpSendCrossSite  <br/> ||
|SmtpSendCrossForest  <br/> ||
|Transportroles\logs\frontend\protocollog\smtpreceive  <br/> ||
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
|Read  <br/> ||
|NotRead  <br/> ||
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

