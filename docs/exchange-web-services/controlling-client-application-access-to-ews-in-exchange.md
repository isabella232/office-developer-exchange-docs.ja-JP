---
title: Exchange において、EWS へのクライアント アプリケーションのアクセスを制御する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: EWS へのクライアント アプリケーションのアクセスを管理するためのオプションについての詳細です。
ms.openlocfilehash: e3a0e07b733b4ebc070ab6b3fc73c8aec4b62785
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353064"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a>Exchange において、EWS へのクライアント アプリケーションのアクセスを制御する

EWS へのクライアント アプリケーションのアクセスを管理するためのオプションについての詳細です。
  
作成された EWS クライアント アプリケーションはすべて、EWS 操作を呼び出す前に、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降の バージョンの Exchange へのアクセス権を付与されている必要があります。テスト サーバーまたは運用サーバーの管理者は、Exchange 管理シェルを使用して、すべてのユーザーおよびアプリケーション、個々のユーザー、または個々のアプリケーションの EWS へのアクセスを制限できます。EWS へのアクセス制御は、ドメイン アカウントに基づきます。ローカル セキュリティ機関によって認証された資格情報で接続が行われた場合、サーバーはドメイン アカウントのみが接続できることを示すエラーを返します。  
  
## <a name="access-control-for-ews-clients-and-users"></a>EWS のクライアントおよびユーザーのアクセス制御
<a name="bk_configure"> </a>

試験用サーバーまたは運用サーバーの管理者は、以下のようにして EWS に接続するクライアントのアクセス制御を構成することができます。 
  
- すべてのクライアント アプリケーションの接続をブロックする。
    
- 特定のクライアント アプリケーションの接続のみを許可する。
    
- 明示的にブロックされているものを除き、すべてのクライアント アプリケーションの接続を許可する。
    
- すべてのクライアント アプリケーションの接続を許可する。
    
アプリケーションは、HTTP Web 要求で送信されるユーザー エージェント文字列によって識別されます。
  
> [!IMPORTANT]
> アプリケーション レベルのブロックは、セキュリティ機能ではありません。ユーザー エージェント文字列は容易にスプーフィングされます。EWS へのアクセスが許可されているアプリケーションの場合でも、アプリケーションは EWS に接続する前に資格情報を提示し、サーバーによって認証される必要があります。  
  
管理者は、次の方法で EWS に接続するメールボックスの所有者のアクセス制御を構成できます。 
  
- 組織全体をブロックまたは、許可する。
    
- EWS へのアクセス権を持たないメールボックスの所有者を包含または除外する役割ベースの認証スコープによって識別された、ユーザーのグループをブロック、または許可する。
    
- 個々のメールボックスの所有者をブロック、または許可する。
    
特定のアクセス制御の設定は、アクセス制御の全般設定より優先されます。たとえば、組織によって EWS へのアクセスが拒否されている場合でも、個々のメールボックスの所有者がアプリケーションへのアクセスを許可されている場合、個々の設定が優先され、アクセスが許可されます。  
  
## <a name="delegation-and-ews-access-management"></a>委任と EWS アクセス管理
<a name="bk_delegation"> </a>

アクセス権を持たない委任ユーザーがクライアント アプリケーションを使用した場合、プリンシパル ユーザーが EWS へのアクセス権を持っている場合でも、そのユーザーは EWS を使用してプリンシパル ユーザーのメールボックスにアクセスすることはできません。委任ユーザーが EWS へのアクセス権を持っている場合、プリンシパル ユーザーが EWS のアクセス権がなくても、その委任ユーザーは EWS クライアント アプリケーションを使用してプリンシパル ユーザーのメールボックスにアクセスすることができます。  
  
## <a name="impersonation-and-ews-access-management"></a>偽装と EWS アクセス管理
<a name="bk_impersonation"> </a>

メールボックスの所有者の代わりに EWS に接続するクライアント アプリケーションは、メールボックスの所有者の EWS 設定を使用できない場合があります。たとえば、会社に電子メールをアーカイブするアプリケーションは、メールボックス ユーザーの設定に関係なく EWS に接続する必要があります。メール クライアントなどその他のアプリケーションは、メールボックスの所有者の EWS 設定を使用する必要があります。  
  
管理者は、それぞれのサーバー上で使用するアプリケーションやアプリケーション クラスごとに権限借用アカウントを作成する必要があります。これにより管理者は、EWS へのアクセス許可を持たないすべてのユーザーに役割ベースのアクセス制御スコープを構成できます。  
  
権限借用アカウントを有効にするには、テストまたは運用サーバー管理者が次のいずれかを実行します。 
  
- 認証ユーザー グループを Pre-Win2K Compatible Access グループに追加する。 
    
- Exchange Servers グループを Windows Authorization Access グループに追加する。 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a>アクセス管理のための Exchange 管理シェル コマンドレット
<a name="bk_cmdlets"> </a>

管理者は、EWS アクセス制御を構成する際、以下の Exchange 管理シェル コマンドレットを使用します。 
  
- [Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb124754.aspx)   
- [Set-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb125264.aspx)   
- [Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997571.aspx)   
- [Set-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997443.aspx)
    
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)  
- [Exchange で EWS へのアクセスを制御する](how-to-control-access-to-ews-in-exchange.md)
- 
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [Windows PowerShell](http://msdn.microsoft.com/ja-JP/library/dd835506%28v=vs.85%29.aspx)
    

