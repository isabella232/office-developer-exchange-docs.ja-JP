---
title: DistributionList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistributionList
api_type:
- schema
ms.assetid: f65aea01-e870-44a2-8571-fa6c001341cc
description: DistributionList 要素は配布リストを表します。
ms.openlocfilehash: 1ca198543c6da62827f2f2b0fe2b7ec9c7e79615
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545273"
---
# <a name="distributionlist"></a>DistributionList

**DistributionList 要素** は配布リストを表します。 
  
```xml
<DistributionList>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <DisplayName/>
   <FileAs/>
   <ContactSource/>
   <Members/>
</DistributionList>
```

 **DistributionListType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |base64Binary 形式で表されるオブジェクトのネイティブ MIME ストリームを格納します。  <br/> |
|[ItemId](itemid.md) <br/> |ストア内の配布リスト アイテムの一意の識別子と変更キー Exchangeします。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |配布リスト アイテムを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |配布リスト アイテムのメッセージ クラスを表します。  <br/> |
|[[件名]](subject.md) <br/> |アイテムと応答オブジェクトを格納Exchangeの件名を表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |配布リスト アイテムの感度の状態を格納します。  <br/> |
|[Body](body.md) <br/> |配布リスト アイテムの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |ストア内の配布リスト アイテムに添付されているアイテムまたはファイルExchangeします。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内の配布リスト アイテムが受信された日時を表します。  <br/> |
|[サイズ](size.md) <br/> |配布リスト アイテムのサイズをバイト単位で表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内の配布リスト アイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |配布リスト アイテムの重要性について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが Outbox の既定のフォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーがアイテムを送信したかどうかを示します。  <br/> |
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
|[DisplayTo](displayto.md) <br/> |To 行の内容に使用される表示文字列を表します。 これは、すべての宛先受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに表示される添付ファイルが 1 つ以上ある場合に **true** に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |配布リスト アイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の配布リスト アイテムのカルチャを表します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを変更する最後のユーザーの表示名を格納します。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Web App エンドポイントに連結する URL をMicrosoft Office Outlookし、Web App エンドポイントでアイテムを読み取Outlook Web App。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |エンドポイントに連結する URL を表し、Outlook Web App内のアイテムを編集Outlook Web App。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子を含む。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーン テキストを表します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |配布リストの表示名を定義します。  <br/> |
|[FileAs](fileas.md) <br/> |連絡先フォルダーに配布リストをファイルする方法を表します。  <br/> |
|[ContactSource](contactsource.md) <br/> |連絡先がドメイン ストアまたは Active Directory ドメイン サービス (Exchange DS) にあるかどうかをADします。  <br/> |
|[Members (MemberListType)](members-memberlisttype.md) <br/> |配布リストのメンバーの一覧を含む。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議時間に隣接しているすべての予定表アイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |UpdateItem 操作中に配布リストの 1 つのプロパティに追加する [データを識別します](updateitem-operation.md)。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議時間と競合するアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つの配布リストを識別します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つの配布リストを識別します。  <br/> |
|[Items](items.md) <br/> |アイテムの配列を含む。  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダーに作成するアイテムの配列を格納します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作で配布リスト アイテムの 1 つのプロパティへの更新 [を表します](updateitem-operation.md)。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

