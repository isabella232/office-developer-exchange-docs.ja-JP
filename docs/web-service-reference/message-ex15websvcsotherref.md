---
title: メッセージ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 2400b33c-43b2-4fc2-b6fb-275a99e0e810
description: Message 要素は、Microsoft Exchange の電子メールメッセージを表します。
ms.openlocfilehash: 510e97572e54f0ea0cb65fc7c75910e69cc0651f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467782"
---
# <a name="message"></a>メッセージ

**Message**要素は、Microsoft Exchange の電子メールメッセージを表します。 
  
```xml
<Message>
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
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <ReminderMessageData/>
</Message>
```

 **MessageType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージクラスを表します。  <br/> |
|[件名](subject.md) <br/> |Exchange ストアアイテムおよび応答オブジェクトの件名を表します。 件名は255文字に制限されます。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度レベルを示します。  <br/> |
|[Body](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムが受信された日付と時刻を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのサイズ (バイト単位) を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要度について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分にアイテムを送信したかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前に送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテム内に含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日付と時刻を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日付と時刻を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日付と時刻を表します。 これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の時間 (分単位) を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[CC] 行の内容として使用される表示文字列を表します。 これは、すべての CC 受信者表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |[宛先] ボックスの内容に対して使用される表示文字列を表します。 これは、すべての受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[Sender](sender.md) <br/> |アイテムの送信者を識別します。  <br/> |
|[ToRecipients](torecipients.md) <br/> |メッセージの受信者のセットが含まれています。  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |メッセージのコピーを受信する受信者のコレクションを表します。  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |電子メールメッセージのブラインドカーボンコピー (Bcc) を受信する受信者のコレクションを表します。  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |アイテムの送信者が開封確認メッセージを要求するかどうかを示します。  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |アイテムの送信者が配信確認を要求するかどうかを示します。  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |このメッセージが属しているスレッドを表すバイナリ ID を含みます。  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |会話識別子を表します。  <br/> |
|[From](from.md) <br/> |メッセージが送信された相手のアドレスを表します。  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |アイテムのインターネットメッセージ識別子を表します。  <br/> |
|[IsRead](isread.md) <br/> |メッセージが開封されたかどうかを示します。  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |電子メールメッセージに対する応答が要求されているかどうかを示します。  <br/> |
|[References](references.md) <br/> |返信と元のメッセージを相互に関連付けるために使用される Usenet ヘッダーを表します。  <br/> |
|[ReplyTo](replyto.md) <br/> |返信を送信する宛先のアドレスのセットを指定します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[ReceivedBy](receivedby.md) <br/> |代理人アクセスシナリオの代理人を識別します。  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |代理人アクセスシナリオのプリンシパルを識別します。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを最後に変更したユーザーの表示名を含みます。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。  <br/> |
|[ReminderMessageData](remindermessagedata.md) <br/> |事前通知メッセージのデータが保存されています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表アイテムを説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべてのアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカルクライアントストアに作成する単一のアイテムを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別の Exchange アイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列を格納します。  <br/> |
|[アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカルクライアントストアで更新する単一のアイテムを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

別の**message**要素[message (availability)](message-availability.md)は、空き時間情報の操作が OOF メッセージを返すために使用されます。 
  
[Message](message-ex15websvcsotherref.md)要素は、電子メールメッセージ、および Exchange Web サービス (EWS) スキーマで厳密に型指定されていないその他すべてのアイテムを表します。 IPM などのアイテム。共有と IPM. InfoPath は、**メッセージ**要素として返されます。 Exchange 2010 は、応答で基本**Item**要素を返しません。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

