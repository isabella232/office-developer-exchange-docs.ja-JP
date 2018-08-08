---
title: Exchange 内の EWS の構成オプション
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: EWS クライアントからアクセス可能な構成設定と、EWS クライアントに影響を与える構成可能な Exchange の設定に関する情報について紹介します。
ms.openlocfilehash: d6c2866abf3dc16c77d84355afb9d86b0a9934c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758882"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Exchange 内の EWS の構成オプション

EWS クライアントからアクセス可能な構成設定と、EWS クライアントに影響を与える構成可能な Exchange の設定に関する情報について紹介します。 
  
多数の構成設定が EWS クライアント アプリケーションの動作に影響を与えます。こうした設定は、次のいずれかになります。  
  
- クライアントから読み取り専用または読み書き可能。
    
- EWS サービスをホストしている Exchange サーバーでアクセスされる。
    
クライアントは、Exchange Online、Office 365 の一部としての Exchange Online、およびオンプレミスの Exchange サーバー上の設定にアクセスできます。Exchange 管理者は、オンプレミスの Exchange サーバーのすべての設定を使用できますが、Exchange Online テナント管理者には使用できない設定もあります。この記事では、クライアント、Exchange Server 管理者、および Exchange Online テナント管理者が、どの構成設定にアクセスできるかについて説明します。
  
## <a name="configuration-settings-that-clients-can-access"></a>クライアントがアクセスできる構成設定

クライアント アプリケーションは、Exchange サーバーの構成オプションのいくつかを取得および設定できます。すべての EWS アプリケーションが必要とする構成設定は、自動検出サービスによって提供されます。その他の構成設定は、特殊なアプリケーションのシナリオに使用されます。  
  
**表 1. EWS クライアントの構成オプションを提供する Web サービスの機能**

|**機能**|**説明**|
|:-----|:-----|
|自動検出サービス  <br/> |[自動検出サービス](autodiscover-for-exchange.md)は、クライアント アプリケーションに構成情報を提供します。これにより、クライアントは EWS と通信するように、そのクライアント自体を自動的に構成できるようになります。  <br/> |
|メールボックスに保存されているカスタム構成情報  <br/> |メールボックスに[カスタム構成情報を保存する](persistent-application-settings-in-ews-in-exchange.md)オプションはいくつかありますが (ユーザー構成オブジェクト、カスタム アイテム、または拡張プロパティ)、そのうちの 1 つを使用できます。  <br/> |
|代理人管理  <br/> | EWS には、メールボックスへの代理人アクセスを管理するための CRUD 操作が用意されています。 代理人とは、別のユーザーのメールボックスへのアクセス許可が与えられているユーザーのことです。<br/><br/>  [代理人管理の操作](http://msdn.microsoft.com/ja-JP/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management)を使用して代理人管理を有効にできます (EWS を使用する場合)。また、EWS マネージ API を使用している場合は、次のメソッドを使用します。<br/><br/>- [ExchangeService.AddDelegates](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|電子情報開示検索の構成  <br/> |電子情報開示クライアント アプリケーションは、電子情報開示検索クエリ、検索可能なメールボックスの一覧、およびインプレース メールボックス ホールドの ID を含む[構成情報の検索](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx)が可能です。   <br/> |
|フォルダーのアクセス許可  <br/> |フォルダーのアクセス許可により、ユーザーがパブリック フォルダーで実行可能な操作を制限します。また、代理人アクセスの場合は、代理人が他のユーザーのフォルダーで実行可能な操作を制限します。 [Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドまたは [GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)のどちらかを使用すると、各フォルダーのアクセス許可セットにアクセスできます。このフォルダーには、パブリック フォルダー、共有プライベート フォルダー、またはユーザーが代理人アクセスするフォルダーが含まれます。  <br/> |
|メールのヒント、ユニファイド メッセージング、または保護ルール  <br/> |[GetServiceConfiguration 操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)によって、メールのヒント、ユニファイド メッセージング、および保護ルールに関する読み取り専用の[サービス構成情報](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)が得られます。  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Exchange サーバーで管理者がアクセスできる構成設定

ほとんどのクライアント アプリケーションのシナリオでは、サーバー構成設定に変更を加える必要はありません。ただし、それが必要になるシナリオもあります。 たとえば、中間層アプリケーションがユーザーとして機能できるようにするには、サーバーで Exchange の偽装を設定する必要があります。 一部の設定は、オンプレミスの Exchange サーバーでのみアクセス可能な点に注意してください。 Exchange Online を対象にしている場合、クライアント アプリケーションは既定の設定で操作する必要があります。
  
**表 2. EWS クライアントに影響する Exchange サーバーの構成オプション**

|**機能**|**Exchange Online からアクセス可能にするか**|**詳細の参照先**|
|:-----|:-----|:-----|
|仮想ディレクトリの設定 (認証を含む)  <br/> |いいえ  <br/> |[Get-WebServicesVirtualDirectory](http://technet.microsoft.com/ja-JP/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](http://technet.microsoft.com/ja-JP/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|自動検出  <br/> |いいえ  <br/> |[Get-AutodiscoverVirtualDirectory](http://technet.microsoft.com/ja-JP/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](http://technet.microsoft.com/ja-JP/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|準拠  <br/> |はい  <br/> |[アーカイブ](http://technet.microsoft.com/ja-JP/library/dd979800%28v=exchg.150%29.aspx) <br/> [電子情報開示](http://technet.microsoft.com/ja-JP/library/dd298021%28v=exchg.150%29.aspx) <br/> [保存機能](http://technet.microsoft.com/ja-JP/library/dd335168%28v=exchg.150%29.aspx) <br/> [データ損失防止](http://technet.microsoft.com/ja-JP/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|管理の委任  <br/> |はい  <br/> |[受信者のアクセス許可の管理](http://technet.microsoft.com/ja-JP/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Exchange の偽装  <br/> |はい  <br/> |[Exchange の偽装を構成する](http://msdn.microsoft.com/ja-JP/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|メールのヒント、ユニファイド メッセージング、または保護ルール  <br/> |はい  <br/> |[メールヒント](http://technet.microsoft.com/ja-JP/library/jj649091%28v=exchg.150%29.aspx) <br/> [ユニファイド メッセージングのコマンドレット](http://technet.microsoft.com/ja-JP/library/aa997665%28v=exchg.150%29.aspx) <br/> [Outlook の保護ルール](http://technet.microsoft.com/ja-JP/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|調整  <br/> |いいえ  <br/> |[調整設定](ews-throttling-in-exchange.md) <br/> |
|ユーザー エージェントのフィルター処理  <br/> |はい  <br/> |[ユーザー エージェントのフィルター処理](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange で EWS を使用して、サービス構成情報を取得する](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)   
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

