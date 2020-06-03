---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: ItemId 要素には、Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。
localization_priority: Priority
ms.openlocfilehash: d5931702225c6864b1ca60a6f0753b65f65aca30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441563"
---
# <a name="itemid"></a>ItemId

**ItemId**要素には、Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |Exchange ストア内の特定のアイテムを識別します。 **Id**は大文字と小文字を区別します。そのため、 **id**間の比較には、大文字と小文字を区別するか、バイナリにする必要があります。  <br/> |
|**ChangeKey** <br/> | 特定のバージョンのアイテムを識別します。 <br/><br/>次のシナリオでは、 **Changekey**が必要です。 <br/> <br/>- **ConflictResolution**属性が自動解決に設定されている場合、 [updateitem](updateitem.md)要素には**changekey**が必要です。 自動解決は既定値です。 **Changekey**属性が含まれていない場合、応答は、 **Errorchangekeyrequired**に[等しい値を](responsecode.md)返します。  <br/><br/>- [SendItem](senditem.md)要素には、試行された操作がアイテムの最新バージョンに対して動作するかどうかをテストするための**changekey**が必要です。 **Changekey**属性が**ItemId**に含まれていない場合、または**changekey**が空の場合は、応答は**ErrorStaleObject**に等しい、応答し[た値を](responsecode.md)返します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるときのイベントを表します。  <br/> |
|[対する createdevent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されたときのイベントを表します。  <br/> |
|[削除 (ItemSync)](delete-itemsync.md) <br/> |ローカルクライアントストアで削除する単一のアイテムを識別します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されたときのイベントを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |1つのメールボックスアイテムをエクスポートする要求の状態と結果を格納します。  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |定期的な予定表アイテムの最初の出現を表します。  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |メールボックス内のすべての会話アイテムのアイテム識別子のコレクションが含まれています。  <br/> |
|[無視](ignore.md) <br/> |同期中にスキップするアイテムを識別します。  <br/> |
|[Item](item.md) <br/> |汎用の Exchange アイテムを表します。  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする単一のアイテムを表します。  <br/> |
|[ItemChange](itemchange.md) <br/> |アイテム識別子と、アイテムに適用する更新を含みます。  <br/><br/> この要素の XPath 式を次に示します。 <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Exchange ストア内のアイテムの削除、送信、取得、移動、またはコピーに使用するアイテム、オカレンスアイテム、定期的なマスターアイテムの一意の id が含まれています。 <br/> <br/>  この要素の XPath 式は次のとおりです。 <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[ItemIds (非 Emptyarrayofitemidstype)](itemids-nonemptyarrayofitemidstype.md) <br/> |メールボックスからエクスポートするアイテムを識別するアイテム識別子の配列を格納します。  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |定期的な予定表アイテムの最後の発生を表します。  <br/> |
|[メールボックス](mailbox.md) <br/> |メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[対する modifiedevent](modifiedevent.md) <br/> |アイテムが変更されたときに発生するイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |ある親フォルダーから別の親フォルダーにアイテムが移動されたときに発生するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメールアイテムによってトリガーされるイベントを表します。  <br/> |
|[発生](occurrence.md) <br/> |定期的な予定表アイテムの1つの変更されたアイテムを表します。  <br/> |
|[PlayOnPhone (Exchange Web サービス)](playonphone-exchange-web-services.md) <br/> |電話のアイテムを読み取るための要求を表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[RoomList](roomlist.md) <br/> |会議室の一覧を識別する電子メールアドレスを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |1つのメールボックスアイテムをアップロードする要求の状態と結果を格納します。  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |1つのユーザー構成オブジェクトを定義します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ExportItems 操作](exportitems-operation.md)
- [UploadItems 操作](uploaditems-operation.md) 
- [FindConversation 操作](findconversation-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

