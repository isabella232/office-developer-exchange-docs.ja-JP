---
title: Exchange で Web サービスの使用を開始する
manager: sethgros
ms.date: 2/27/2017
ms.audience: Developer
localization_priority: Normal
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Exchange の EWS などの Web サービスを初めて使用する際に役立つ情報を紹介します。
ms.openlocfilehash: 2f203c5634c29105feb39220c3ebdd9624bb49ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759185"
---
# <a name="start-using-web-services-in-exchange"></a>Exchange で Web サービスの使用を開始する

Exchange の EWS などの Web サービスを初めて使用する際に役立つ情報を紹介します。
  
[Exchange の Web サービス](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)により、Exchange Online、Office 365 の一部としての Exchange Online、および Exchange Server 2007 以降のオンプレミス バージョンの Exchange に保存されたメールボックスのデータにアクセスできるようになり、その情報を組織の要件に従って管理する際に使用できるカスタム アプリケーションの作成が可能になります。 作成可能な EWS や Web サービスのアプリケーションの範囲は実質的に無限ですが、どのような種類のアプリケーションにも特定の基本的概念が適用されます。 このセクションでは、Exchange の EWS などの Web サービスの使用を開始するために、十分に理解しておく必要のある基本的な概念についての情報を提供します。 
  
## <a name="build-your-knowledge"></a>知識を身につける
<a name="bk_Knowledge"> </a>

Web サービス アプリケーションの開発に .NET Framework とその他のプラットフォームのどちらを使用するにしても、開発プロジェクトの開始前に理解しておく必要のある重要な概念があります。 
  
**表 1.Web サービスの概念**

|**概念**|**概要**|
|:-----|:-----|
|[アーキテクチャ](ews-applications-and-the-exchange-architecture.md) <br/> |EWS が Exchange アーキテクチャで動作するしくみと、EWS が使用するプロトコルについて説明します。  <br/> |
|[EWS アプリケーションの種類](ews-application-types.md) <br/> |Exchange の EWS を使用して作成できる、最も一般的な種類のアプリケーションについて説明します。  <br/> |
|[EWS のアクセス](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Exchange 管理者は、EWS へのアクセスをグローバルに (組織全体、個別のユーザー、および個別のアプリケーションに) 制限できます。適切なアクセス レベルを見つけてください。  <br/> |
|[セットアップ](setting-up-your-ews-application.md) <br/> |EWS マネージ API または EWS を使用して Exchange と通信するアプリケーションを作成するために実行する必要のあるタスクについての情報を確認します。  <br/> |
|[認証](authentication-and-ews-in-exchange.md) <br/> |Exchange Online および Exchange オンプレミスに接続するための認証オプションについて説明します。  <br/> |
|[自動検出](autodiscover-for-exchange.md) <br/> |EWS によってユーザーのアカウントで情報にアクセスできる URL エンドポイントの検出に使用可能なサービスのセットについて説明します。  <br/> |
|[メールボックス サーバー](http://technet.microsoft.com/ja-JP/library/jj150491%28v=exchg.150%29.aspx) <br/> |EWS クライアントから利用できるようなる情報のプライマリ リポジトリについて説明します。EWS は、Active Directory ドメイン サービス (AD DS) に保存されている情報の限定的なセットにアクセスできます。  <br/> |
|[Outlook 用メール アプリと EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Outlook 用メール アプリについての情報と、そのアプリが Exchange の EWS で動作するしくみを説明します。  <br/> |
|[メール、予定表、および連絡先の Office 365 REST API](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Office 365 の一部としての Exchange Online のメール、予定表、および連絡先へのアクセスに使用できる Office 365 API について説明します。  <br/> |
|[EWS マネージ API](get-started-with-ews-managed-api-client-applications.md) <br/> |.NET Framework 開発者に推奨されるクライアント API の情報について紹介します。  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |EWS XML の要求と応答を使用する初めてのアプリケーションの作成について紹介します。  <br/> |
|[Exchange 製品バージョンでの EWS 機能](ews-functionality-in-exchange-product-versions.md) <br/> |Exchange のバージョンで使用可能な EWS 機能について説明します。  <br/> |
|[トレースとトラブルシューティング](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |EWS マネージ API のエラーをトラブルシューティングするために、EWS の要求と応答をトレースする方法について説明します。  <br/> |
   
## <a name="create-your-first-application"></a>初めてのアプリケーションを作成する
<a name="create"> </a>

初めての .NET Framework または EWS クライアント アプリケーションの作成に取りかかる準備ができている場合は、「[EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)」または「[EWS クライアント アプリケーションの概要](get-started-with-ews-client-applications.md)」を参照してください。
  
## <a name="get-code-samples"></a>コード サンプルを取得する
<a name="samples"> </a>

Exchange の EWS などの Web サービスを操作する方法を示すコード サンプルと用例については、次のリソースを参照してください。
  
- [Exchange コード サンプル](http://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Exchange API のドキュメント](develop-web-service-clients-for-exchange.md)
    
- [Exchange 開発者フォーラム](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)
    
その他にも多数のサンプルが、ブログやコードのデモ サイト、フォーラムにあります。また、[EWSEditor](http://ewseditor.codeplex.com/) のダウンロードもお勧めしています。このプロジェクトは EWS のほとんどの機能を実装しています。ここでは、主要な EWS 機能のすべての例が見つかります。
  
.NET Framework 開発者ではない場合は、Java、Python、PHP などの言語を使用する EWS 開発者に向けた多数のクライアント ライブラリがあります。 
  
## <a name="ask-questions-and-solve-problems"></a>質問と問題の解決
<a name="questions"> </a>

何かするときにサポートが必要なのに解決策が見当たらない状況ですか。 [Exchange Development フォーラム](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)を検索し、ほかの誰かが同じ課題に遭遇し、その解決策を見いだしたかどうかを調べることができます。 Exchange 開発についての何百もの質問に寄稿者コミュニティが回答しています。 Exchange 開発を対象にしているサード パーティのサイト、フォーラム、およびブログも調べてみてください。探しているソリューションが見つかることがあります。 
  
追加の支援が必要な場合は、[Microsoft サポート](https://support.microsoft.com/)にお問い合わせください。Exchange 開発者のサポート チームには、Exchange 開発についての質問を解決に導く経験豊富な担当者が配属されています。 
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS マネージ API、EWS、Web サービスについて探究してみましょう](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Exchange の EWS クライアントの設計の概要](ews-client-design-overview-for-exchange.md) 
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md) 
- [Exchange web サービスの参照](../web-service-reference/web-services-reference-for-exchange.md)
    

