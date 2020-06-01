---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: DeliveryStatus 要素は、メッセージの状態を指定します。
ms.openlocfilehash: ae32202284d3dd272f693fbb7b76070cb6019d28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461402"
---
# <a name="deliverystatus"></a>DeliveryStatus

**Deliverystatus**要素は、メッセージの状態を指定します。 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[受信者 Trackingイベント](recipienttrackingevent.md) <br/> |受信者に対する1つのイベントに関する情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**Deliverystatus**要素の使用可能なテキスト値を次の表に示します。 
  
**DeliveryStatus 要素の値**

|**値**|**説明**|
|:-----|:-----|
|いか  <br/> |メッセージが配信されなかったことを指定します。  <br/> |
|Pending  <br/> |メッセージがモデレーターからの承認を待機していることを指定します。  <br/> |
|届け  <br/> |メッセージが指定されたすべての受信者に配信されたことを示します。  <br/> |
|付与  <br/> |メッセージが検索範囲外のサーバーに転送されたことを示します。  <br/> |
|Read  <br/> |受信者によってメッセージが配信および開封されたことを示します。  <br/> |
   
## <a name="remarks"></a>注釈

**Deliverystatus**要素の種類は、Exchange Server 2010 の**Messagetrackingdeliverystatustype**た。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

