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
description: 項目要素には、項目の配列が含まれています。
ms.openlocfilehash: 241a56ee23e87d6a4320b93cc65b1f5aa1f60120
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832163"
---
# <a name="items"></a>アイテム

**項目**要素には、項目の配列が含まれています。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Item](item.md) <br/> |Exchange ストア内の項目を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議のメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |[CopyItem 操作](copyitem-operation.md)要求の結果ステータスを格納します。  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateItem 操作](createitem-operation.md)を要求します。  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |[GetItem 操作](getitem-operation.md)要求の結果ステータスを格納します。  <br/> |
|[GroupedItems](groupeditems.md) <br/> |グループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを呼び出します。  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |[MoveItem 操作](moveitem-operation.md)要求の結果ステータスを格納します。  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |[FindItem 操作](finditem-operation.md)時に単一のルート フォルダーの検索の結果が含まれています。  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |[UpdateItem 操作](updateitem-operation.md)要求の結果ステータスを格納します。  <br/> |
   
## <a name="remarks"></a>備考

[CreateItem 操作](createitem-operation.md)要求内の項目の設定方法については、 [(NonEmptyArrayOfAllItemsType) の項目](items-nonemptyarrayofallitemstype.md)を参照してください。
  
[メッセージ](message-ex15websvcsotherref.md)要素は、電子メール メッセージ、Exchange Web サービス (EWS) スキーマが厳密に型指定されない他のすべての項目を表します。 IPM などの項目です。共有し、IPM.InfoPath は、**メッセージ**の要素として返されます。 バージョンの Exchange が Exchange Server 2010 で始まるでは、応答の基本要素の[項目](item.md)は返されません。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目




  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
  
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

