---
title: RecipientTrackingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvents
api_type:
- schema
ms.assetid: c4f729aa-674e-43b2-97f2-bf49740b0a34
description: RecipientTrackingEvents 要素は、メッセージの 1 つまたは複数のイベントのコレクションを表します。
ms.openlocfilehash: 5fa5df422eff533891d021b77d5443b314d36244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832993"
---
# <a name="recipienttrackingevents"></a>RecipientTrackingEvents

**RecipientTrackingEvents**要素は、メッセージの 1 つまたは複数のイベントのコレクションを表します。 
  
```XML
<RecipientTrackingEvents>
   <RecipientTrackingEvent/>
</RecipientTrackingEvents>
```

 **ArrayOfRecipientTrackingEventType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |追跡レポートで特定のイベントの詳細が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[MessageTrackingReport](messagetrackingreport.md) <br/> |[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。  <br/> |
   
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

