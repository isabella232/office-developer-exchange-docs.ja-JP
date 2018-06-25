---
title: Exchange での EWS の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Exchange で使用できる EWS 操作に関する情報を検索します。
ms.openlocfilehash: c56c3be746138cec251836fcb61ee3738d168869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760366"
---
# <a name="ews-operations-in-exchange"></a>Exchange での EWS の操作

Exchange で使用できる EWS 操作に関する情報を検索します。
  
Exchange Web サービス (EWS) は、Exchange ストアからの情報にアクセスできるようにする多くの操作を提供します。 このセクションの記事では、要求、応答、および各操作のための XML の例だけでなく、EWS の操作、エラーの応答メッセージの全体的な構造に関する情報を提供します。 クライアントとサーバー間で送信されるメッセージの構造の概要を提供します。 メッセージ構造体をデバッグして、EWS の要求で行うことができます詳細を確認するには、この情報を使用します。 詳細についてはどのような XML 構造は、 [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)を参照してください。
  
EWS のすべての機能は、スキーマのバージョンに関連付けられます。 新しい EWS のスキーマ バージョンは、Exchange Server または Exchange Online の新しいリリースで導入されます。 [RequestServerVersion](requestserverversion.md)要素には、スキーマのバージョンをサーバー バージョンにマップする**バージョン**の属性が含まれています。 この資料では、各操作が導入されたに関する情報を提供します。 操作内の特定の機能には、サービスの新しいバージョンを必要があります。 バージョン管理されたスキーマは、EWS の以前のバージョンを対象に設計されたクライアントが EWS の新しいバージョンで動作するように実装されます。 
  
EWS エンドポイント、メールボックスを処理するこれらの操作対象にできます。 Http:// 構造体に次のような URL を使用して、EWS のエンドポイントを参照する<clientaccessserver>.com/ews/exchange.asmx、<clientaccessserver>は、Exchange クライアント アクセス サーバー、メールボックスを処理します。 自動検出を使用すると、メールボックスを処理するクライアント アクセス サーバーへの URL を取得します。 自動検出の詳細については、 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)を参照してください。
  
## <a name="ediscovery-operations"></a>電子情報開示の操作
<a name="bk_eDiscovery"> </a>

電子的証拠開示の操作では、法的保存の検索操作を提供し、メールボックスのデータをインデックス化し、検索の検索結果で返されることはできませんを識別します。
  
