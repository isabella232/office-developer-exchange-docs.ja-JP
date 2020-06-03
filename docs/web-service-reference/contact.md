---
title: Contact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Contact 要素は、Exchange ストア内の連絡先アイテムを表します。
ms.openlocfilehash: b5b4af211815dbbd09449ca2f3c6b6b2dfba6f93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44445651"
---
# <a name="contact"></a>Contact

**Contact**要素は、Exchange ストア内の連絡先アイテムを表します。 
  
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
|[MimeContent](mimecontent.md) <br/> |Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージクラスを表します。  <br/> |
|[件名](subject.md) <br/> |Exchange ストアアイテムおよび応答オブジェクトの件名を表します。  <br/> |
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
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日付と時刻を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日付と時刻を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日付と時刻を表します。 これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の時間 (分単位) を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] 行の内容として使用される表示文字列を表します。 これは、すべての Cc 受信者表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |To 行の内容として使用される表示文字列を表します。 これは、すべての受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを最後に変更したユーザーの表示名を含みます。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。  <br/> |
|[FileAs](fileas.md) <br/> |連絡先フォルダーに連絡先をファイリングする方法を表します。  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |連絡先に対して表示される内容を作成する方法を定義します。  <br/> |
|[DisplayName (文字列)](displayname-string.md) <br/> |連絡先の表示名を定義します。  <br/> |
|[GivenName](givenname.md) <br/> |連絡先の特定の名前が含まれています。  <br/> |
|[[頭文字](initials.md)] <br/> |連絡先のイニシャルを表します。  <br/> |
|[MiddleName](middlename.md) <br/> |連絡先のミドルネームを表します。  <br/> |
|[ニックネーム](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[CompleteName](completename.md) <br/> |連絡先の完全な名前を表します。  <br/> |
|[CompanyName](companyname.md) <br/> |連絡先に関連付けられている会社名を表します。  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |連絡先の電子メールアドレスのコレクションを表します。  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |連絡先に関連付けられている物理的な住所のコレクションを格納します。  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |連絡先の電話番号のコレクションを表します。  <br/> |
|[AssistantName](assistantname.md) <br/> |連絡先のアシスタントを表します。  <br/> |
|[Birthday](birthday.md) <br/> |連絡先の生年月日を表します。  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |連絡先のホームページ (Web アドレス) を表します。  <br/> |
|[Children](children.md) <br/> |連絡先の子の名前を格納します。  <br/> |
|[Companies](companies.md) <br/> |連絡先に関連付けられている会社のコレクションを表します。  <br/> |
|[ContactSource](contactsource.md) <br/> |連絡先が Exchange ストアまたは Active Directory ディレクトリサービスに存在するかどうかを示します。  <br/> |
|[Department](department.md) <br/> |作業中の連絡先の部署を表します。  <br/> |
|[ジェネレーター](generation.md) <br/> |連絡先の氏名の後の省略形を表します。  <br/> |
|[ImAddresses](imaddresses.md) <br/> |連絡先のインスタントメッセージアドレスのコレクションを表します。  <br/> |
|[JobTitle](jobtitle.md) <br/> |連絡先の役職を表します。  <br/> |
|[Manager](manager.md) <br/> |連絡先の上司を表します。  <br/> |
|[Mileage](mileage.md) <br/> |連絡先アイテムのマイレージを表します。  <br/> |
|[OfficeLocation](officelocation.md) <br/> |連絡先の勤務先の場所を表します。  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |物理アドレスの表示の種類を表します。  <br/> |
|[Profession](profession.md) <br/> |連絡先の職業を表します。  <br/> |
|[SpouseName](spousename.md) <br/> |連絡先の配偶者またはパートナーの名前を表します。  <br/> |
|[姓](surname.md) <br/> |連絡先の姓を表します。  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |連絡先の結婚記念日を含みます。  <br/> |
|[HasPicture](haspicture.md) <br/> |連絡先アイテムに、連絡先の写真を表す添付ファイルがあるかどうかを示します。  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |連絡先の氏名を含み、姓と名のスペルを入力します。  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |連絡先の名の先頭にスペルを入力します。  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |連絡先の姓が入力されています。  <br/> |
|[Alias](alias.md) <br/> |連絡先の電子メールエイリアスが保存されています。  <br/> |
|[メモ (連絡先)](notes-contact.md) <br/> |補足連絡先情報が含まれています。  <br/> |
|[写真](photo.md) <br/> |連絡先の写真をエンコードする値を格納します。  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |連絡先の SMIME 証明書をエンコードする値を格納します。  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |連絡先の Microsoft Exchange 証明書をエンコードする値を格納します。  <br/> |
|[DirectoryId](directoryid.md) <br/> |連絡先のディレクトリ ID を格納します。  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |連絡先のマネージャーメールボックスを識別する SMTP 情報を含みます。  <br/> |
|[DirectReports](directreports.md) <br/> |連絡先の直属の部下を識別する SMTP 情報を含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表アイテムを説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテムまたはフォルダーの1つのプロパティに追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべてのアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカルクライアントストアに作成する1つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別の Exchange アイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列を格納します。  <br/> |
|[アイテム (非 Emptyarrayofallitemstype)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素によって識別されるフォルダー内に作成するアイテムの配列が含まれています。  <br/> |
|[Resolution](resolution.md) <br/> |1つの解決済みエンティティを含みます。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカルクライアントストアで更新する単一のアイテムを識別します。  <br/> |
   
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
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)


[連絡先の作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[連絡先の更新](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[連絡先の削除](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

