---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: DeliveryStatus 要素は、メッセージの状態を指定します。
ms.openlocfilehash: f11952f401e0d22d780725598bfb32cbd3a8d622
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543388"
---
# <a name="deliverystatus"></a>DeliveryStatus

**DeliveryStatus 要素** は、メッセージの状態を指定します。 
  
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
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |受信者の 1 つのイベントの情報を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

次の表に **、DeliveryStatus** 要素で使用できるテキスト値を示します。 
  
**DeliveryStatus 要素の値**

|**値**|**説明**|
|:-----|:-----|
|失敗しました  <br/> |メッセージが配信されていないと指定します。  <br/> |
|保留中  <br/> |メッセージがモデレーターからの承認を待つことを指定します。  <br/> |
|配信  <br/> |指定した受信者全員にメッセージが配信されたと指定します。  <br/> |
|転送  <br/> |メッセージが検索範囲外のサーバーに転送されたと指定します。  <br/> |
|読み取り  <br/> |メッセージが受信者によって配信および読み取りされたと指定します。  <br/> |
   
## <a name="remarks"></a>注釈

**DeliveryStatus 要素は**、2010 年に **MessageTrackingDeliveryStatusType** Exchange Serverしました。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

