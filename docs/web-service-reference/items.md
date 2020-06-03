---
title: アイテム
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: Items 要素には、項目の配列が含まれています。
ms.openlocfilehash: 489e34ad0e4bcc2520febb3c213db970fa496051
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458132"
---
# <a name="items"></a>アイテム

**Items**要素には、項目の配列が含まれています。 
  
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
|[Item](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |[Copyitem 操作](copyitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |単一の[CreateItem 操作](createitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |[GetItem 操作](getitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[GroupedItems](groupeditems.md) <br/> |グループ化された[FindItem 操作](finditem-operation.md)呼び出しの結果であるアイテムのコレクションを表します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |[Moveitem 操作](moveitem-operation.md)要求の状態と結果を格納します。  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |[FindItem 操作](finditem-operation.md)中の1つのルートフォルダの検索結果を格納します。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |[Updateitem 操作](updateitem-operation.md)要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

[CreateItem 操作](createitem-operation.md)要求のアイテムセットの詳細については、「 [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)」を参照してください。
  
[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージ、および Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。 IPM などのアイテム。共有と IPM. InfoPath は、**メッセージ**要素として返されます。 Exchange Server 2010 以降のバージョンの Exchange では、応答で基本[アイテム](item.md)要素は返されません。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
  
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

