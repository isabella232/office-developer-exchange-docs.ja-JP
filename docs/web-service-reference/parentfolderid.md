---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: ParentFolderId 要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。
ms.openlocfilehash: 6075e7aade7a05aad965efb95b326a2f1effb4bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534831"
---
# <a name="parentfolderid"></a>ParentFolderId

**ParentFolderId** 要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

**FolderIdType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |フォルダー ストア内のフォルダーを識別する文字列Exchangeします。 この属性は必須です。  <br/> |
|**ChangeKey** <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が **含** まれます。 この属性は省略可能です。 フォルダーの正しいバージョンが使用されていることを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |メールボックス内の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |メールボックス内の連絡先アイテムを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されるイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |メールボックス内のプライベート配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[項目](item.md) <br/> |アイテムの一般的なExchangeを表します。  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする 1 つのアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |メールボックス内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |メールボックス内の会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |メールボックス内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |メールボックス内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |メールボックス内の電子メール メッセージを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されたイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |ある親フォルダーから別の親フォルダーにアイテムまたはフォルダーを移動するイベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによってトリガーされるイベントを表します。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼に対する Accept 返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |会議出席依頼に対する仮返信を表します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼に対する辞退の返信を表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムをストアからExchangeします。  <br/> |
|[タスク](task.md) <br/> |メールボックス内のタスク アイテムを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |ストア内のアイテムの作成者への返信Exchangeします。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |アイテムストア内のアイテムの識別された受信者全員に対する返信Exchangeします。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送Exchangeストア アイテムを格納します。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議のキャンセルに使用される応答オブジェクトを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

