---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: UniqueRecipients 要素には、特定のフォルダー内のスレッドの受信者の一覧が含まれています。 この要素は値の取得のみ可能です。
ms.openlocfilehash: d7f6b0aa01aceb6a251fb0c46d89b34cad260acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530727"
---
# <a name="uniquerecipients"></a>UniqueRecipients

**UniqueRecipients**要素には、特定のフォルダー内のスレッドの受信者の一覧が含まれています。 この要素は値の取得のみ可能です。 
  
[FindConversationResponse](findconversationresponse.md)
  
[会話](conversations-ex15websvcsotherref.md)
  
[会話 (ConversationType)](conversation-conversationtype.md)
  
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
|[String](string.md) <br/> |会話の一意の受信者を表します。 この要素は値の取得のみ可能です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |単一の会話を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

