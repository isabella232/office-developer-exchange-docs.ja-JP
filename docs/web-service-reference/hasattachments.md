---
title: HasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- HasAttachments
api_type:
- schema
ms.assetid: 538b7a85-11d7-4daa-8458-09b540760e8b
description: HasAttachments 要素は、アイテムに表示される添付ファイルが少なくとも 1 つある場合、または添付ファイルを持つアイテムが会話に少なくとも 1 つ含まれている場合に true に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。
ms.openlocfilehash: dea1ffdc5ae29a0bc7c585e0ebee9ed104143c53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547289"
---
# <a name="hasattachments"></a>HasAttachments

**HasAttachments** 要素は、アイテムに表示される添付ファイルが少なくとも 1 つある場合、または添付ファイルを持つアイテムが会話に少なくとも 1 つ含まれている場合に true に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 
  
```XML
<HasAttachments/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[条件](conditions.md) <br/> |満たされると、そのルールのルール アクションをトリガーする条件を表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |1 つの会話を表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[例外](exceptions.md) <br/> |受信トレイ ルールで使用可能なすべてのルール例外条件を表します。  <br/> |
|[項目](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |ユーザー ストア内の会議Exchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。 true の値 **は** 、アイテムまたは会話に表示される添付ファイルが少なくとも 1 つ含むという意味です。 false の **値は** 、アイテムまたは会話に添付ファイルがないか、非表示の添付ファイルのみを持つという意味です。 
  
## <a name="remarks"></a>注釈

**HasAttachments** プロパティは **、Boolean AllAttachmentsHidden** MAPI プロパティから計算されます。 アイテムに添付ファイルが存在しない場合 **、AllAttachmentsHidden** プロパティは存在しません。 アイテムのすべての添付ファイルが非表示の場合 **、AllAttachmentsHidden** プロパティは true **です**。 **AllAttachmentsHidden** プロパティが少なくとも 1 つの添付ファイルを持ち、少なくとも 1 つの添付ファイルが表示されている場合は false です。 アイテムの **検索、グループ化、並べ替えには、AllAttachmentsHidden** MAPI プロパティを使用します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
  
[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)

