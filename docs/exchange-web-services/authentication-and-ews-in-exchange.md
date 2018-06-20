---
title: Exchange の認証と EWS
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9a83df96-aca0-42b3-b8f5-2b414f0363f1
description: Exchange を対象とする EWS アプリケーションの適切な認証基準の選択に役立つ情報を紹介します。
ms.openlocfilehash: c81b29cbe9aa3c658a8f776876366fd0875b2669
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758878"
---
# <a name="authentication-and-ews-in-exchange"></a>Exchange の認証と EWS

Exchange を対象とする EWS アプリケーションの適切な認証基準の選択に役立つ情報を紹介します。
  
認証は、Exchange Web サービス (EWS) アプリケーションの主要な部分の 1 つです。Exchange Online、Office 365 の一部としての Exchange Online、および Exchange 2013 以降のオンプレミス バージョンの Exchange では、アプリケーションと Exchange サーバー間の通信をセキュリティで保護するため、標準的な Web 認証プロトコルをサポートしています。
  
Exchange Online を対象にしている、選択した認証方法は要求と、アプリケーションが送信する応答を暗号化するために HTTPS を使用する必要があります。 オンプレミスの Exchange サーバーは、HTTP を使用できますが、アプリケーションと Exchange サーバー間のセキュリティで保護された通信のために、アプリケーションが EWS のエンドポイントに送信するすべての要求には、HTTPS を使用することをお勧めします。
  
Exchange には認証オプションが用意されており、次の中から選択できます。  
  
- OAuth 2.0 (Exchange Online のみ)
    
- NTLM (オンプレミスの Exchange のみ)
    
- 基本 (推奨されていません)
    
選択した認証方法は、組織は Exchange のオンラインまたは Exchange 設置のどちらを使用しているかどうか、OAuth トークンを発行できるサードパーティのプロバイダーへのアクセスがあるかどうかのセキュリティ要件によって異なります。 この資料では、アプリケーションの適切な標準の認証を選択するうえで役立つ情報を提供します。
  
## <a name="oauth-authentication"></a>OAuth 認証

すべての新しいアプリケーションで OAuth 標準を使用して、Exchange Online サービスに接続することをお勧めします。アプリケーションに OAuth を実装するためには追加の作業が必要ですが、基本認証に勝るセキュリティ上の利点はそれに見合う価値があります。ただし、レコードに関しては、認識しておくべきデメリットもいくつかあります。
  
**表 1 です。OAuth を使用しての利点と欠点**

|**利点**|**短所**|
|:-----|:-----|
| OAuth は業界標準の認証プロトコルです。<br/><br/>認証はサードパーティのプロバイダーによって管理されます。アプリケーションで Exchange の資格情報を収集して保存する必要はありません。<br/><br/>心配が少ないため、アプリケーションは、認証プロバイダーから不明確なトークンを受信するだけしたがって、アプリケーションのセキュリティ侵害はトークン、ユーザーの Exchange 情報ではないのみを公開できます。  <br/> | OAuth はサード パーティの認証プロバイダーに依存しています。このためユーザーの組織や顧客に追加のコストが発生します。<br/><br/>OAuth 標準の実装は基本認証の実装よりも困難です。<br/><br/>OAuth を実装するには、認証プロバイダーと Exchange サーバーの両方にアプリケーションを統合する必要があります。   <br/> |
   
