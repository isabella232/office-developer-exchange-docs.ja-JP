---
title: Exchange 内の EWS の構成オプション
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: 'EWS クライアントからアクセス可能な構成設定と、EWS クライアントに影響を与える構成可能な Exchange の設定に関する情報について紹介します。 '
ms.openlocfilehash: d6c2866abf3dc16c77d84355afb9d86b0a9934c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
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
  
**表 1 です。EWS のクライアントの構成オプションを提供する web サービスの機能**

|**機能**|**説明**|
|:-----|:-----|
|自動検出サービス  <br/> |[自動検出サービス](autodiscover-for-exchange.md)は、クライアントが自動的に通信 EWS 自体を構成するように、クライアントに構成情報を使用してアプリケーションを提供します。  <br/> |
|メールボックスに保存されているカスタム構成情報  <br/> |[カスタム構成情報を格納](persistent-application-settings-in-ews-in-exchange.md)するいくつかのオプションのいずれかを使用するには、メールボックスの: ユーザーの構成オブジェクト、カスタム アイテム、または拡張プロパティです。  <br/> |
|代理人管理  <br/> | EWS では、メールボックスに代理人アクセスを管理する CRUD 操作を提供します。 デリゲートは、別のユーザーのメールボックスにアクセスする権限が与えられているユーザーです。<br/><br/>  [代理人の管理操作](http://msdn.microsoft.com/en-us/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management)を使用するには、ews、委任管理を有効にするまたは、EWS のマネージ API を使用する場合は、以下の方法を使用することができます。<br/><br/>- [ExchangeService.AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|電子情報開示検索の構成  <br/> |電子的証拠開示のクライアント アプリケーションは、電子的証拠開示検索クエリ、検索可能なメールボックスの一覧を含む[構成情報の検索](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx)を取得でき、埋め込み先のメールボックスの id を保持します。  <br/> |
|フォルダーのアクセス許可  <br/> |フォルダーのアクセス許可を制限する、パブリック フォルダーでユーザーが実行できるし、代理人アクセスの場合、代理人で何ができる別のユーザーのフォルダーにします。 [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドまたは[GetFolder の操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)のいずれかを使用すると、パブリック フォルダー、共有フォルダー、またはユーザーが代理人アクセス フォルダーを含め、すべてのフォルダーのアクセス許可セットにアクセスします。  <br/> |
|メールのヒント、ユニファイド メッセージング、または保護ルール  <br/> |[GetServiceConfiguration 操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)では、メール ヒント、ユニファイド メッセージング、および保護のルールの読み取り専用の[サービスの構成情報](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)を提供します。  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Exchange サーバーで管理者がアクセスできる構成設定

クライアント アプリケーションのほとんどのシナリオは、サーバーの構成設定への変更を必要としません。ただし、いくつかのシナリオを実行します。 たとえば、ユーザーとして動作するように中間層のアプリケーションを有効にするには、サーバー上で Exchange の偽装を設定する必要があります。 いくつかの設定には、オンプレミスの Exchange サーバーにだけアクセスできることに注意してください。 対象とする Exchange のオンライン、クライアント アプリケーションが既定の設定を操作する必要があります。
  
**表 2 になります。EWS のクライアントに影響する Exchange サーバーの構成オプション**

|**機能**|**Exchange オンラインからアクセスできるようにしますか。**|**詳細についてを参照してください.**|
|:-----|:-----|:-----|
|仮想ディレクトリの設定 (認証を含む)  <br/> |いいえ  <br/> |[Get WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998810%28v=exchg.150%29.aspx) <br/> [セット WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|自動検出  <br/> |いいえ  <br/> |[Get AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa996819%28v=exchg.150%29.aspx) <br/> [セット AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|コンプライアンス  <br/> |はい  <br/> |[アーカイブ](http://technet.microsoft.com/en-us/library/dd979800%28v=exchg.150%29.aspx) <br/> [電子的証拠開示](http://technet.microsoft.com/en-us/library/dd298021%28v=exchg.150%29.aspx) <br/> [保持](http://technet.microsoft.com/en-us/library/dd335168%28v=exchg.150%29.aspx) <br/> [データ損失の防止](http://technet.microsoft.com/en-us/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|代理人管理  <br/> |はい  <br/> |[受信者のアクセス許可を管理します。](http://technet.microsoft.com/en-us/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Exchange の偽装  <br/> |はい  <br/> |[Exchange の偽装を構成します。](http://msdn.microsoft.com/en-us/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|メールのヒント、ユニファイド メッセージング、または保護ルール  <br/> |はい  <br/> |[メール ヒント](http://technet.microsoft.com/en-us/library/jj649091%28v=exchg.150%29.aspx) <br/> [ユニファイド メッセージングのコマンドレット](http://technet.microsoft.com/en-us/library/aa997665%28v=exchg.150%29.aspx) <br/> [Outlook の保護ルール](http://technet.microsoft.com/en-us/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|調整  <br/> |いいえ  <br/> |[調整の設定](ews-throttling-in-exchange.md) <br/> |
|ユーザー エージェントのフィルター処理  <br/> |はい  <br/> |[ユーザー エージェントをフィルタ リング](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange EWS を使用してサービスの構成情報を取得します。](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md)   
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

