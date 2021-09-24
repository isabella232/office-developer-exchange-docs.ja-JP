---
title: アイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Items 要素には、アイテムの配列が含まれています。
ms.openlocfilehash: b6e9db6524640098a902f431393fccd6bd4e8868
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540888"
---
# <a name="items"></a>アイテム

**Items 要素** には、アイテムの配列が含まれています。 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 **ArrayOfRealItemsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |ストア内のアイテムをExchangeします。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |電子メール メッセージExchangeを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[Contact](contact.md) <br/> |連絡先アイテムExchangeを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議ストア内の会議メッセージExchangeします。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議ストアの会議の応答Exchangeします。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議ストアでの会議の取り消しExchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
|[PostItem](postitem.md) <br/> |ストア内の投稿アイテムをExchangeします。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |CopyItem 操作要求の状態と結果 [を格納](copyitem-operation.md) します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |1 つの CreateItem 操作要求の状態と [結果を格納](createitem-operation.md) します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |GetItem 操作要求の状態と [結果を格納](getitem-operation.md) します。  <br/> |
|[GroupedItems](groupeditems.md) <br/> |グループ化された FindItem 操作呼び出しの結果であるアイテムの [コレクションを表](finditem-operation.md) します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |MoveItem 操作要求の状態と結果 [を格納](moveitem-operation.md) します。  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |FindItem 操作中に 1 つのルート フォルダーを検索した結果 [を格納します](finditem-operation.md)。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |UpdateItem 操作要求の状態と [結果を格納](updateitem-operation.md) します。  <br/> |
   
## <a name="remarks"></a>注釈

[CreateItem](createitem-operation.md)操作要求内のアイテムのセットの詳細については[、「Items (NonEmptyArrayOfAllItemsType)」を参照してください](items-nonemptyarrayofallitemstype.md)。
  
[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージと、Web サービス (EWS) スキーマによって強く入力されていない他のすべてのExchangeを表します。 IPM などのアイテム。共有と IPM.InfoPath は Message 要素として **返** されます。 2010 Exchangeから始まるExchange Serverのバージョンは、応答で[base Item](item.md)要素を返す必要があります。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
  
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

