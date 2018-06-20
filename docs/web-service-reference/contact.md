---
title: 連絡先
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
description: 連絡先の要素は、Exchange ストア内の連絡先アイテムを表します。
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759673"
---
# <a name="contact"></a>連絡先

**連絡**の要素は、Exchange ストア内の連絡先アイテムを表します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素名**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[Subject](subject.md) <br/> |Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。  <br/> |
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
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分自身にアイテムを送信するかどうかを示します。  <br/> |
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
|[DisplayTo](displayto.md) <br/> |行の内容のために使用される表示文字列を表します。 これは、すべての受信者の表示名の連結された文字列です。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
|[カルチャ](culture.md) <br/> |メールボックス内の指定したアイテムのカルチャを表します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |最後の項目を変更するのにはユーザーの表示名が含まれています。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に修正された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムや会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。  <br/> |
|[表題](fileas.md) <br/> |連絡先フォルダーに連絡先を保存する方法を表します。  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |連絡先の表示内容を構築する方法を定義します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |連絡先の表示名を定義します。  <br/> |
|[GivenName](givenname.md) <br/> |連絡先の指定された名前が含まれています。  <br/> |
|[[頭文字]](initials.md) <br/> |連絡先のイニシャルを表します。  <br/> |
|[ミドル ネーム](middlename.md) <br/> |連絡先のミドル ネームを表します。  <br/> |
|[ニックネーム](nickname.md) <br/> |連絡先のニックネームを表します。  <br/> |
|[CompleteName](completename.md) <br/> |連絡先の完全な名前を表します。  <br/> |
|[[得意先名]](companyname.md) <br/> |連絡先に関連付けられている会社名を表します。  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |連絡先の電子メール アドレスのコレクションを表します。  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |連絡先に関連付けられている物理アドレスのコレクションが含まれています。  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |連絡先の電話番号のコレクションを表します。  <br/> |
|[AssistantName](assistantname.md) <br/> |連絡先にアシスタントを表します。  <br/> |
|[Birthday](birthday.md) <br/> |連絡先の生年月日を表します。  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |連絡先のホーム ページ (Web アドレス) を表します。  <br/> |
|[Children](children.md) <br/> |連絡先の子供の名前が含まれています。  <br/> |
|[Companies](companies.md) <br/> |連絡先に関連付けられている企業のコレクションを表します。  <br/> |
|[ContactSource](contactsource.md) <br/> |連絡先が Exchange ストアまたは Active Directory ディレクトリ サービス内にあるかどうかについて説明します。  <br/> |
|[Department](department.md) <br/> |職場の連絡先の部署を表します。  <br/> |
|[生成](generation.md) <br/> |連絡先の完全な名前を次世代の省略形を表します。  <br/> |
|[ImAddresses](imaddresses.md) <br/> |連絡先のインスタント メッセージング アドレスのコレクションを表します。  <br/> |
|[役職](jobtitle.md) <br/> |取引先担当者の役職名を表します。  <br/> |
|[マネージャー](manager.md) <br/> |連絡先のマネージャーを表します。  <br/> |
|[マイレージ](mileage.md) <br/> |連絡先アイテムの経費情報を表します。  <br/> |
|[事業所](officelocation.md) <br/> |連絡先のオフィスの場所を表します。  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |物理アドレスの表示の種類を表します。  <br/> |
|[Profession](profession.md) <br/> |連絡先の職業を表します。  <br/> |
|[SpouseName](spousename.md) <br/> |連絡先の配偶者またはパートナーの名前を表します。  <br/> |
|[姓](surname.md) <br/> |連絡先の姓を表します。  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |取引先担当者の結婚記念日が含まれています。  <br/> |
|[HasPicture](haspicture.md) <br/> |連絡先アイテムが連絡先の画像を表す添付ファイルがあるかどうかを示します。  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |発音のスペルの最初と最後の名前を含む、連絡先の完全な名前が含まれています。  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |連絡先の名前を含む発音のスペルします。  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |連絡先の姓が含まれている発音のスペルします。  <br/> |
|[エイリアス](alias.md) <br/> |連絡先の電子メール エイリアスが含まれています。  <br/> |
|[ノート (連絡先)](notes-contact.md) <br/> |補足の連絡先情報が含まれています。  <br/> |
|[Photo](photo.md) <br/> |連絡先の写真をエンコードする値が含まれています。  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |連絡先の SMIME の証明書をエンコードする値が含まれています。  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |連絡先の [Microsoft Exchange 証明書をエンコードする値が含まれています。  <br/> |
|[DirectoryId](directoryid.md) <br/> |連絡先のディレクトリ ID が含まれています。  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |連絡先のマネージャーのメールボックスを識別するための SMTP 情報が含まれています。  <br/> |
|[DirectReports](directreports.md) <br/> |取引先担当者の直属の部下を識別するための SMTP 情報が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素名**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表のアイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムまたはフォルダーのプロパティを追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべての項目を識別します。  <br/> |
|[(ItemSync) を作成します。](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列が含まれています。  <br/> |
|[アイテム (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素で識別されるフォルダーを作成する項目の配列が含まれています。  <br/> |
|[解決策](resolution.md) <br/> |解決された 1 つのエンティティが含まれています。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[更新プログラム (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つの項目を識別します。  <br/> |
   
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
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)


[連絡先 (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[連絡先を更新](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[連絡先を削除します。](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

