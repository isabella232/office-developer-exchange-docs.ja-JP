---
title: Exchange での EWS 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Exchange で使用可能な EWS 操作についての情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 143903d9198a7e31e876adcbbb336df34ecf01fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526124"
---
# <a name="ews-operations-in-exchange"></a>Exchange での EWS 操作

Exchange で使用可能な EWS 操作についての情報を検索します。
  
Exchange Web サービス (EWS) には、Exchange ストアからの情報へのアクセスを可能にする多くの操作が用意されています。 このセクションの記事では、EWS 操作の要求、応答、エラー応答メッセージの全体的な構造、および各操作の XML 例について説明します。 クライアントとサーバー間で送信されるメッセージ構造の概要を説明します。 この情報を使用して、メッセージ構造をデバッグしたり、EWS 要求で何ができるかについての情報を見つけることができます。 XML 構造が何を表しているかの詳細については、「 [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)」を参照してください。
  
すべての EWS 機能は、スキーマのバージョンに関連付けられています。 新しい EWS スキーマのバージョンは、Exchange Server または Exchange Online の新しいリリースで導入されました。 [RequestServerVersion](requestserverversion.md)要素には、サーバーバージョンをスキーマバージョンにマップする**version**属性が含まれています。 この記事では、各操作がいつ導入されたかについて説明します。 操作内の特定の機能によっては、サービスの新しいバージョンが必要になる場合があります。 以前のバージョンの EWS に対して設計されたクライアントが、新しいバージョンの EWS で動作するように、バージョン付きのスキーマが実装されています。 
  
これらの操作は、メールボックスを処理する EWS エンドポイントを対象とすることができます。 Http:///ews/exchange .asmx に似た URL を使用して、EWS エンドポイントを参照できます。 <clientaccessserver> ここで、 <clientaccessserver> はメールボックスをサービスする Exchange クライアントアクセスサーバーです。 自動検出を使用して、メールボックスをサービスするクライアントアクセスサーバーへの URL を取得できます。 自動検出の詳細については、「 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)」を参照してください。
  
## <a name="ediscovery-operations"></a>電子情報開示の操作
<a name="bk_eDiscovery"> </a>

電子情報開示操作は、法的情報保留のための検索操作を提供し、探索検索結果でインデックスが作成されずに返されるメールボックスのデータを特定します。
  
