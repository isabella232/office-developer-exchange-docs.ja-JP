---
title: Exchange における EWS のプロパティと拡張プロパティ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 68623048-060e-4602-b3fa-62617a94cf72
description: Exchange で EWS を使用して、アイテムとフォルダーのプロパティを定義してアクセスできるようにする方法を説明します。
ms.openlocfilehash: 0c01d9bd21cbef0a3536c8dbd85e192199b7b8ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759182"
---
# <a name="properties-and-extended-properties-in-ews-in-exchange"></a>Exchange における EWS のプロパティと拡張プロパティ

Exchange で EWS を使用して、アイテムとフォルダーのプロパティを定義してアクセスできるようにする方法を説明します。
  
Exchange メールボックスには、電子メール メッセージ、予定、会議など、多数のアイテムが含まれています。 それらのアイテムはプロパティで構成されます。プロパティにはアイテムの記述があります。 アイテムのプロパティを使用して、[検索](search-and-ews-in-exchange.md)、[アイテムの変更の同期](mailbox-synchronization-and-ews-in-exchange.md)、および[カスタム プロパティの種類の作成](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)を行うことができます。 この記事では、プロパティの概要と、アプリケーションでプロパティを使用する方法の概要について扱います。
  
## <a name="exchange-item-properties"></a>Exchange のアイテム プロパティ
<a name="ItemsAreProperties"> </a>

Exchange のアイテムとフォルダーは、基本的には表内の行です。 アイテムまたはフォルダーを識別する主なプロパティは、[EWS 識別子](ews-identifiers-in-exchange.md)です。 Exchange データベースにはその他の識別子に関連するプロパティがありますが、EWS の場合、EWS 識別子はアイテムを記述するプロパティのコレクションの主キーとして機能します。 EWS の識別子プロパティには、次の 2 つの部分があります。
  
- アイテムを識別する [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) プロパティまたは [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) プロパティ 
    
- アイテムまたはフォルダーが変更されたかどうかに関するステートフルな情報を含む **ChangeKey** プロパティ 
    