短所を最小限に抑えるために、ことができますを使用する[Microsoft Azure AD 認証ライブラリ](http://msdn.microsoft.com/library/a03f39fa-7ba4-4182-a98e-55562a64b8f3%28Office.15%29.aspx)(ADAL) クラウドまたはオンプレミスの Active Directory ドメイン サービス (AD DS) に対してユーザーを認証し、呼び出しのセキュリティを保護するためのアクセス トークンを取得しに、Exchange サーバーです。 Exchange Online は、ADAL でサポートされている、Azure Active Directory サービスによって発行されたトークンが必要です。ただし、任意のサードパーティのライブラリを使用できます。 
  
EWS アプリケーションで OAuth 認証を使用する方法の詳細については、次のリソースを参照してください。
  
- [Office 365 の試用版](http://office.microsoft.com/compare-office-365-for-business-plans-FX102918419.aspx?CR_CC=200061904&amp;WT.srch=1&amp;WT.mc_ID=PS_bing_O365Comm_office%20365%20trial_Text)を使用して、クライアント アプリケーションをテストするのには Exchange サーバーをセットアップします。
    
- [Azure AD Authentication Library for .NET](http://msdn.microsoft.com/library/a03f39fa-7ba4-4182-a98e-55562a64b8f3%28Office.15%29.aspx)
    
- [Azure Active Directory の構成](http://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)、OAuth トークンを認証に使用するアプリケーションを有効にします。
    
- [認証 OAuth を使用して、EWS アプリケーション](how-to-authenticate-an-ews-application-by-using-oauth.md)を調べることができますコードの例のサンプル コードを確認します。 
    
## <a name="ntlm-authentication"></a>NTLM 認証

NTLM 認証が使用できるのは、オンプレミスの Exchange サーバーのみです。会社のファイアウォールの内側で実行されるアプリケーションに対しては、NTLM 認証と .NET Framework 間の統合で、アプリケーションを認証するための組み込みの手段を用意しています。  
  
**表 2 になります。NTLM 認証を使用しての利点と欠点**

|**利点**|**短所**|
|:-----|:-----|
| Works「アウト ボックスの」Exchange サーバーにします。 [Exchange 管理シェル コマンドレット](how-to-control-access-to-ews-in-exchange.md)を使用して Exchange サービスへのアクセスを構成できます。<br/><br/>.NET Framework [CredentialCache](http://msdn2.microsoft.com/EN-US/library/615e0wsd)オブジェクトを使用すると、自動的にユーザーの資格情報を取得します。<br/><br/>[コード サンプルは、利用可能な](http://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)を使用して、ログオンしたユーザーの資格情報に、オンプレミスの Exchange サーバーへの認証をします。  <br/> | ユーザーは、NTLM 認証を使用するためにドメインにログオンする必要がある。<br/><br/>ユーザーのドメイン アカウントに関連付けられていないメール アカウントにアクセスすることが困難となります。<br/><br/>サービス アプリケーションに、NTLM 認証を利用するためのドメイン アカウントが必要。  <br/> |
   
## <a name="basic-authentication"></a>基本認証

基本認証は、クライアント アプリケーションに対して適切な基本レベルのセキュリティを提供します。すべての新しいアプリケーションが認証用に、NTLM または OAuth プロトコルを使用することを強くお勧めします。ただし、状況によっては、基本認証を選択することが適切な場合もあります。
  
**表 3。基本認証を使用しての利点と欠点**

|**利点**|**短所**|
|:-----|:-----|
| Works「アウト ボックスの」Exchange サーバーにします。 [Exchange 管理シェル コマンドレット](how-to-control-access-to-ews-in-exchange.md)を使用して Exchange サービスへのアクセスを構成できます。<br/><br/>Windows アプリケーションでは、ログオンしたユーザーの既定の資格情報を使用できます。<br/><br/>多く[なコード サンプルでは利用可能な](http://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)EWS が基本認証を使用してを呼び出す方法を説明します。  <br/> | 収集し、ユーザーの資格情報を保存するようにアプリケーションが必要です。<br/><br/>すべてのユーザが基本認証を使用するには、NTLM 認証を無効にする必要がある。<br/><br/>アプリケーションでは、セキュリティ侵害が発生する場合、ユーザーの電子メール アドレスと、攻撃者にパスワードを公開できます。  <br/> |
   
基本認証が、ユーザーの組織と顧客のセキュリティ要件を満たしているかどうかを判断する必要があります。基本認証は、簡単なテストやデモ アプリケーションなどで、詳細なセットアップ タスクを行わないようにする場合に、最適な選択肢になることがあります。
  
## <a name="see-also"></a>関連項目

- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)   
- [サインオン Microsoft Azure AD を使用して Web アプリケーションに追加します。](http://msdn.microsoft.com/library/055e1155-2d4d-4c85-b44e-d406872ba595%28Office.15%29.aspx)    
- [Exchange EWS へのアクセスを制御します。](how-to-control-access-to-ews-in-exchange.md)    
- [Exchange クライアント アプリケーションの EWS へのアクセスを制御します。](controlling-client-application-access-to-ews-in-exchange.md)    
- [サポートされているトークンと要求の種類](http://msdn.microsoft.com/library/9d35e4bc-7b72-49d1-b723-5464eee6be2c%28Office.15%29.aspx)
    

