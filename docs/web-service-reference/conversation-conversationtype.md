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
description: 会話要素は、単一の会話を表します。
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458937"
---
# <a name="conversation-conversationtype"></a>会話 (ConversationType)

**会話**要素は、単一の会話を表します。 
  
[FindConversationResponse](findconversationresponse.md)
  
[会話](conversations-ex15websvcsotherref.md)
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ConversationId](conversationid.md) <br/> |会話の識別子を表します。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話のトピックを表します。 この要素は値の取得のみ可能です。  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |特定のフォルダーから集約された会話の受信者の一覧が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |メールボックス全体で集約された会話の受信者の一覧が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |現在のフォルダーで、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |メールボックス内のすべてのフォルダーにわたって、この会話で現在未読のメッセージを送信したすべてのユーザーの一覧が含まれています。  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |現在のフォルダー内のスレッドアイテムのすべての送信者の一覧が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |メールボックス内のスレッドアイテムのすべての送信者の一覧が含まれています。  <br/> |
|[LastDeliveryTime](lastdeliverytime.md) <br/> |現在のフォルダーで、このスレッドで最後に受信したメッセージの配信時刻を含みます。  <br/> |
|[GlobalLastDeliveryTime](globallastdeliverytime.md) <br/> |メールボックス内のすべてのフォルダーにわたって、この会話で最後に受信したメッセージの配信時刻を含みます。  <br/> |
|[カテゴリ](categories-ex15websvcsotherref.md) <br/> |現在のフォルダー内のすべての会話アイテムに適用されるカテゴリを識別する文字列のコレクションが含まれています。  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |メールボックス内のすべての会話アイテムのカテゴリリストが保存されています。  <br/> |
|[FlagStatus](flagstatus.md) <br/> |現在のフォルダー内のスレッドアイテムの集約フラグの状態を含みます。  <br/> |
|[GlobalFlagStatus](globalflagstatus.md) <br/> |メールボックス内のすべての会話アイテムの集約フラグの状態を格納します。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |現在のフォルダー内の1つ以上の会話アイテムに添付ファイルがあるかどうかを示す値を格納します。  <br/> |
|[GlobalHasAttachments](globalhasattachments.md) <br/> |メールボックス内の少なくとも1つの会話アイテムに添付ファイルがあるかどうかを示す値を格納します。  <br/> |
|[MessageCount](messagecount.md) <br/> |現在のフォルダー内の会話アイテムの合計数が含まれます。  <br/> |
|[GlobalMessageCount](globalmessagecount.md) <br/> |メールボックス内の会話アイテムの合計数が含まれます。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |フォルダー内の未読の会話アイテムの数が含まれます。  <br/> |
|[GlobalUnreadCount](globalunreadcount.md) <br/> |メールボックス内のすべての未開封の会話アイテムの数を含みます。  <br/> |
|[[サイズ]](size.md) <br/> |現在のフォルダー内のすべての会話アイテムのサイズから計算された会話のサイズを格納します。  <br/> |
|[GlobalSize](globalsize.md) <br/> |メールボックス内のすべての会話アイテムのサイズによって計算された会話のサイズを含みます。  <br/> |
|[ItemClasses (ArrayOfItemClassType)](itemclasses-arrayofitemclasstype.md) <br/> |現在のフォルダー内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれます。  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |メールボックス内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれています。  <br/> |
|[Importance](importance.md) <br/> |現在のフォルダー内のすべての会話アイテムの集約された重要度を含みます。  <br/> |
|[GlobalImportance](globalimportance.md) <br/> |メールボックス内のすべての会話アイテムの集約された重要度を含みます。  <br/> |
|[ItemIds](itemids.md) <br/> |現在のフォルダー内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[会話](conversations-ex15websvcsotherref.md) <br/> |**Findconversation**応答で返されるスレッドの配列を格納します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[FindConversation 操作](findconversation-operation.md)
  
[ApplyConversationAction 操作](applyconversationaction-operation.md)


[EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

