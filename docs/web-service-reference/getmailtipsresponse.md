---
title: GetMailTipsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: GetMailTipsResponse 要素は、GetMailTips 操作の応答メッセージを表します。
ms.openlocfilehash: e7a18e8818761af931d32b26aeaf58a2853fa684
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760787"
---
# <a name="getmailtipsresponse"></a>GetMailTipsResponse

**GetMailTipsResponse**要素は、 [GetMailTips 操作](getmailtips-operation.md)の応答メッセージを表します。
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 **GetMailTipsResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages (ArrayOfMailTipsResponseMessageType)](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |メール ヒントの応答メッセージの一覧を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMailTips 操作](getmailtips-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

