---
title: Contact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Contact 要素は、連絡先ストア内の連絡先Exchangeします。
ms.openlocfilehash: a91d8cab7db0bfe0cc102aa75d51df5b60603a77
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543542"
---
# <a name="contact"></a>Contact

**Contact 要素** は、連絡先ストア内の連絡先Exchangeします。 
  
```XML
<Contact>
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
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 **ContactItemType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |base64Binary 形式で表されるオブジェクトのネイティブの Multipurpose Internet Mail Extensions (MIME) ストリームを含みます。  <br/> |
|[ItemId](itemid.md) <br/> |ストア内のアイテムの一意の識別子と変更キー Exchangeします。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[[件名]](subject.md) <br/> |アイテムと応答オブジェクトを格納Exchangeの件名を表します。  <br/> |
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
|[DisplayTo](displayto.md) <br/> |To 行の内容に使用される表示文字列を表します。 これは、すべての宛先受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに表示される添付ファイルが 1 つ以上ある場合に **true** に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを変更する最後のユーザーの表示名を格納します。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Web App エンドポイントに連結する URL をMicrosoft Office Outlookし、Web App エンドポイントでアイテムを読み取Outlook Web App。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |エンドポイントに連結する URL を表し、Outlook Web App内のアイテムを編集Outlook Web App。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子を含む。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーン テキストを表します。  <br/> |
|[FileAs](fileas.md) <br/> |連絡先フォルダーに連絡先をファイルする方法を表します。  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |連絡先に対して表示される情報を作成する方法を定義します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |連絡先の表示名を定義します。  <br/> |
|[GivenName](givenname.md) <br/> |連絡先の指定された名前が含まれる。  <br/> |
|[[頭文字](initials.md)] <br/> |連絡先のイニシャルを表します。  <br/> |
|[MiddleName](middlename.md) <br/> |連絡先のミドルネームを表します。  <br/> |
|[ニックネーム](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[CompleteName](completename.md) <br/> |連絡先の完全な名前を表します。  <br/> |
|[CompanyName](companyname.md) <br/> |連絡先に関連付けられている会社名を表します。  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |連絡先の電子メール アドレスのコレクションを表します。  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |連絡先に関連付けられている物理アドレスのコレクションが含まれます。  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |連絡先の電話番号のコレクションを表します。  <br/> |
|[AssistantName](assistantname.md) <br/> |連絡先のアシスタントを表します。  <br/> |
|[Birthday](birthday.md) <br/> |連絡先の生年月日を表します。  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |連絡先のホーム ページ (Web アドレス) を表します。  <br/> |
|[Children](children.md) <br/> |連絡先の子の名前が含まれる。  <br/> |
|[Companies](companies.md) <br/> |連絡先に関連付けられている会社のコレクションを表します。  <br/> |
|[ContactSource](contactsource.md) <br/> |連絡先が連絡先ストアまたは Active Directory ディレクトリ Exchangeに存在するかどうかを説明します。  <br/> |
|[Department](department.md) <br/> |仕事中の連絡先の部署を表します。  <br/> |
|[ジェネレーション](generation.md) <br/> |連絡先の完全な名前に従う世代の省略形を表します。  <br/> |
|[ImAddresses](imaddresses.md) <br/> |連絡先のインスタント メッセージング アドレスのコレクションを表します。  <br/> |
|[JobTitle](jobtitle.md) <br/> |連絡先の役職を表します。  <br/> |
|[Manager](manager.md) <br/> |連絡先のマネージャーを表します。  <br/> |
|[Mileage](mileage.md) <br/> |連絡先アイテムのマイレージを表します。  <br/> |
|[OfficeLocation](officelocation.md) <br/> |連絡先のオフィスの場所を表します。  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |物理アドレスの表示の種類を表します。  <br/> |
|[Profession](profession.md) <br/> |連絡先の専門職を表します。  <br/> |
|[SpouseName](spousename.md) <br/> |連絡先の配偶者/パートナーの名前を表します。  <br/> |
|[姓](surname.md) <br/> |連絡先の姓を表します。  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |連絡先の結婚記念日が含まれる。  <br/> |
|[HasPicture](haspicture.md) <br/> |連絡先アイテムに連絡先の画像を表す添付ファイルが含されているかどうかを示します。  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |連絡先の完全な名前 (名前と名を含む) が、読み上がり形式で表示されます。  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |連絡先の最初の名前を含み、スペルは電話で入力されます。  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |連絡先の最後の名前を含み、スペルは電話で入力されます。  <br/> |
|[Alias](alias.md) <br/> |連絡先の電子メール エイリアスが含まれる。  <br/> |
|[Notes (Contact)](notes-contact.md) <br/> |補足的な連絡先情報が含まれる。  <br/> |
|[写真](photo.md) <br/> |連絡先の写真をエンコードする値を含む。  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |連絡先の SMIME 証明書をエンコードする値を含んでいます。  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |連絡先の Microsoft 証明書をエンコードExchange値を含む。  <br/> |
|[DirectoryId](directoryid.md) <br/> |連絡先のディレクトリ ID が含まれます。  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |連絡先のマネージャー メールボックスを識別する SMTP 情報が含まれる。  <br/> |
|[DirectReports](directreports.md) <br/> |連絡先の直接レポートを識別する SMTP 情報が含まれる。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議時間に隣接しているすべての予定表アイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |UpdateItem 操作中にアイテムまたはフォルダーの 1 つのプロパティに追加する [データを識別します](updateitem-operation.md)。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議時間と競合しているすべてのアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別のアイテムExchange付けられたアイテムを表Exchangeします。  <br/> |
|[Items](items.md) <br/> |アイテムの配列を含む。  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列を格納します。  <br/> |
|[解決策](resolution.md) <br/> |1 つの解決済みエンティティを含む。  <br/> |
|[SetItemField](setitemfield.md) <br/> |UpdateItem 操作内のアイテムの 1 つのプロパティへの更新 [を表します](updateitem-operation.md)。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つのアイテムを識別します。  <br/> |
   
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
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)


[連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[連絡先の削除](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

