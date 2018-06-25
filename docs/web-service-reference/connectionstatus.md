---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: ConnectionStatus 要素は、ストリーミングのサブスクリプションの状態の説明を提供します。
ms.openlocfilehash: 567308d79eaccba24230deddf5d78a724b8746af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759660"
---
# <a name="connectionstatus"></a>ConnectionStatus

**ConnectionStatus**要素は、ストリーミングのサブスクリプションの状態の説明を提供します。 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 **ConnectionStatusType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[GetStreamingEvents の操作](getstreamingevents-operation.md)を要求します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素の使用可能なテキスト値は、次のように。
  
- OK
    
- 更新不可
    
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetStreamingEvents の操作](getstreamingevents-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

