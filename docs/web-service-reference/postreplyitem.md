---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: PostReplyItem 要素には、投稿するアイテムへの返信が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 70a0d6a7c670d0f16a55e66e7ef329331a04a5f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832868"
---
# <a name="postreplyitem"></a>PostReplyItem

**PostReplyItem**要素には、投稿するアイテムへの返信が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。 
  
```xml
<PostReplyItem>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
      <NewBodyContent/>
</PostReplyItem>
```

 **PostReplyItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。 このプロパティは値の取得のみ可能です。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[Subject](subject.md) <br/> |Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。 件名は、255 文字までに制限されています。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度レベルを示します。  <br/> |
|[Body/本文](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムを受信したときの日時を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのバイト単位のサイズを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要性をについて説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムの返信するアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムはまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日時を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日時を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生したときの日時を表します。 [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストアのアイテムのアラームが設定されたかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |分前にアラームが表示されるときに、イベントの数を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] 行の内容のために使用される表示文字列を表します。 これは、すべての Cc 受信者の表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |ボックスの内容のために使用される表示文字列を表します。 これは、すべての受信者の表示名の連結された文字列です。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |アイテムに添付ファイルがある場合に**true**に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
|[カルチャ](culture.md) <br/> |メールボックス内の指定したアイテムのカルチャを表します。  <br/> |
|[送信者](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[ToRecipients](torecipients.md) <br/> |一連メッセージの受信者にはが含まれています。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受け取る受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |アイテムの送信者が開封確認メッセージを要求するかどうかを示します。  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |アイテムの送信者が配信済みメッセージを要求するかどうかを示します。  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |このメッセージが属するスレッドを表すバイナリの ID が含まれています。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話 id を表します。  <br/> |
|[From](from.md) <br/> |メッセージの送信元アドレスを表します。  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |アイテムのインターネット メッセージ id を表します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが読み取られたかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |電子メール メッセージへの応答が要求されたかどうかを示します。  <br/> |
|[参照資料](references.md) <br/> |元のメッセージに応答を関連付けるために使用する Usenet ヘッダーを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |応答を送信するアドレスのセットを識別します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセス シナリオでは、デリゲートを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセスのシナリオでプリンシパルを識別します。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |新しい投稿アイテムの本文の内容を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての項目について説明します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべての項目について説明します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

