---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: PostReplyItem 要素には、投稿アイテムへの返信が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。
ms.openlocfilehash: 657173e19d5dc1bb6a8126b62c5977d5afc1c17c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527908"
---
# <a name="postreplyitem"></a>PostReplyItem

**PostReplyItem** 要素には、投稿アイテムへの返信が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |base64Binary 形式で表されるオブジェクトのネイティブの Multipurpose Internet Mail Extensions (MIME) ストリームを含みます。  <br/> |
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[件名](subject.md) <br/> |アイテムと応答オブジェクトを格納Exchangeの件名を表します。 件名は 255 文字に制限されます。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの感度レベルを示します。  <br/> |
|[Body](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテム ストア内のアイテムに添付されているアイテムまたはファイルExchangeします。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムが受信された日時を表します。  <br/> |
|[サイズ](size.md) <br/> |アイテムのサイズをバイト単位で表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要度について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが Outbox の既定のフォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分にアイテムを送信したかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前に送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日時を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日時を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションをExchangeします。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日時を表します。 これは [、ReminderMinutesBeforeStart](reminderminutesbeforestart.md) 要素によって使用され、アラームが表示される時間を決定します。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |ユーザー ストア内のアイテムに対してアラームが設定されているかどうかをExchangeします。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の分数を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |Cc 行の内容に使用される表示文字列を表します。 これは、すべての Cc 受信者の表示名の連結文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |To ボックスの内容に使用される表示文字列を表します。 これは、すべての宛先受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに添付ファイルがある場合に **true に** 設定されているプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[Sender](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[ToRecipients](torecipients.md) <br/> |メッセージの受信者のセットが含まれる。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受信する受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールのブラインド カーボン コピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |アイテムの送信者が読み取り受領書を要求するかどうかを示します。  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |アイテムの送信者が配信レシートを要求するかどうかを示します。  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |このメッセージが属するスレッドを表すバイナリ ID を含む。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話識別子を表します。  <br/> |
|[From](from.md) <br/> |メッセージの送信先アドレスを表します。  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |アイテムのインターネット メッセージ識別子を表します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが読み取りされているかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |電子メール メッセージへの応答が要求されたかどうかを示します。  <br/> |
|[関連情報](references.md) <br/> |返信を元のメッセージに関連付ける Usenet ヘッダーを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |返信を送信するアドレスのセットを識別します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は読み取り専用です。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセス シナリオの代理人を識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセス シナリオのプリンシパルを識別します。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |投稿アイテムの新しい本文コンテンツを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議時間に隣接しているすべてのアイテムについて説明します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するアイテムについて説明します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションをExchangeします。  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

