---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: ParentFolderId 要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832687"
---
# <a name="parentfolderid"></a>ParentFolderId

**ParentFolderId**要素は、アイテムまたはフォルダーを含む親フォルダーの識別子を表します。 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

**FolderIdType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |Exchange ストア内のフォルダーを識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|**変更キー** <br/> |**Id**属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |メールボックスの予定表フォルダーを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |メールボックス内の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |メールボックス内の連絡先アイテムを表します。  <br/> |
|[メッセージ](contactsfolder.md) <br/> |メールボックスの連絡先フォルダーを表します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーのコピー先のイベントを表します。  <br/> |
|[CreatedEvent](createdevent.md) <br/> |アイテムまたはフォルダーが作成されているイベントを表します。  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |アイテムまたはフォルダーが削除されるイベントを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |メールボックス内の個人用配布リストを表します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[アイテム](item.md) <br/> |一般的な Exchange アイテムを表します。  <br/> |
|[項目 (UploadItemType)](item-uploaditemtype.md) <br/> |メールボックスにアップロードする 1 つの項目を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |メールボックスで会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |メールボックス内の会議のメッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |メールボックスで会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |メールボックスで会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |メールボックスで電子メール メッセージを表します。  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |アイテムまたはフォルダーが変更されるイベントを表します。  <br/> |
|[MovedEvent](movedevent.md) <br/> |アイテムまたはフォルダーが 1 つの親フォルダー間で移動して別の親フォルダー イベントを表します。  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |メールボックス内の新しいメール アイテムによって発生するイベントを表します。  <br/> |
|[AcceptItem](acceptitem.md) <br/> |会議出席依頼、承諾の返信を表します。  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |仮の予定を表しますが、会議出席依頼に返信します。  <br/> |
|[DeclineItem](declineitem.md) <br/> |会議出席依頼を辞退の返信を表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアから項目を削除します。  <br/> |
|[タスク](task.md) <br/> |メールボックス内の作業項目を表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Exchange ストア内のアイテムの作成者に返信が含まれています。  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。  <br/> |
|[ForwardItem](forwarditem.md) <br/> |受信者に転送するのには、Exchange ストアの項目が含まれています。  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |会議をキャンセルするために使用される応答オブジェクトを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

