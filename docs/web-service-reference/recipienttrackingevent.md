---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: RecipientTrackingEvent 要素には、受信者の 1 つのイベントに関する情報が含まれる。
ms.openlocfilehash: 30d9cd4ca075fda9607b191f576cac1b7a529988
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525764"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

**RecipientTrackingEvent 要素** には、受信者の 1 つのイベントに関する情報が含まれる。 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 **RecipientTrackingEventType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Date (MessageTracking)](date-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[[受信者]](recipient.md) <br/> |この要素は必須です。  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |この要素は必須です。  <br/> |
|[EventDescription](eventdescription.md) <br/> |この要素は必須です。  <br/> |
|[EventData](eventdata.md) <br/> |この要素は省略できます。  <br/> |
|[Server (MessageTracking)](server-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[InternalId](internalid.md) <br/> |この要素は必須です。  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |この要素は省略できます。  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |この要素は省略できます。  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |この要素は省略できます。  <br/> |
|[RootAddress](rootaddress.md) <br/> |この要素は省略できます。  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |受信者の 1 つ以上の追跡イベントの一覧を含む。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

