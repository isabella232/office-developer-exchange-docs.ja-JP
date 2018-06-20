---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: RecipientTrackingEvent 要素には、受信者の 1 つのイベントの情報が含まれています。
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832989"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

**RecipientTrackingEvent**要素には、受信者の 1 つのイベントの情報が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[日付 (MessageTracking)](date-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[Recipient](recipient.md) <br/> |この要素は必須です。  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |この要素は必須です。  <br/> |
|[EventDescription](eventdescription.md) <br/> |この要素は必須です。  <br/> |
|[EventData](eventdata.md) <br/> |この要素はオプションです。  <br/> |
|[サーバー (MessageTracking)](server-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[Internalid など](internalid.md) <br/> |この要素は必須です。  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |この要素はオプションです。  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |この要素はオプションです。  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |この要素はオプションです。  <br/> |
|[RootAddress](rootaddress.md) <br/> |この要素はオプションです。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |受信者の 1 つまたは複数の追跡イベントのリストが含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

