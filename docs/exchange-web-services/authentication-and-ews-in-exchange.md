---
title: Exchange での認証と EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Exchange を対象とする EWS アプリケーションの適切な認証基準の選択に役立つ情報を紹介します。
localization_priority: Priority
ms.openlocfilehash: 69018b6f88fc80e1e18edd96ed0e16d52064572d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528483"
---
# <a name="authentication-and-ews-in-exchange"></a>Exchange での認証と EWS

Exchange を対象とする EWS アプリケーションの適切な認証基準の選択に役立つ情報を紹介します。
  
認証は、Exchange Web サービス (EWS) アプリケーションの主要な部分の 1 つです。Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降のオンプレミス バージョンの Exchange では、アプリケーションと Exchange サーバー間の通信をセキュリティで保護するため、標準的な Web 認証プロトコルをサポートしています。
  
Exchange Online を対象にしている場合は、選択した認証方法で HTTPS を使用して、アプリケーションが送信する要求と応答を暗号化する必要があります。 オンプレミスの Exchange サーバーでは HTTP を使用できますが、アプリケーションと Exchange サーバー間の通信をセキュリティで保護するために、アプリケーションが EWS のエンドポイントに送信するすべての要求で HTTPS を使用することをお勧めします。
  
Exchange には認証オプションが用意されており、次の中から選択できます。 
  
- OAuth 2.0 (Exchange Online のみ)
    
- NTLM (オンプレミスの Exchange のみ)
    
- 基本 (推奨されていません)
    
選択する認証方法は、Exchange Online またはオンプレミスの Exchange を使用しているかどうか、および OAuth トークンを発行できるサードパーティのプロバイダーへのアクセス権があるかどうかという、組織のセキュリティ要件によって異なります。 この記事では、アプリケーションに適切な認証基準を選択するうえで役立つ情報を提供します。
  
## <a name="oauth-authentication"></a>OAuth 認証

すべての新しいアプリケーションで OAuth 標準を使用して、Exchange Online サービスに接続することをお勧めします。アプリケーションに OAuth を実装するためには追加の作業が必要ですが、基本認証に勝るセキュリティ上の利点はそれに見合う価値があります。ただし、レコードに関しては、認識しておくべきデメリットもいくつかあります。
  
**表 1. OAuth を使用するメリットとデメリット**

|**メリット**|**欠点**|
|:-----|:-----|
| OAuth は業界標準の認証プロトコルです。<br/><br/>認証はサードパーティのプロバイダーによって管理されます。アプリケーションで Exchange の資格情報を収集して保存する必要はありません。<br/><br/>アプリケーションは認証プロバイダーから不透明なトークンを受信するだけなので、心配の種は少なくて済みます。そのため、アプリケーションでセキュリティ違反があっても、トークンが公開されるだけでユーザーの Exchange 資格情報が公開されることはありません。  <br/> | OAuth はサード パーティの認証プロバイダーに依存しています。このためユーザーの組織や顧客に追加のコストが発生します。<br/><br/>OAuth 標準の実装は基本認証の実装よりも困難です。<br/><br/>OAuth を実装するには、認証プロバイダーと Exchange サーバーの両方にアプリケーションを統合する必要があります。  <br/> |
   
デメリットを最小限にするには、[Microsoft Azure AD Authentication Library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries) (ADAL) を使用して、クラウドまたはオンプレミスの Active Directory ドメイン サービス (AD DS) に対してユーザーを認証し、Exchange サーバーへの呼び出しをセキュリティ保護するためのアクセス トークンを取得します。Exchange Online には、ADAL (ただし、任意のサードパーティのライブラリも使用可) でサポートされている Azure Active Directory サービスによって発行されたトークンが必要です。  
  
EWS アプリケーションで OAuth 認証を使用する方法の詳細については、次のリソースを参照してください。
  
- [Office 365 試用版](https://docs.microsoft.com/office/developer-program/office-365-developer-program)。クライアント アプリケーションのテストに使用する Exchange サーバーをセットアップします。
    
- [.NET 用 Azure AD Authentication ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)
    
- 「[Azure Active Directory を構成する](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)」。アプリケーションでの認証に OAuth トークンを使用できるようにします。
    
- 学習できるコード例については、「[OAuth を使用して EWS アプリケーションを認証する](how-to-authenticate-an-ews-application-by-using-oauth.md)」のサンプル コードを確認してください。 
    
## <a name="ntlm-authentication"></a>NTLM 認証

NTLM 認証が使用できるのは、オンプレミスの Exchange サーバーのみです。会社のファイアウォールの内側で実行されるアプリケーションに対しては、NTLM 認証と .NET Framework 間の統合で、アプリケーションを認証するための組み込みの手段を用意しています。  
  
**表 2. NTLM 認証を使用するメリットとデメリット**

|**メリット**|**欠点**|
|:-----|:-----|
| “追加設定なし” で Exchange サーバーで機能する。 [Exchange 管理シェル コマンドレット](how-to-control-access-to-ews-in-exchange.md)を使用して、Exchange サービスへのアクセスを構成できる。<br/><br/>.NET Framework の [CredentialCache](https://msdn2.microsoft.com/library/615e0wsd) オブジェクトを使用して、ユーザーの資格情報を自動的に取得する。<br/><br/>オンプレミスの Exchange サーバーへの認証にログオン ユーザーの資格情報を使用する[コード サンプルが利用可能](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)。  <br/> | ユーザーは、NTLM 認証を使用するためにドメインにログオンする必要がある。<br/><br/>ユーザーのドメイン アカウントに関連付けられていないメール アカウントへのアクセスが困難。<br/><br/>サービス アプリケーションに、NTLM 認証を利用するためのドメイン アカウントが必要。  <br/> |

   
## <a name="basic-authentication"></a>基本認証

基本認証は、クライアント アプリケーションに対して適切な基本レベルのセキュリティを提供します。すべての新しいアプリケーションが認証用に、NTLM または OAuth プロトコルを使用することを強くお勧めします。ただし、状況によっては、基本認証を選択することが適切な場合もあります。
  
**表 3. 基本認証を使用するメリットとデメリット**

|**メリット**|**欠点**|
|:-----|:-----|
| “追加設定なし” で Exchange サーバーで機能する。 [Exchange 管理シェル コマンドレット](how-to-control-access-to-ews-in-exchange.md)を使用して、Exchange サービスへのアクセスを構成できる。<br/><br/>Windows アプリケーションで、ログオン ユーザーの既定の資格情報を使用できる。<br/><br/>基本認証を使用して EWS を呼び出す方法を示す多数の[コード サンプルが利用可能](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)。  <br/> | アプリケーションでユーザーの資格情報を収集して保存することが必要。<br/><br/>すべてのユーザーが基本認証を使用するように強制する場合は、NTLM 認証を無効にする必要があります。<br/><br/>アプリケーションでセキュリティ違反が発生した場合、攻撃者にユーザーのメール アドレスとパスワードが漏洩する可能性がある。  <br/> |
   
基本認証が、ユーザーの組織と顧客のセキュリティ要件を満たしているかどうかを判断する必要があります。基本認証は、簡単なテストやデモ アプリケーションなどで、詳細なセットアップ タスクを行わないようにする場合に、最適な選択肢になることがあります。
  
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [Microsoft Azure AD を使用して Web アプリケーションへのサインオンを追加する](https://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Exchange で EWS へのアクセスを制御する](how-to-control-access-to-ews-in-exchange.md)    
- [Exchange で EWS へのクライアント アプリケーションのアクセスを制御する](controlling-client-application-access-to-ews-in-exchange.md)   
- [サポートされているトークンとクレームの種類](https://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
 