---
title: Exchange で EWS へのクライアント アプリケーションのアクセスを制御する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: EWS へのクライアント アプリケーション アクセスを管理するためのオプションについて説明します。
ms.openlocfilehash: 29a640178afc9814a0b2232225ae4307e49afed2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758880"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Exchange で EWS へのクライアント アプリケーションのアクセスを制御する

EWS へのクライアント アプリケーション アクセスを管理するためのオプションについて説明します。
  
作成された EWS クライアント アプリケーションはすべて、EWS 操作を呼び出す前に、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降の バージョンの Exchange へのアクセス権を付与されている必要があります。テスト サーバーまたは運用サーバーの管理者は、Exchange 管理シェルを使用して、すべてのユーザーおよびアプリケーション、個々のユーザー、または個々のアプリケーションの EWS へのアクセスを制限できます。EWS へのアクセス制御は、ドメイン アカウントに基づきます。ローカル セキュリティ機関によって認証された資格情報で接続が行われた場合、サーバーはドメイン アカウントのみが接続できることを示すエラーを返します。  
  
## <a name="access-control-for-ews-clients-and-users"></a>EWS クライアントおよびユーザーのアクセス制御
<a name="bk_configure"> </a>

テスト サーバーまたは運用サーバーの管理者は、次の方法で EWS に接続するクライアントのアクセス制御を構成できます。  
  
- すべてのクライアント アプリケーションの接続をブロックする。
    
- 特定のクライアント アプリケーションの接続のみを許可する。
    
- 明示的にブロックされているものを除き、すべてのクライアント アプリケーションの接続を許可する。
    
- すべてのクライアント アプリケーションの接続を許可する。
    
アプリケーションは、HTTP Web 要求で送信されるユーザー エージェント文字列によって識別されます。
  
> [!アプリケーション レベルのセキュリティに関するメモ] ブロックは、そのセキュリティ機能ではありません。 ユーザー エージェント文字列は容易に偽装します。 アプリケーションには、EWS へのアクセスが許可されている場合、アプリケーションする必要がありますが資格情報を提示するアプリケーションは、EWS を接続する前にサーバーが認証されます。 
  
管理者は、次の方法で EWS に接続するメールボックスの所有者のアクセス制御を構成できます。  
  
- 組織全体をブロックまたは、許可する。
    
- EWS へのアクセス権を持たないメールボックスの所有者を包含または除外する役割ベースの認証スコープによって識別された、ユーザーのグループをブロック、または許可する。
    
- 個々のメールボックスの所有者をブロック、または許可する。
    
特定のアクセス制御の設定は、アクセス制御の全般設定より優先されます。たとえば、組織によって EWS へのアクセスが拒否されている場合でも、個々のメールボックスの所有者がアプリケーションへのアクセスを許可されている場合、個々の設定が優先され、アクセスが許可されます。  
  
## <a name="delegation-and-ews-access-management"></a>EWS へのアクセス管理および委任 
<a name="bk_delegation"> </a>

アクセス権を持たない委任ユーザーがクライアント アプリケーションを使用した場合、プリンシパル ユーザーが EWS へのアクセス権を持っている場合でも、そのユーザーは EWS を使用してプリンシパル ユーザーのメールボックスにアクセスすることはできません。委任ユーザーが EWS へのアクセス権を持っている場合、プリンシパル ユーザーが EWS のアクセス権がなくても、その委任ユーザーは EWS クライアント アプリケーションを使用してプリンシパル ユーザーのメールボックスにアクセスすることができます。  
  
## <a name="impersonation-and-ews-access-management"></a>権限の借用および EWS へのアクセス管理 
<a name="bk_impersonation"> </a>

メールボックスの所有者の代わりに EWS に接続するクライアント アプリケーションは、メールボックスの所有者の EWS 設定を使用できない場合があります。たとえば、会社に電子メールをアーカイブするアプリケーションは、メールボックス ユーザーの設定に関係なく EWS に接続する必要があります。メール クライアントなどその他のアプリケーションは、メールボックスの所有者の EWS 設定を使用する必要があります。  
  
管理者は、それぞれのサーバー上で使用するアプリケーションやアプリケーション クラスごとに権限借用アカウントを作成する必要があります。これにより管理者は、EWS へのアクセス許可を持たないすべてのユーザーに役割ベースのアクセス制御スコープを構成できます。  
  
権限借用アカウントを有効にするには、テストまたは運用サーバー管理者が次のいずれかを実行します。  
  
- 認証ユーザー グループを Pre-Win2K Compatible Access グループに追加する。  
    
- Exchange Servers グループを Windows Authorization Access グループに追加する。  
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>アクセス管理のための Exchange 管理シェル コマンドレット 
<a name="bk_cmdlets"> </a>

管理者は、次の Exchange 管理シェル コマンドレットを使用して EWS のアクセス制御を構成します。  
  
- [Get CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx)
    
- [セット CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx)
    
- [Get OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx)
    
- [セット OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx)
    
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)  
- [Exchange EWS へのアクセスを制御します。](how-to-control-access-to-ews-in-exchange.md)
- [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

