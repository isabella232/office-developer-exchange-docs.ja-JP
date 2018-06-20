---
title: ApplyConversationActionResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponse
api_type:
- schema
ms.assetid: 682d47a6-f9fe-4cc6-a56c-c5db835d5ec6
description: ApplyConversationActionResponse 要素は、ApplyConversationAction の操作要求に対する応答を定義します。
ms.openlocfilehash: 39f7344596de7376e770ed98dbe372a590057deb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759412"
---
# <a name="applyconversationactionresponse"></a>ApplyConversationActionResponse

**ApplyConversationActionResponse**要素は、 [ApplyConversationAction 操作](applyconversationaction-operation.md)要求への応答を定義します。 
  
[ApplyConversationActionResponse](applyconversationactionresponse.md)
  
```XML
<ApplyConversationActionResponse>
   <ResponseMessages/>
</ApplyConversationActionResponse>
```

 **ApplyConversationActionResponseType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Exchange Web サービス要求に対する応答メッセージが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

なし。
  
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

