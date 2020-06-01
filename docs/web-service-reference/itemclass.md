---
title: ItemClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClass
api_type:
- schema
ms.assetid: 56020078-50b4-4880-894a-a9f234033cfb
description: ItemClass 要素は、アイテムのメッセージクラスを表します。
ms.openlocfilehash: 31d46b2b41b4b22ca5afeb842d7b0e0d16677920
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455416"
---
# <a name="itemclass"></a>ItemClass

**Itemclass**要素は、アイテムのメッセージクラスを表します。 
  
```XML
<ItemClass/>
```

 **ItemClassType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼への返信を承諾するかを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[会話 (ConversationType)](conversation-conversationtype.md) <br/> |単一の会話を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼への返信を拒否することを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[GlobalItemClasses](globalitemclasses.md) <br/> |メールボックス内の会話アイテムのすべてのアイテムクラスを表すアイテムクラスのリストが含まれています。  <br/> |
|[アイテム](item.md) <br/> |汎用の Exchange アイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮の返信を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

アイテムの種類と一貫性のあるテキスト値が必要な場合があります。 たとえば、メッセージを作成または更新する場合は、IPM.メモまたはメッセージと一貫性のある別のクラスが必要です。 空の値は許可されていません。 ただし、アイテムを作成または更新する場合は、空の種類が有効です。
  
**Itemclass**がアイテムの種類と一致しない値に設定されている場合は、エラーが返されます。 たとえば、メッセージの**Itemclass**をタスクの**itemclass**値に設定することはできません。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

