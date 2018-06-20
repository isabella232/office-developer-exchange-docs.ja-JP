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
description: DeliveryStatus 要素は、メッセージのステータスを指定します。
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760006"
---
# <a name="deliverystatus"></a>DeliveryStatus

**DeliveryStatus**要素は、メッセージのステータスを指定します。 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |受信者の 1 つのイベントの情報が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**DeliveryStatus**要素の可能なテキスト値を次の表に一覧します。 
  
**DeliveryStatus 要素の値**

|**値**|**説明**|
|:-----|:-----|
|失敗しました。  <br/> |メッセージが配信されなかったことを指定します。  <br/> |
|Pending  <br/> |メッセージがモデレーターの承認を待機しているかを指定します。  <br/> |
|配信  <br/> |すべての指定された受信者にメッセージが配信されたことを指定します。  <br/> |
|転送  <br/> |検索範囲外のサーバにメッセージが転送されたことを指定します。  <br/> |
|読み取り  <br/> |メッセージが配信され、受信者が読み取ることを指定します。  <br/> |
   
## <a name="remarks"></a>備考

**DeliveryStatus**要素は、[Exchange Server 2010 の型**MessageTrackingDeliveryStatusType**のでした。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

