---
title: 会話 (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: テーマ要素は、1 つのテーマを表します。
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759754"
---
# <a name="conversation-conversationtype"></a>会話 (ConversationType)

**テーマ**要素は、1 つのテーマを表します。 
  
[FindConversationResponse](findconversationresponse.md)
  
[スレッド](conversations-ex15websvcsotherref.md)
  
[会話 (ConversationType)](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 **ConversationType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |スレッドの識別子を表します。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話のトピックを表します。 この要素は、読み取り専用です。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |特定のフォルダーから集約された会話の宛先のリストが含まれています。 この要素は、読み取り専用です。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス間で集計する対話の受信者のリストが含まれています。 この要素は、読み取り専用です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。 この要素は、読み取り専用です。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストが含まれています。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |会話項目を現在のフォルダー内のすべての送信者の一覧が含まれています。 この要素は、読み取り専用です。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |現在のフォルダーには、この会話の最後に受信したメッセージの配信時刻が含まれています。  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |現在のフォルダー内のすべての会話項目に適用されるカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話項目のカテゴリの一覧が含まれています。  <br/> |
|[フラグ](flagstatus.md) <br/> |テーマ フォルダー内のアイテムの現在の集計のフラグの状態が含まれています。  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |メールボックス内のすべての会話項目の集計のフラグの状態が含まれています。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |添付ファイルを現在のフォルダーに項目を少なくとも 1 つのテーマがあるかどうかを示す値が含まれています。  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |メールボックス内の少なくとも 1 つのテーマのアイテムに添付ファイルがあるかどうかを示す値が含まれています。  <br/> |
|[MessageCount](messagecount.md) <br/> |現在のフォルダー内の会話の項目の合計数が含まれています。  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |会話メールボックス内のアイテムの合計数が含まれています。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |フォルダー内のアイテムを未読の会話の数が含まれています。  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |メールボックス内のすべての未読の会話項目の数が含まれています。  <br/> |
|[Size](size.md) <br/> |現在のフォルダー内のすべての会話項目のサイズから計算された会話のサイズが含まれています。  <br/> |
|[GlobalSize](globalsize.md) <br/> |メールボックス内のすべての会話アイテムのサイズから計算された会話のサイズが含まれています。  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |会話の項目の現在のフォルダーのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |会話内のアイテムをメールボックスのすべてのアイテム クラスを表す項目のクラスのリストが含まれています。  <br/> |
|[Importance](importance.md) <br/> |集計の重要性現在のフォルダー内のすべての会話項目にはが含まれています。  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |メールボックス内のすべての会話項目の集計の重要性が含まれています。  <br/> |
|[Itemid](itemids.md) <br/> |現在のフォルダー内のすべての会話項目の項目の識別子のコレクションが含まれています。  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[スレッド](conversations-ex15websvcsotherref.md) <br/> |**FindConversation**の応答で返される会話の配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。
  
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