次の表に、電子情報開示操作の一覧を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration 操作](getdiscoverysearchconfiguration-operation.md) <br/> |Exchange 2013  <br/> |
|[GetHoldOnMailboxes 操作](getholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[GetNonIndexableItemDetails 操作](getnonindexableitemdetails-operation.md) <br/> |Exchange 2013  <br/> |
|[GetNonIndexableItemStatistics 操作](getnonindexableitemstatistics-operation.md) <br/> |Exchange 2013  <br/> |
|[Getsearchablemailemail箱操作](getsearchablemailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[SearchMailboxes ボックスの操作](searchmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
|[SetHoldOnMailboxes 操作](setholdonmailboxes-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a>Exchange メールボックスデータの操作
<a name="bk_Exchange_mailbox_data"> </a>

Exchange メールボックスデータ操作を使用すると、クライアントはアイテム、フォルダー、および添付ファイルを処理および整理し、あいまいな名前解決と配布リストの展開を行うことができます。 Exchange メールボックスのデータ操作には、アイテム、フォルダー、添付ファイル、およびユーティリティの操作が含まれます。
  
次の表に、Exchange メールボックスのデータ操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[アーカイブアイテムの操作](archiveitem-operation.md) <br/> |Exchange 2013  <br/> |
|[CreateItem 操作](createitem-operation.md) <br/> |Exchange 2007  <br/> |
|[CopyItem 操作](copyitem-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteItem 操作](deleteitem-operation.md) <br/> |Exchange 2007  <br/> |
|[FindItem 操作](finditem-operation.md) <br/> |Exchange 2007  <br/> |
|[GetItem 操作](getitem-operation.md) <br/> |Exchange 2007  <br/> |
|[MarkAllItemsAsRead 操作](markallitemsasread-operation.md) <br/> |Exchange 2013  <br/> |
|[MoveItem 操作](moveitem-operation.md) <br/> |Exchange 2007  <br/> |
|[SendItem 操作](senditem-operation.md) <br/> |Exchange 2007  <br/> |
|[UpdateItem 操作](updateitem-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表に、Exchange メールボックスデータフォルダーの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[CreateFolder 操作](createfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[CreateFolderPath 操作](createfolderpath-operation.md) <br/> |Exchange 2013  <br/> |
|[CreateManagedFolder 操作](createmanagedfolder-operation.md) <br/> |Exchange 2007。 Exchange 2010 以降のバージョンの Exchange では、この機能は強調されていません。 メッセージングレコード管理用の保持タグおよびポリシーを使用するように移行する方法の詳細については、「[管理フォルダーからの移行](https://technet.microsoft.com/library/dd298032%28v=exchg.141%29.aspx)」を参照してください。  <br/> |
|[CopyFolder 操作](copyfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteFolder 操作](deletefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[EmptyFolder 操作](emptyfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[FindFolder 操作](findfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[GetFolder 操作](getfolder-operation.md) <br/> |Exchange 2007  <br/> |
|[MoveFolder 操作](movefolder-operation.md) <br/> |Exchange 2007  <br/> |
|[UpdateFolder 操作](updatefolder-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表に、Exchange メールボックスデータ添付操作の一覧を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[CreateAttachment 操作](createattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[GetAttachment 操作](getattachment-operation.md) <br/> |Exchange 2007  <br/> |
|[DeleteAttachment 操作](deleteattachment-operation.md) <br/> |Exchange 2007  <br/> |
   
次の表に、Exchange メールボックスのアラーム操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetReminders 操作](getreminders-operation.md) <br/> |Exchange 2013  <br/> |
|[PerformReminderAction 操作](performreminderaction-operation.md) <br/> |Exchange 2013  <br/> |
   
次の表に、Exchange メールボックスデータの会話操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[ApplyConversationAction 操作](applyconversationaction-operation.md) <br/> |Exchange 2010 Service Pack 1 (SP1)  <br/> |
|[FindConversation 操作](findconversation-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[GetConversationItems 操作](getconversationitems-operation.md) <br/> |Exchange 2013  <br/> |
   
次の表に、Exchange メールボックスデータユーティリティの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[ConvertId 操作](convertid-operation.md) <br/> |Exchange 2007 Service Pack 1  <br/> |
|[ExpandDL 操作](expanddl-operation.md) <br/> |Exchange 2007  <br/> |
|[GetUserPhoto 操作](getuserphoto-operation.md) <br/> |Exchange 2013。 この操作には、REST と SOAP の実装の両方があります。  <br/> |
|[MarkAsJunk 操作](markasjunk-operation.md) <br/> |Exchange 2013  <br/> |
|[ResolveNames 操作](resolvenames-operation.md) <br/> |Exchange 2007  <br/> |
|[GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="availability-operations"></a>可用性の操作
<a name="bk_Availability"> </a>

可用性の操作により、より安全で最新の、または豊富な空き時間情報が提供され、予定表と空き時間情報の共有の機能が向上します。 空き時間情報データは、会議をスケジュールするための重要なコンポーネントです。 可用性運用は、効果的なスケジュール設定のための信頼できる基盤を提供します。 
  
次の表に、可用性の操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetUserAvailability 操作](getuseravailability-operation.md) <br/> |Exchange 2007  <br/> |
|[GetRoomLists 操作](getroomlists-operation.md) <br/> |Exchange 2010  <br/> |
|[GetRooms 操作](getrooms-operation.md) <br/> |Exchange 2010  <br/> |
|[GetUserOofSettings 操作](getuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
|[SetUserOofSettings 操作](setuseroofsettings-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="bulk-transfer-operations"></a>一括転送操作
<a name="bk_bulk_transfer"> </a>

一括転送操作を使用すると、クライアントはメールボックスのアイテムをストリームすることができます。 
  
次の表に一括転送操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[UploadItems 操作](uploaditems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[ExportItems 操作](exportitems-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="delegate-management-operations"></a>管理操作を委任する
<a name="bk_delegate_management"> </a>

代理人管理操作を使用すると、クライアントはメールボックスの代理人の追加、取得、更新、削除を行うことができます。 
  
次の表に、代理人の管理操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[AddDelegate 操作](adddelegate-operation.md) <br/> |Exchange 2007 Service Pack 1 (SP1)  <br/> |
|[GetDelegate 操作](getdelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[UpdateDelegate 操作](updatedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
|[RemoveDelegate 操作](removedelegate-operation.md) <br/> |Exchange 2007 SP1  <br/> |
   
## <a name="inbox-rules-operations"></a>受信トレイルールの操作
<a name="bk_inbox_rules"> </a>

受信トレイルールの操作を使用すると、クライアントは受信トレイルールを取得して、サーバー上のメッセージに対して更新することができます。 受信トレイルールは、メッセージがフォルダーに配信されるときに、クライアントがメッセージを自動的に整理、分類、および処理できるようにする一連の条件と関連付けられたアクションです。 
  
次の表に、受信トレイルールの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetInboxRules の操作](getinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[UpdateInboxRules の操作](updateinboxrules-operation.md) <br/> |Exchange 2010 SP1  <br/> |
   
## <a name="mail-app-management-operations"></a>メールアプリの管理操作
<a name="bk_mail_apps"> </a>

メールアプリの管理操作により、Outlook 用メールアプリを管理できます。 これらの操作は、Outlook Web App および Outlook 2013 で利用可能なメールアプリに関する情報をインストール、アンインストール、無効化、および取得するために使用できます。
  
次の表に、メールアプリの管理操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[DisableApp 操作](disableapp-operation.md) <br/> |Exchange 2013  <br/> |
|[GetAppManifests 操作](getappmanifests-operation.md) <br/> |Exchange 2013  <br/> |
|[GetAppMarketplaceUrl 操作](getappmarketplaceurl-operation.md) <br/> |Exchange 2013  <br/> |
|[GetClientAccessToken 操作](getclientaccesstoken-operation.md) <br/> |Exchange 2013  <br/> |
|[InstallApp 操作](installapp-operation.md) <br/> |Exchange 2013  <br/> |
|[アン Installapp 操作](uninstallapp-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="mail-tips-operation"></a>メールヒントの操作
<a name="bk_mail_tips"> </a>

メールヒント操作を使用すると、作成者がメッセージを作成している場合に、受信者のメールボックスに関する情報をクライアントがサーバーから要求できるようになります。 次の表に、メールヒント操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetMailTips ヒント操作](getmailtips-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="message-tracking-operations"></a>メッセージ追跡操作
<a name="bk_message_tracking"> </a>

メッセージ追跡操作を使用すると、クライアントは、指定された条件に一致するメッセージを検索し、メッセージ追跡レポート内の各メッセージに関する詳細な追跡情報を取得できます。 
  
次の表に、メッセージ追跡操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[FindMessageTrackingReport 操作](findmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
|[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="notification-operations"></a>通知の操作   
<a name="bk_notification"> </a>

通知操作は、指定されたメールボックスのアイテムとフォルダーに関連付けられているイベントをクライアントアプリケーションに通知します。 サブスクリプションモデルは、プッシュベース、プルベース、またはストリーミングベースにすることができます。 
  
次の表に、通知操作の一覧を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetEvents 操作](getevents-operation.md) <br/> |Exchange 2007  <br/> |
|[GetStreamingEvents の操作](getstreamingevents-operation.md) <br/> |Exchange 2010 SP1  <br/> |
|[サブスクライブ操作](subscribe-operation.md) <br/> |Exchange 2007  <br/> |
|[Unsubscribe 操作](unsubscribe-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="persona-operations"></a>Persona 操作
<a name="bk_personas"> </a>

ペルソナ操作は、リンクされた連絡先に関する情報を検索して取得するためのインターフェイスを提供します。 次の表に、ペルソナ操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[FindPeople 操作](findpeople-operation.md) <br/> |Exchange 2013  <br/> |
|[GetPersona 操作](getpersona-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="retention-policy-operation"></a>アイテム保持ポリシーの操作
<a name="bk_retention_policy"> </a>

[アイテム保持ポリシー] 操作には、ユーザーのアイテム保持ポリシーにリンクされているすべての保持タグの一覧が表示されます。 
  
次の表に、アイテム保持ポリシーの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetUserRetentionPolicyTags 操作](getuserretentionpolicytags-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="service-configuration-operation"></a>サービス構成操作
<a name="bk_service_config"> </a>

サービス構成操作により、クライアントは、ユニファイドメッセージング、保護ルール、ポリシーヒント、およびメールヒントサービスの構成情報を取得できます。 
  
次の表に、サービスの構成操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetServiceConfiguration 操作](getserviceconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="sharing-operations"></a>共有操作
<a name="bk_sharing"> </a>

共有の操作により、クライアントは予定表データと連絡先データを共有できます。 
  
次の表に、共有操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[CreateItem (AcceptSharingInvitation)](createitem-acceptsharinginvitation.md) <br/> |Exchange 2010。 **CreateItem**操作は、すべてのバージョンの EWS に適用できますが、 **acceptsharinginvitation**応答オブジェクトは、exchange 2010 以降のバージョンの exchange の ews にのみ適用されます。  <br/> |
|[GetSharingFolder 操作](getsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
|[GetSharingMetadata 操作](getsharingmetadata-operation.md) <br/> |Exchange 2010  <br/> |
|[RefreshSharingFolder 操作](refreshsharingfolder-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="synchronization-operations"></a>同期操作
<a name="bk_synchronization"> </a>

同期操作では、ユーザーのフォルダーとアイテムの一段階の同期キャッシュコピーが提供されます。 
  
次の表に、同期操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md) <br/> |Exchange 2007  <br/> |
|[SyncFolderItems 操作](syncfolderitems-operation.md) <br/> |Exchange 2007  <br/> |
   
## <a name="time-zone-operation"></a>タイムゾーンの操作
<a name="bk_timezone"> </a>

タイムゾーン操作を使用すると、クライアントはサーバーでサポートされているタイムゾーン定義の一覧を取得できます。 
  
次の表に、タイムゾーン操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[GetServerTimeZones 操作](getservertimezones-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="unified-messaging-operations"></a>ユニファイドメッセージングの操作
<a name="bk_um"> </a>

ユニファイドメッセージングの操作により、クライアントは、ユニファイドメッセージングのプロパティに関する情報を読み取って、電話でボイスメールメッセージを再生することができます。 
  
次の表に、ユニファイドメッセージングの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[切断電話操作](disconnectphonecall-operation.md) <br/> |Exchange 2010  <br/> |
|[GetPhoneCallInformation 操作](getphonecallinformation-operation.md) <br/> |Exchange 2010  <br/> |
|[PlayOnPhone 操作 (EWS)](playonphone-operation-ews.md) <br/> |Exchange 2010  <br/> |
   
[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)を使用して、メールボックスのユニファイドメッセージング構成情報を取得します。 ユニファイドメッセージング web サービスは、Exchange 2007 を対象としたユニファイドメッセージングアプリケーションに対して使用します。 詳細については、「[ユニファイドメッセージング web サービスリファレンス (Exchange](unified-messaging-web-service-reference-for-exchange.md))」を参照してください。
  
## <a name="unified-contact-store-operations"></a>統合連絡先ストアの操作
<a name="bk_ucs"> </a>

統合連絡先ストアは、Office 製品間で一貫した連絡先環境を提供し、サードパーティアプリケーションが同じ連絡先ストアを使用するための統合ポイントとして機能します。 これにより、ユーザーとアプリケーションは、連絡先情報を格納、管理、およびアクセスして、Lync、Exchange 2013、Outlook、Outlook Web App、および統合連絡先ストアへのアクセスを実装するその他のアプリケーション間でグローバルに利用できるようになります。 Exchange は、統合連絡先ストアの機能のコンテンツストアです。
  
次の表に、統合連絡先ストアの操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[AddNewImContactToGroup 操作](addnewimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddImContactToGroup 操作](addimcontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddImGroup 操作](addimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[AddNewTelUriContactToGroup 操作](addnewteluricontacttogroup-operation.md) <br/> |Exchange 2013  <br/> |
|[Adddeploy Grouptoimlist 操作](adddistributiongrouptoimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[GetImItemList 操作](getimitemlist-operation.md) <br/> |Exchange 2013  <br/> |
|[GetImItems 操作](getimitems-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveContactFromImList 操作](removecontactfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveImContactFromGroup 操作](removeimcontactfromgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveDistributionGroupFromImList 操作](removedistributiongroupfromimlist-operation.md) <br/> |Exchange 2013  <br/> |
|[RemoveImGroup 操作](removeimgroup-operation.md) <br/> |Exchange 2013  <br/> |
|[SetImGroup 操作](setimgroup-operation.md) <br/> |Exchange 2013  <br/> |
   
## <a name="user-configuration-operations"></a>ユーザー構成操作
<a name="bk_user_config"> </a>

ユーザー構成操作は、クライアントがユーザー構成情報を作成、削除、取得、更新できるようにします。 
  
次の表に、ユーザーの構成操作を示します。
  
|**操作名**|**導入バージョン**|
|:-----|:-----|
|[CreateUserConfiguration 操作](createuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[DeleteUserConfiguration 操作](deleteuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[GetUserConfiguration 操作](getuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
|[UpdateUserConfiguration 操作](updateuserconfiguration-operation.md) <br/> |Exchange 2010  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
    