次の表は、電子的証拠開示の操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[GetSearchableMailboxes 操作](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[SearchMailboxes 操作](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Exchange のメールボックス データの操作
<a name="bk_Exchange_mailbox_data"> </a>

Exchange のメールボックス データの操作は、クライアントを処理し、あいまいな名前解決、配布リストの展開に加え、アイテム、フォルダー、および添付ファイルを整理するを有効にします。 Exchange のメールボックス データの操作には、アイテム、フォルダー、添付ファイル、およびユーティリティの操作が含まれます。
  
次の表は、Exchange のメールボックス データの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[ArchiveItem 操作](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|
  [CreateItem 操作](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|
  [CopyItem 操作](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteItem の操作](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|
  [FindItem 操作](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|
  [GetItem 操作](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[MarkAllItemsAsRead 操作](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|
  [MoveItem 操作](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|
  [SendItem 操作](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|
  [UpdateItem 操作](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表は、Exchange メールボックスのデータ フォルダーの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|
  [CreateFolder 操作](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[CreateFolderPath 操作](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[CreateManagedFolder 操作](createmanagedfolder-operation.md) <br/> |Exchange 2007。 この機能はバージョンの Exchange が Exchange 2010 で始まる deemphasized されています。 メッセージング レコード管理用のタグを保存し、ポリシーを使用して移行する方法の詳細については、[管理対象フォルダーからの移行](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.141%29.aspx)を参照してください。  <br/> |
|[CopyFolder 操作](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteFolder 操作](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[EmptyFolder 操作](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|
  [FindFolder 操作](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|
  [GetFolder 操作](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[MoveFolder 操作](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|
  [UpdateFolder 操作](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表は、Exchange メールボックスのデータの添付ファイルの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[CreateAttachment 操作](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[GetAttachment 操作](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteAttachment 操作](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表に、Exchange メールボックスのアラームの操作を示します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetReminders 操作](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[PerformReminderAction 操作](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
次の表に、Exchange メールボックス データの対話操作を示します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[ApplyConversationAction 操作](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|
  [FindConversation 操作](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|
  [GetConversationItems 操作](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
次の表は、Exchange のメールボックス データ ユーティリティの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[ConvertId 操作](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[ExpandDL 操作](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[GetUserPhoto 操作](getuserphoto-operation.md) <br/> |Exchange 2013。 この操作では、残りの部分と SOAP の実装の両方があります。  <br/> |
|[MarkAsJunk の操作](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[ResolveNames 操作](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>可用性の操作
<a name="bk_Availability"> </a>

予定表と空き時間情報より最新の状態で、豊富なセキュリティで保護された空き時間情報を提供することで経験を共有する、可用性の操作が向上します。 空き時間情報データは、会議をスケジュールすることの重要なコンポーネントです。 可用性の操作では、効果的なスケジュールに関する信頼性の高い基盤を提供します。 
  
次の表は、可用性の操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetUserAvailability 操作](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[GetRoomLists 操作](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[GetRooms 操作](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[GetUserOofSettings 操作](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[SetUserOofSettings 操作](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>一括転送操作
<a name="bk_bulk_transfer"> </a>

一括転送操作は、メールボックスとの間にクライアントがストリームの項目を有効にします。 
  
次の表は、バルク転送の操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[UploadItems 操作](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[ExportItems 操作](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>管理作業を委任します。
<a name="bk_delegate_management"> </a>

代理人の管理操作は、追加、取得、更新、クライアントを有効にし、自分のメールボックスからデリゲートを削除します。 
  
次の表に、代理人の管理操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[AddDelegate 操作](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[GetDelegate 操作](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[UpdateDelegate 操作](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[RemoveDelegate 操作](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>受信トレイ ルールの操作
<a name="bk_inbox_rules"> </a>

受信トレイ ルールの操作は、クライアントが受信トレイ ルールを取得し、サーバー上のメッセージの更新を有効にします。 受信トレイ ルールは、条件およびクライアントが自動的に整理、分類、およびフォルダーにメッセージが配信されると同時に、メッセージの機能を有効にするに関連付けられているアクションのセットです。 
  
次の表に、受信トレイ ルールの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetInboxRules の操作](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[UpdateInboxRules の操作](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>メール アプリケーションの管理
<a name="bk_mail_apps"> </a>

メール アプリケーションの管理操作を使用すると、Outlook のメール アプリケーションを管理できます。 インストール、アンインストール、無効にするには、これらの操作を使用して Outlook Web App および Outlook 2013 で使用可能なメール ・ アプリケーションに関する情報を取得できます。
  
メール アプリケーションの管理操作を次の表に一覧します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[DisableApp 操作](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[GetAppManifests 操作](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[GetClientAccessToken 操作](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[InstallApp 操作](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[UninstallApp 操作](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>メール ヒントの操作
<a name="bk_mail_tips"> </a>

メール ヒントの操作は、作成者がメッセージを作成するときに受信者のメールボックスのサーバーから情報を要求するクライアントを有効にします。 次の表に、メール ヒントの操作を示します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetMailTips 操作](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>メッセージ追跡の操作
<a name="bk_message_tracking"> </a>

メッセージ追跡操作は、指定条件を満たすメッセージを検索して、メッセージ ・ トラッキング ・ レポート内の各メッセージについての詳細な追跡情報を取得するクライアントを有効にします。 
  
次の表は、メッセージの操作を追跡します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>通知の操作
<a name="bk_notification"> </a>

通知の操作は、指定されたメールボックス アイテムおよびフォルダーに関連付けられているイベントのクライアント アプリケーションを通知します。 プッシュ、プル ベース、またはストリーム ベースのサブスクリプション モデルができます。 
  
次の表は、通知の操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetEvents 操作](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[GetStreamingEvents の操作](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[サブスクライブ操作](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Unsubscribe 操作](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>ペルソナの操作
<a name="bk_personas"> </a>

ペルソナの操作は、検索し、リンクされた取引先担当者に関する情報を取得するためのインターフェイスを提供します。 次の表は、ペルソナの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[FindPeople 操作](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[GetPersona 操作](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>保持ポリシーの操作
<a name="bk_retention_policy"> </a>

保持ポリシーの操作には、ユーザーのアイテム保持ポリシーにリンクされているすべての保持タグの一覧が用意されています。 
  
次の表に、保持ポリシーの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetUserRetentionPolicyTags 操作](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>サービス構成の操作
<a name="bk_service_config"> </a>

サービスの構成操作は、ユニファイド メッセージング、保護の規則、ポリシーのヒントは、メール ヒントおよびサービスの構成情報を取得するクライアントを有効にします。 
  
サービス構成の操作を次の表に一覧します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetServiceConfiguration 操作](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>操作の共有
<a name="bk_sharing"> </a>

共有の操作は、予定表データ、連絡先データを共有するクライアントを有効にします。 
  
次の表は、共有の操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[Createitem メソッド (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010。 **CreateItem**操作は、EWS のすべてのバージョンに該当する場合は、 **AcceptSharingInvitation**応答オブジェクトは EWS バージョンの Exchange が Exchange 2010 を起動します。  <br/> |
|[GetSharingFolder 操作](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[GetSharingMetadata 操作](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[RefreshSharingFolder 操作](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>同期操作
<a name="bk_synchronization"> </a>

同期操作は、ユーザーのフォルダーおよびアイテムのキャッシュされたコピーの一方向同期を提供します。 
  
次の表は、同期操作を示します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[SyncFolderItems の操作](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>タイム ゾーンの処理
<a name="bk_timezone"> </a>

タイム ゾーンの操作は、サーバーでサポートされているタイム ゾーン定義の一覧を取得するクライアントを有効にします。 
  
次の表に、タイム ゾーンの処理をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[GetServerTimeZones 操作](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>ユニファイド メッセージングの操作
<a name="bk_um"> </a>

ユニファイド メッセージング操作は、ユニファイド メッセージングのプロパティについての情報を読み取ると、電話でボイス メール メッセージを再生するのにはクライアントを有効にします。 
  
次の表に、ユニファイド メッセージングの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[DisconnectPhoneCall 操作](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[GetPhoneCallInformation 操作](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[PlayOnPhone 操作 (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)を使用すると、メールボックスのユニファイド メッセージングの構成情報を取得できます。 ユニファイド メッセージングの web サービスを Exchange 2007 ユニファイド メッセージング アプリケーションを使用します。 詳細については、 [exchange ユニファイド メッセージングの web サービス参照](unified-messaging-web-service-reference-for-exchange.md)を参照してください。
  
## <a name="unified-contact-store-operations"></a>統合連絡先ストアの操作
<a name="bk_ucs"> </a>

統合連絡先ストアでは、Office 製品間で一貫性のある取引先担当者の経験を提供し、同じ連絡先ストアを使用するサードパーティ製のアプリケーションの統合ポイントとして機能します。 格納、管理、および連絡先情報にアクセスおよび Lync 2013 の Exchange、Outlook、Outlook Web App では、統合連絡先ストアへのアクセスを実装するその他のアプリケーション間でグローバルに使用できるようにするには、ユーザーやアプリケーションを有効にします。 Exchange は、統合連絡先ストアで利用するコンテンツのストアです。
  
次の表は、統合連絡先ストアの操作をします。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[AddNewImContactToGroup 操作](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddImContactToGroup 操作](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddImGroup 操作](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddNewTelUriContactToGroup 操作](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddDistributionGroupToImList 操作](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[GetImItemList 操作](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[GetImItems 操作](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveContactFromImList 操作](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveImContactFromGroup 操作](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveDistributionGroupFromImList 操作](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveImGroup 操作](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[SetImGroup 操作](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>ユーザーの構成の操作
<a name="bk_user_config"> </a>

ユーザーの構成操作は、作成、削除、取得するには、クライアントを有効にして、ユーザー構成情報を更新します。 
  
次の表は、ユーザーの構成操作を示します。
  
|**操作名**|**導入されました。**|
|:-----|:-----|
|[CreateUserConfiguration 操作](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[DeleteUserConfiguration 操作](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[GetUserConfiguration 操作](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[UpdateUserConfiguration 操作](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange、EWS の管理 API、EWS、および web サービスを探索します。](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
    

