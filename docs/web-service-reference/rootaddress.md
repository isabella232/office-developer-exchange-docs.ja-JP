---
title: RootAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: RootAddress 要素は、RecipientTrackingEvent イベントのイベントを開始する最初のアドレスを表します。
ms.openlocfilehash: afe544d6ee8dea4cb416ad033ed2cd68976ec087
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833250"
---
# <a name="rootaddress"></a>RootAddress

**RootAddress**要素は、 [RecipientTrackingEvent](recipienttrackingevent.md)イベントのイベントを開始する最初のアドレスを表します。 
  
```xml
<RootAddress/>
```

 **NonEmptyStringType**
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

テキスト値は、追跡イベントを開始するアドレスです。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
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

