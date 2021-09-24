---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: GlobalLastDeliveryTime 要素には、メールボックス内のすべてのフォルダーでこの会話で最後に受信したメッセージの配信時間が含まれます。
ms.openlocfilehash: f012c11ec2a30680d1f6a851a4c3f3f6fc94a824
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539810"
---
# <a name="globallastdeliverytime"></a>GlobalLastDeliveryTime

**GlobalLastDeliveryTime** 要素には、メールボックス内のすべてのフォルダーでこの会話で最後に受信したメッセージの配信時間が含まれます。 
  
[FindConversationResponse](findconversationresponse.md)
  
[会話](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[GlobalLastDeliveryTime](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 **xs:dateTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**GlobalLastDeliveryTime** 要素のテキスト値は、メールボックス内のすべてのフォルダーでこの会話で最後に受信されたメッセージの日時です。 
  
## <a name="remarks"></a>注釈

この要素は、2010 Exchange Server Service Pack 1 (SP1) で導入されました。この要素を記述するスキーマは、Web サービスをホストする IIS 仮想Exchangeにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)
  
[ApplyConversationAction 操作](applyconversationaction-operation.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

