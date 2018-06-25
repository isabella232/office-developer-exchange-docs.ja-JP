---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: GlobalLastDeliveryTime 要素には、メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。
ms.openlocfilehash: fded5cd1891a406f0979cf4bec7321779d70ab3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831733"
---
# <a name="globallastdeliverytime"></a>GlobalLastDeliveryTime

**GlobalLastDeliveryTime**要素には、メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。 
  
[FindConversationResponse](findconversationresponse.md)
  
[スレッド](conversations-ex15websvcsotherref.md)
  
[会話 (ConversationType)](conversation-conversationtype.md)
  
[GlobalLastDeliveryTime](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 **xs:dateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |1 つのテーマを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**GlobalLastDeliveryTime**要素のテキスト値とは、メッセージ、メールボックス内のすべてのフォルダーをこの会話に受信した最後の日時です。 
  
## <a name="remarks"></a>備考

この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [FindConversation 操作](findconversation-operation.md)
  
[ApplyConversationAction 操作](applyconversationaction-operation.md)


[EWS での会話](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

