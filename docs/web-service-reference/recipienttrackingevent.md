---
title: 受信者 Trackingイベント
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
description: 受信者 Trackingevent 要素には、受信者に対する1つのイベントに関する情報が含まれています。
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465486"
---
# <a name="recipienttrackingevent"></a>受信者 Trackingイベント

受信者**trackingevent**要素には、受信者に対する1つのイベントに関する情報が含まれています。 
  
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

 **受信者 Trackingeventtype**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[日付 (MessageTracking)](date-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[[受信者]](recipient.md) <br/> |この要素は必須です。  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |この要素は必須です。  <br/> |
|[イベントの説明](eventdescription.md) <br/> |この要素は必須です。  <br/> |
|[EventData](eventdata.md) <br/> |この要素は省略できます。  <br/> |
|[サーバー (MessageTracking)](server-messagetracking.md) <br/> |この要素は必須です。  <br/> |
|[InternalId](internalid.md) <br/> |この要素は必須です。  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |この要素は省略できます。  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |この要素は省略できます。  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |この要素は省略できます。  <br/> |
|[RootAddress](rootaddress.md) <br/> |この要素は省略できます。  <br/> |
|[プロパティ (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[受信者 Trackingevents](recipienttrackingevents.md) <br/> |受信者の1つまたは複数の追跡イベントのリストを格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

