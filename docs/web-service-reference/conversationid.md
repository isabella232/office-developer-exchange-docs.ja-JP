---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: ConversationId 要素には、アイテムまたは会話の識別子が含まれる。
ms.openlocfilehash: 345c7c692576abb8c1e1b9848b005ca3d0c0fa0f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547541"
---
# <a name="conversationid"></a>ConversationId

**ConversationId 要素** には、アイテムまたは会話の識別子が含まれる。 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |ストア内の特定のアイテムExchangeします。  <br/> |
|**ChangeKey** <br/> | アイテムの特定のバージョンを識別します。 次 **のシナリオでは、ChangeKey** が必要です。  <br/><br/>- **ConflictResolution** 属性が **AutoResolve** に設定されている場合 [、UpdateItem](updateitem.md)要素には ChangeKey が必要です。 AutoResolve は既定値です。 **ChangeKey 属性が** 含まれていない場合、応答は **ErrorChangeKeyRequired** と等しい [ResponseCode](responsecode.md)値を返します。<br/><br/>- [SendItem](senditem.md)要素 [、DeleteItem](deleteitem.md)要素、 [および DeleteFolder](deletefolder.md) 要素では、試行された操作がアイテムの最新バージョンで動作するかどうかをテストするために **ChangeKey** が必要です。 **ChangeKey 属性が ItemId** に含まれていない場合、または **ChangeKey** が空の場合、応答は ErrorStaleObject に等しい [ResponseCode](responsecode.md)値 **を返します**。   <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[ConversationAction](conversationaction.md) <br/> |1 つの会話に適用する 1 つのアクションを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[項目](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[PostItem](postitem.md) <br/> |ストア内の投稿アイテムをExchangeします。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindConversation 操作](findconversation-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

