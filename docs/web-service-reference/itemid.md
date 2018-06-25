---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: ItemId の要素には、Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。
ms.openlocfilehash: 9c5d71a23e1e4b77d2a50016aa4d765d872d04cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832157"
---
# <a name="itemid"></a>ItemId

**ItemId**の要素には、Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |Exchange ストア内の特定の項目を識別します。 **Id**は大文字小文字を区別します。したがって、 **Id**の間の比較は大文字小文字を区別またはバイナリをする必要があります。  <br/> |
|**変更キー** <br/> | アイテムの特定のバージョンを識別します。 <br/><br/>の**変更キー**は、次のシナリオで必要です。 <br/> <br/>- [UpdateItem](updateitem.md)要素では、自動解決する**ConflictResolution**属性が設定されている場合に、**変更キー**が必要です。 自動解決は、既定値です。 **変更キー**属性が含まれていない場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorChangeKeyRequired**に等しい。  <br/><br/>[SendItem](senditem.md)要素には、試行した操作は、項目の最新バージョンに対して機能するかどうかをテストするための**変更キー**が必要です。 **アイテム Id**の**変更キー**の属性が含まれていない場合、または**変更キー**が空の場合は、応答が値を返す[ResponseCode](responsecode.md) **ErrorStaleObject**に等しい。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるときにイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されたときにイベントを表します。  <br/> |
|[(ItemSync) を削除します。](delete-itemsync.md) <br/> |ローカル クライアント ストアで削除するのには 1 つの項目を識別します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されたときにイベントを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |状態および 1 つのメールボックス アイテムをエクスポートするのには要求の結果が含まれています。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムが最初に見つかった位置を表します。  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話項目の項目の識別子のコレクションが含まれています。  <br/> |
|[Ignore](ignore.md) <br/> |同期中にスキップする項目を識別します。  <br/> |
|[アイテム](item.md) <br/> |一般的な Exchange アイテムを表します。  <br/> |
|[項目 (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする 1 つの項目を表します。  <br/> |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新プログラムが含まれています。  <br/><br/> この要素への XPath 式は、次のようにします。 <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[Itemid](itemids.md) <br/> | アイテム、出現アイテム、および削除、送信、取得、移動、または Exchange ストア内のアイテムをコピーするに使用されるマスターの定期的なアイテムの一意の id が含まれています。 <br/> <br/>  この要素への XPath 式は、次のように。 <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[Itemid (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムが最後に見つかった位置を表します。  <br/> |
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムが変更されたときに発生するイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |1 つの親フォルダーから別の親フォルダーにアイテムが移動したときに発生するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによって発生するイベントを表します。  <br/> |
|[出現](occurrence.md) <br/> |定期的な予定表アイテムの 1 つの変更されたアイテムを表します。  <br/> |
|[PlayOnPhone (Exchange Web サービス)](playonphone-exchange-web-services.md) <br/> |電話上のアイテムの読み取り要求を表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室の一覧を識別する電子メール アドレスを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |状態および 1 つのメールボックス アイテムをアップロードするための要求の結果が含まれています。  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |1 人のユーザーの構成オブジェクトを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md) 
- 
  [FindConversation 操作](findconversation-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

