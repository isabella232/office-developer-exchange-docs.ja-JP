---
title: Conversation (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: Conversation 要素は、1 つの会話を表します。
ms.openlocfilehash: 7ce75fad17589f4d9a3ca52bcb2041eb1d1f4d2e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515958"
---
# <a name="conversation-conversationtype"></a>Conversation (ConversationType)

**Conversation 要素は**、1 つの会話を表します。 
  
[FindConversationResponse](findconversationresponse.md)
  
[会話](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |会話の識別子を表します。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話のトピックを表します。 この要素は読み取り専用です。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |特定のフォルダーから集計された会話の受信者リストを格納します。 この要素は読み取り専用です。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス全体で集計された会話の受信者リストを格納します。 この要素は読み取り専用です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在のフォルダー内のこの会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれます。 この要素は読み取り専用です。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |メールボックス内のすべてのフォルダーで、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれます。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |現在のフォルダー内の会話アイテムのすべての送信者の一覧が含まれます。 この要素は読み取り専用です。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内の会話アイテムのすべての送信者の一覧が含まれます。  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |現在のフォルダー内のこの会話で最後に受信したメッセージの配信時間を格納します。  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |メールボックス内のすべてのフォルダーでこの会話で最後に受信したメッセージの配信時間を格納します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |現在のフォルダー内のすべての会話アイテムに適用されるカテゴリを識別する文字列のコレクションを格納します。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話アイテムのカテゴリ リストが含まれます。  <br/> |
|[FlagStatus](flagstatus.md) <br/> |現在のフォルダー内の会話アイテムの集計フラグの状態を格納します。  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |メールボックス内のすべての会話アイテムの集計フラグの状態を格納します。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |現在のフォルダーに少なくとも 1 つの会話アイテムに添付ファイルが含まれているかどうかを示す値が含まれる。  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |メールボックス内の少なくとも 1 つの会話アイテムに添付ファイルが含まれているかどうかを示す値が含まれる。  <br/> |
|[MessageCount](messagecount.md) <br/> |現在のフォルダー内の会話アイテムの総数を格納します。  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |メールボックス内の会話アイテムの総数を格納します。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |フォルダー内の未読の会話アイテムの数を格納します。  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |メールボックス内のすべての未読会話アイテムの数が含まれます。  <br/> |
|[サイズ](size.md) <br/> |現在のフォルダー内のすべての会話アイテムのサイズから計算される会話のサイズを格納します。  <br/> |
|[GlobalSize](globalsize.md) <br/> |メールボックス内のすべての会話アイテムのサイズから計算される会話のサイズを格納します。  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |現在のフォルダー内の会話アイテムのすべてのアイテム クラスを表すアイテム クラスの一覧を格納します。  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |メールボックス内の会話アイテムのすべてのアイテム クラスを表すアイテム クラスの一覧を格納します。  <br/> |
|[Importance](importance.md) <br/> |現在のフォルダー内のすべての会話アイテムの集計重要度を格納します。  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |メールボックス内のすべての会話アイテムの集計重要度が格納されます。  <br/> |
|[ItemIds](itemids.md) <br/> |現在のフォルダー内のすべての会話アイテムのアイテム識別子のコレクションを格納します。  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションを格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話](conversations-ex15websvcsotherref.md) <br/> |**FindConversation** 応答で返される会話の配列を含む。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web Services をホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
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

