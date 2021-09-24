---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: UniqueRecipients 要素には、特定のフォルダー内の会話の受信者リストが含まれる。 この要素は読み取り専用です。
ms.openlocfilehash: d611efa7d632a07e14740bd211c4bfa796173a68
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510793"
---
# <a name="uniquerecipients"></a>UniqueRecipients

**UniqueRecipients 要素** には、特定のフォルダー内の会話の受信者リストが含まれる。 この要素は読み取り専用です。 
  
[FindConversationResponse](findconversationresponse.md)
  
[会話](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[UniqueRecipients](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 **ArrayOfStringsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[String](string.md) <br/> |会話の一意の受信者を表します。 この要素は読み取り専用です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

