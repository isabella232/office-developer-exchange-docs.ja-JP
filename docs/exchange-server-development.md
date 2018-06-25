---
title: オンラインの Exchange および Exchange の開発
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Exchange Server、Exchange オンライン Office 365 の一部として、Exchange のオンライン、Exchange 2013、EWS のマネージ API などを含む Exchange 2010 では、Exchange 2007 用の詳細な開発者向けのドキュメントを検索します。
ms.openlocfilehash: b933bd1bdc6dfcbe4941f23dbee9a587745c7bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758877"
---
# <a name="exchange-online-and-exchange-development"></a>オンラインの Exchange および Exchange の開発

Exchange Server、Exchange オンライン Office 365 の一部として、Exchange のオンライン、Exchange 2013、EWS のマネージ API などを含む Exchange 2010 では、Exchange 2007 用の詳細な開発者向けのドキュメントを検索します。 

方法を使用して、起動すると、新しい機能と開発ツールにアクセスし、サービス、web サイト、デスクトップ コンピューター、およびモバイル デバイスからメールボックスのデータを管理し、電子メール、予定表、連絡先、カスタム ソリューションを作成するのには、API リファレンス ドキュメントを取得でき、オンライン Exchange または Exchange 2013 サーバー上に格納されているその他の項目です。 

アプリケーションの開発には、Exchange Web サービス (EWS)、自動検出、Office 用メール アプリやその他の API を使うことができます。 このページでは、右の Exchange テクノロジを選択することができます。

## <a name="exchange-developer-content"></a>Exchange の開発者がコンテンツ  

次の表を利用すると、開発目標の達成に役立つ技術と関連する API コンテンツを特定できます。  
  
|開発するもの|参照先|
|:-----|:-----|
|Office 365 の一部として Exchange Online にアクセスするための REST ベースのアプリケーション|[メール、予定表、および連絡先の Office 365 REST API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Outlook、Outlook Web App、または OWA にデバイスの情報を表示する状況依存のアプリ |[Exchange での Outlook 用メール アプリと EWS](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Java または.NET Framework に基づいていないメールボックス クライアント |[Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|EWS にアクセスする.NET Framework を使用しているメールボックスのクライアント |[EWS マネージ API クライアント アプリケーションの概要](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|EWS にアクセスするのには Java を使用しているメールボックスのクライアント |[GitHub 上の EWS Java API](https://github.com/OfficeDev/ews-java-api) |
|Outlook のユーザー インターフェイスをカスタマイズしたり、Outlook のビジネス ロジックに依存しているアプリケーション  |[Outlook VBA リファレンス](https://msdn.microsoft.com/en-us/VBA/VBA-Outlook) |
|Exchange Online を対象とするアプリケーションまたは Exchange の以前のバージョンから移行する必要がある Exchange 2013  |[Exchange テクノロジへの移行](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|マネージ コードから Windows PowerShell を使用するカスタム管理ツール   |[Exchange 管理シェル](management/exchange-management-shell.md) |
|ソリューションのバックアップを作成または、Exchange データを復元するには  |[Exchange のバックアップ/リストア](backup-restore/backup-and-restore-for-exchange-2013.md) |
|トランスポート パイプラインでメッセージへのアクセスをサポートする拡張機能   |[Exchange のトランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md)  |
|モバイル デバイスをメールボックスのクライアント   |[Exchange ActiveSync](https://technet.microsoft.com/en-us/library/aa998357.aspx) |
   
## <a name="exchange-interactions-with-custom-applications"></a>カスタム アプリケーションと Exchange の相互作用

アプリケーションが Exchange に格納されたデータを使用して操作できるようにする技術もあれば、Exchange サーバーの管理および制御に使用する技術もあります。多くの場合、複数のプログラミング技術や言語を使用してタスクを実行することができます。これにより、使い慣れた技術と言語をを使えるようになります。たとえば、メールの REST API、EWS、または EWS Managed API を使用して、Exchange ストア内のアイテムのプロパティを設定できます。
  
Exchange は、アプリケーションのアーキテクチャと機能によって、さまざまな方法でカスタム アプリケーションと対話します。その中核で Exchange は、メッセージの送信だけでなく、メールボックスの維持、フォーム ベースのアプリケーションの実行なども行います。

|Exchange の相互作用|説明|
|:-----|:-----|
|**メッセージ トランスポート**|Exchange は、メッセージを送信するアプリケーションの標準メール サーバーの役割をします。<br/>Exchange には、REST、EWS、EWS Managed API などのメッセージを転送する複数の API が含まれます。<br/>加えて、メッセージが Exchange によって処理され、届けられる際に、アプリケーションはトランスポート エージェントを使用して応答できます。 |
|**メールボックス格納域** |Exchange は、メールボックスに格納されたデータにアクセスするアプリケーション向けに、フォルダー、アイテム、プロパティの階層構造を提供します。<br/>格納された情報には、データベースとコンポーネントのオブジェクト スタイルを組み合わせて使用することでアクセスできます。<br/>データのクエリを実行すると、Exchange は、ユーザーおよびストアのアクセス許可に基づいて、格納されたデータへのアクセスを管理します。<br/>一般的に、メールボックスのデータを処理するアプリケーションは、REST、EWS、または EWS Managed API を使用します。|
|**管理されているエンタープライズ サーバー** |Exchange は、Exchange サーバーとストアを管理するアプリケーション向けの管理対象サーバーとして機能します。<br/>アプリケーションは、組織全体で Exchange サーバーの現在のアクティビティと健康状態の設定、制御、監視を行えます。<br/>Exchange の管理アプリケーションは、Exchange 管理シェル を使用して Exchange サーバーを管理します。 |
   
## <a name="see-also"></a>関連項目

- [Exchange のサーバー API への参照](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [Office Blogs で Exchange について読む](https://www.microsoft.com/en-us/microsoft-365/blog/) 
- [Exchange 2013 の 101 コード サンプルの入手](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [EWS のマネージ API (GitHub) を取得します。](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Exchange Server のサポートを得る](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)