メールボックス内のすべてのアイテムは、同じ Exchange データベースに格納され、同じデータベース スキーマを使用します。 アイテムは、[ItemClass](http://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) プロパティ、プロパティの制約、および Exchange ストアでの管理方法に影響するビジネス ロジック層、の組み合わせによって識別されます。 表 1 は、様々なアイテムの種類にプロパティが適用される方法を示しています。ここでは、電子メールのアイテムと予定のアイテムの例を取り上げています。 どちらのアイテムも [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) プロパティの値を持っています。 ただし、[IsAllDayEvent](http://msdn.microsoft.com/library/29140a64-9d7a-4a14-a10d-c98197c9831b%28Office.15%29.aspx) プロパティは電子メール アイテムに設定されず、**IsReadReceiptRequested** プロパティは予定アイテムに設定されません。 どのプロパティが各アイテム クラスに適用できるかを知っている必要はなく、その点は EWS が処理してくれます。 
  
**表 1. 予定のプロパティと電子メールのプロパティの比較**

|**アイテムの種類**|**アイテム クラス**|**件名**|**IsAllDayEvent**|**IsReadReceiptRequested**|
|:-----|:-----|:-----|:-----|:-----|
|メール  <br/> |IPM.Note  <br/> |進捗レポート:プロジェクト X の完了  <br/> |NULL  <br/> |true  <br/> |
|Appointment  <br/> |IPM.Appointment  <br/> |Contoso 全社ミーティング  <br/> |false  <br/> |NULL  <br/> |
   
EWS のスキーマは、Exchange データベースで管理されている、また EWS と Exchange データベースの間のビジネス ロジック層で管理されている制約の多くをサポートしています。EWS のスキーマは、定義されたプロパティのセットを各アイテムの種類ごとに適用します。EWS で提供される厳密に型指定された Exchange データベースのアイテムを次に示します。  
  
- 電子メール メッセージ
    
- 予定
    
- 連絡先
    
- 配布リスト
    
- 会議のメッセージ
    
- 会議出席依頼
    
- 会議の応答
    
- 会議のキャンセル
    
- タスク
    
- アイテムの投稿
    
EWS では、汎用アイテムは電子メール メッセージとして返されます。EWS マネージ API では、これらすべてのアイテムの種類を実装します。
  
> [!NOTE]
> 応答オブジェクトは、他のユーザーから受信したアイテムへの応答として、クライアントによってのみサーバーに送信されます。応答オブジェクトは、Exchange データベース内には存在しません。 
  
## <a name="what-are-properties-in-ews"></a>EWS のプロパティとは
<a name="WhatAreEWSProperties"> </a>

EWS のスキーマは、EWS のクライアントと Exchange の間で送信されるデータを記述します。 スキーマの大部分は、Exchange データベースにアクセスできるアイテムとフォルダーのプロパティを記述します。 EWS のスキーマは、アプリケーションで利用可能な Exchange データベースのプロパティの XML 表現について記述します。 実際のプロパティ、利用可能なプロパティ、それらの形式、返す値は、実行しようとしている処理によって異なります。 たとえば、**Body** プロパティは **FindItem** 操作の最初の 512 文字のみを返しますが、**GetItem** 操作は、アイテムのテキスト全体を返します。 ほとんどのプロパティは、設定および取得が可能ですが、一部のプロパティは Exchange によって設定のみ行われます。 各プロパティは、スキーマに XML 形式で存在しており、Exchange データベースに保存される際のプロパティを反映するか、Exchange データベースに保存されているプロパティから計算されます。 **Subject** プロパティは設定可能なプロパティの例であり、フォルダーの **UnreadCount** プロパティは、計算されたプロパティの例です。 プロパティのコア セットは、コア アイテムの種類と共通です。 
  
アプリケーションが Exchange から取得するプロパティ セットは、次の要因によって決まります。 
  
- アプリケーションが呼び出している操作
    
- 基本的な応答の図形
    
- アイテムの種類
    
- 指定したプロパティのパス
    
これらのさまざまな要素が、アクセスできるデータにどのように影響するかを理解することが重要です。 前述した **Body** プロパティの例のように、いくつかの情報はさまざまな要因に応じて条件付きで利用できます。 これらの要因を理解していると、必要な情報を利用する適切なオプションを選択できるので、時間の節約になります。 どのプロパティが利用できるかを確認するには、これらの要因を吟味して、アプリケーションが必要とするプロパティを利用する方法を判断する必要があります。 ここでは、EWS の応答で返されるプロパティに、これらのさまざまな要因がどのように影響するのか説明します。 
  
### <a name="ews-response-shapes"></a>EWS の応答の図形

Exchange は、アイテムに関する様々な情報を格納しています。 アプリケーションでは、必ずしもすべての情報を必要としない場合があり、情報をまったく取得しないことが最適な場合も少なくありません。 [EWS 応答の図形](property-sets-and-response-shapes-in-ews-in-exchange.md)はプロパティの図形とも呼ばれ、どのプロパティがサーバーから返されるかを示します。 応答の図形の中心となる要素は、基本図形です。 基本図形は、厳密に型指定されたアイテムの既定の事前設定プロパティ バッグです。 EWS マネージ API で基本図形に相当するものは [BasePropertySet](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) です。 EWS には、3 つの既定の応答図形が含まれています。
  
**表 2. 既定の応答の図形**

|**既定の応答の図形の名前**|**EWS マネージ API の同等物**|**説明**|
|:-----|:-----|:-----|
|IdOnly  <br/> |BasePropertySet.IdOnly  <br/> |EWS 識別子と変更キーのみが返されます。 クライアントは、AllProperties または既定の図形から返されるすべてのプロパティを使用する場合を除き、IdOnly 図形を使用し、**PropertySet** クラスのプロパティ パス セットを使用して追加のプロパティを指定します。 ほとんどのアプリケーションは、追加のプロパティを指定して IdOnly 応答図形を使用する必要があります。 これにより、クライアントによって要求される不要なデータの量が減少します。  <br/> |
|既定値  <br/> |N/A  <br/> |アイテムの種類の標準プロパティのセット。アプリケーションがプロパティをすべて使用する場合にのみ、この応答の図形を使用します。    <br/> |
|AllProperties  <br/> |BasePropertySet.FirstClassProperties 値  <br/> |既定の図形よりも大規模なプロパティのセットです。名前が示すものとは異なり、このオプションはアイテムに対してすべてのプロパティを返すことはしません。このプロパティ セットは、クライアント アプリケーションで最も頻繁に使用されるプロパティを返します。追加のプロパティが必要な場合、プロパティ パスを使用して要求できます。   <br/> アプリケーションが、この応答の図形で返されたプロパティをすべて使用するわけではない場合、追加のプロパティを指定して IdOnly の応答の図形を使用します。  <br/> |
   
EWS の操作の多くは、アイテムとそのプロパティを返します。指定した応答の図形に関わりなく、操作が異なれば、異なるプロパティ セットが返ってくることがあります。また、アイテムの種類が異なると、指定した操作と応答の図形に応じて、異なるプロパティが返されます。次の操作では、どのプロパティを返すのかを識別するために応答の図形を使用します。
  
**表 3. 応答の図形を使用する操作**

|**EWS 操作**|**EWS マネージ API メソッド**|
|:-----|:-----|
|[GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |[ExchangeService.GetConversationItems メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |
|[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |[Folder.Bind メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |
|[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |[Item.Bind メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [ExchangeService.BindToItems メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |
|[FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |[ExchangeService.FindConversation メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |
|[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |[Folder.FindFolders メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [ExchangeService.FindFolders メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |
|[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |[Folder.FindItems メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> [ExchangeService.FindItems メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |
|[FindPeople](http://msdn.microsoft.com/library/446106b7-ff2d-4107-90c1-29f4d38ba128%28Office.15%29.aspx) <br/> |実装されていません。  <br/> |
|[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) <br/> |[ExchangeService.ResolveNames メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |[ExchangeService.SearchMailboxes メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.searchmailboxes%28v=exchg.80%29.aspx) <br/> [ExchangeService.BeginSearchMailboxes メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.beginsearchmailboxes%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) <br/> |[ExchangeService.SyncFolderHierarchy メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) <br/> |
|[SyncFolderItems](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) <br/> |[ExchangeService.SyncFolderItems メソッド](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderitems%28v=exchg.80%29.aspx) <br/> |
   
プロパティの図形は、アプリケーションに返してほしいプロパティを識別する基本的な手段です。ただし、アプリケーションが特定のプロパティのより洗練されたセットを必要とすることがあります。これには、プロパティ パスを使用できます。
  
### <a name="choose-properties-by-their-property-path"></a>プロパティ パスによってプロパティを選択する

EWS のプロパティ パスは、要求または応答のいずれかのプロパティを識別するために使用されるメタデータです。 
  
**表 4. プロパティ パスの種類**

|**プロパティ パスの種類**|**スキーマの種類**|**EWS マネージ API の実装**|**説明**|
|:-----|:-----|:-----|:-----|
|FieldUri  <br/> |PathToUnindexedFieldType  <br/> |[ServiceObjectSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceobjectschema%28v=exchg.80%29.aspx) から継承される種類。  <br/> |最も一般的なプロパティ パス。 FieldUri プロパティ パスは、EWS マネージ API の **PropertySet** オブジェクトで指定されます。 FieldUri プロパティ パスでは、EWS のほとんどのプロパティを指定できます。 これは、EWS のスキーマで UnindexedFieldURIType によって記述されます。  <br/> FieldUri プロパティ パスの XML は、次のようになります。  <br/> ```XML<FieldURI FieldURI="item:Subject"/>```このプロパティのパスは、EWS マネージ API の ItemSchema.Subject に相当します。  <br/> |
|IndexedFieldUri  <br/> |PathToIndexedFieldType  <br/> |[ItemSchema](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) から継承される種類。  <br/> |返す値を指定するためにプロパティ インデックスを必要とする、ディクショナリ プロパティを識別します。 プロパティが複数の値を持つことができる場合に、このパスを使用します。 これは、EWS のスキーマで **DictionaryURIType** プロパティによって記述されます。 **DictionaryURIType** プロパティ パスは、EWS マネージ API の **PropertySet** オブジェクトで指定されます。  <br/> IndexedFieldUri プロパティ パスの XML は、次のようになります。  <br/> ```XML<IndexedFieldURI FieldURI="contacts:PhysicalAddress:Street FieldIndex="Home"/>```|
|ExtendedFieldUri  <br/> |PathToExtendedFieldType  <br/> |[ExtendedPropertyDefinition](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |アイテムのカスタム プロパティまたはスキーマ化されていないプロパティを識別する拡張プロパティの定義です。  <br/> ExtendedFieldUri プロパティ パスの XML は、次のようになります。  <br/> ```XML<ExtendedFieldURI> PropertyTag="0x1234" PropertyType="Integer" />```|
|ExceptionFieldUri  <br/> |ExceptionFieldURI  <br/> |[ServiceResponse](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.serviceresponse%28v=exchg.80%29.aspx) <br/> |EWS の応答のエラーに関連付けられているプロパティを指定します。 これは、EWS のスキーマで **ExceptionPropertyURIType** 型によって記述されます。 これは、予定表の定期的なパターンを使用しているときに行われるエラー応答の **MessageXml** 要素でのみ発生します。  <br/> |
   
ベスト プラクティスとして、プロパティを要求するときは、IdOnly 基本図形 (EWS マネージ API の [BasePropertySet.IdOnly](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx)) を使用し、プロパティのパスを指定することにより、アプリケーションにとって必要なプロパティのみを要求します。 
  
### <a name="schematized-properties"></a>スキーマ化されたプロパティ

EWS クライアントが必要とするプロパティのほとんどは、EWS のスキーマによって記述されます。 主なフォルダーとアイテムの種類の定義は、プロパティの定義を含むもので、Types.xsd スキーマ内にあります。 次のスキーマの種類には、使用できるほとんどのオブジェクトのプロパティの定義が含まれています。
  
**表 5. プロパティ定義が含まれているスキーマの種類**

|**EWS のスキーマの種類**|**EWS マネージ API の種類の同等物**|**定義対象**|
|:-----|:-----|:-----|
|**ItemType** <br/> |[アイテム クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) <br/> |基本アイテム型のプロパティ セットこの型は、クライアントから作成することができますが、Exchange によって返されることはありません。Exchange は、汎用的なすべてのオブジェクトに対して MessageType オブジェクトを返します。  <br/> |
|**MessageType** <br/> |[EmailMessage クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |電子メール メッセージ オブジェクトのプロパティ セットとすべての汎用的なオブジェクトのプロパティ セット。  <br/> |
|**CalendarItemType** <br/> |[Appointment クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |予定表アイテムのプロパティ セット。これには、1 つの定期的な予定が含まれます。  <br/> |
|**ContactItemType** <br/> |[Contact クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |連絡先アイテムのプロパティ セット。  <br/> |
|**DistributionListType** <br/> |[ContactGroup クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) <br/> |個人用配布リストのプロパティ セット。  <br/> |
|**MeetingMessageType** <br/> |[MeetingMessage クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingmessage%28v=exchg.80%29.aspx) <br/> |会議のメッセージ型のプロパティ セット。  <br/> |
|**MeetingRequestMessageType** <br/> |[MeetingRequest クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingrequest%28v=exchg.80%29.aspx) <br/> |会議の要求型のプロパティ セット。  <br/> |
|**MeetingResponseMessageType** <br/> |[MeetingResponse クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingresponse%28v=exchg.80%29.aspx) <br/> |会議の応答型のプロパティ セット。  <br/> |
|**MeetingCancellationMessageType** <br/> |[MeetingCancellation クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.meetingcancellation%28v=exchg.80%29.aspx) <br/> |会議の取り消し型のプロパティ セット。  <br/> |
|**TaskType** <br/> |[Task クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |タスク型のプロパティ セット。  <br/> |
|**PostItemType** <br/> |[PostItem クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.postitem%28v=exchg.80%29.aspx) <br/> |Postitem 型のプロパティ セット。  <br/> |
|**FolderType** <br/> |[Folder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) <br/> |フォルダー型のプロパティ セット。  <br/> |
|**CalendarFolderType** <br/> |[CalendarFolder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx) <br/> |SearchFolder 型のプロパティ セット。  <br/> |
|**ContactsFolderType** <br/> |[ContactsFolder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx) <br/> |ContactsFolder 型のプロパティ セット。  <br/> |
|**SearchFolderType** <br/> |[SearchFolder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx) <br/> |SearchFolder 型のプロパティ セット。  <br/> |
|**TasksFolderType** <br/> |[TasksFolder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx) <br/> |TasksFolder 型のプロパティ セット。  <br/> |
|**UserConfigurationType** <br/> |[UserConfiguration クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.userconfiguration%28v=exchg.80%29.aspx) <br/> |UserConfiguration 型のプロパティ セット。  <br/> |
   
EWS スキーマ内のプロパティは、多くのアプリケーションには十分ですが、スキーマで記述されている内容を使用するだけでは実装できないシナリオもあります。 これらのシナリオでは、プロパティを拡張することができます。 
  
### <a name="extended-properties-aka-non-schematized-properties"></a>拡張プロパティ (別名はスキーマ化されていないプロパティ)

拡張プロパティを使用すると、EWS のスキーマで定義されていない Exchange ストア内のアイテムとフォルダーのプロパティにアクセスするためのカスタム プロパティを作成できます。これらを使用して、Exchange データベースのネイティブの MAPI アイテムおよびフォルダーのプロパティにアクセスできます。拡張プロパティを使用して、スキーマ化されたすべてのプロパティにアクセスできます。これは実際には、これらのスキーマ化されたプロパティは単なる Exchange データベースの MAPI プロパティであるためです。  
  
Types.xsd スキーマ内にある、PathToExtendedFieldType スキーマ型は、拡張プロパティを表す XML を定義します。 このスキーマの種類は、XML インスタンスの [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素を定義します。つまり、サービスとクライアント間で送信される XML を定義します。 ExtendedPropertyType スキーマの種類は、[ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素と、拡張プロパティに含まれる値または値の配列の両方を定義します。 次の表は、拡張プロパティの XML のおおよそのマッピングと、EWS マネージ API 内のアイテムの実装方法を示します。 
  
**表 6. EWS マネージ API で実装されると、拡張プロパティの XML**

|**EWS マネージ API の実装**|**内容**|**マップ先**|
|:-----|:-----|:-----|
|[Item.ExtendedProperties プロパティ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.item.extendedproperties%28v=exchg.80%29.aspx) <br/> |アイテムの拡張プロパティのコレクション。  <br/> |アイテムの拡張プロパティの 1 つ以上のインスタンス。  <br/> |
|[ExtendedProperty クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.extendedproperty%28v=exchg.80%29.aspx) <br/> |拡張プロパティの定義と値。  <br/> |ExtendedPropertyType スキーマの種類。  <br/> |
|[ExtendedPropertyDefinition クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) <br/> |拡張プロパティの定義。  <br/> |PathToExtendedFieldType スキーマの種類。  <br/> |
   
アプリケーションで拡張プロパティを使用する方法の詳細については、次のコード サンプルを参照してください。 
  
- [MFCMapi](http://mfcmapi.codeplex.com/)
    
- [Exchange 2013: プログラムを使用してカスタム X ヘッダーをプロビジョニングする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Exchange 2013: プロパティ タグによってプロパティにアクセスする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-719875ac)
    
- [Exchange 2013: 識別子で名前付きプロパティにアクセスする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-02dbe22f)
    
- [Exchange 2013: 名前で名前付きプロパティにアクセスする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-6556e183)
    
- [Exchange 2013: プロパティ セット GUID と名前でプロパティにアクセスする](http://code.msdn.microsoft.com/exchange/Exchange-2013-Access-a-4021f971)
    
- [Exchange 2013: カスタムの拡張プロパティをプログラムによって作成する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Create-314db25a)
    
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange で EWS を使用して X ヘッダーを準備する](how-to-provision-x-headers-by-using-ews-in-exchange.md)
    
- [EWS プロパティ関連のエラー](ews-property-related-errors.md)
    
## <a name="see-also"></a>関連項目


- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    
- [MFCMapi](http://mfcmapi.codeplex.com/)
    

