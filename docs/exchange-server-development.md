---
title: Exchange Online と Exchange の開発
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Office 365 の一部としての Exchange Online とオンプレミスの exchange Server のバージョンを含む、Exchange Server の開発者向けの詳細なドキュメントを参照してください。
localization_priority: Priority
ms.openlocfilehash: 12a29ca07801561e7a746603d795468d9cb7491f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528497"
---
# <a name="exchange-online-and-exchange-development"></a>Exchange Online と Exchange の開発

Office 365 の一部としての Exchange Online とオンプレミスの exchange Server のバージョンを含む、Exchange Server の開発者向けの詳細なドキュメントを参照してください。

[方法]、[スタート]、[新機能]、および [API リファレンスドキュメント] を使用して、サービス、web サイト、デスクトップコンピューター、およびモバイルデバイスのメールボックスデータにアクセスして管理するためのツールを開発し、Exchange Online または Exchange 2010、2013、2016、および2019サーバーに格納されている電子メール、予定表、連絡先、

アプリケーションを開発するために、Graph API、REST API、Exchange Web サービス (EWS)、自動検出、Outlook アドイン、またはその他の Api を使用できます。 このページでは、適切な Exchange テクノロジを選択するための説明をします。

## <a name="exchange-developer-content"></a>Exchange の開発者向けコンテンツ

次の表を使って、開発目標の達成に役立つ技術と関連する API 内容を確認します。

> [!IMPORTANT]
> Microsoft Graph は、Exchange Online のデータへのアクセスで使用する、推奨 API です。 Exchange Online のデータへのアクセスのための新しいアプリケーションでは、Microsoft Graph を使用する必要があります。

|開発するもの|参照先|
|:-----|:-----|
|Office 365 の一部として Exchange Online にアクセスする REST ベースのアプリ。|[メール、予定表、連絡先用の Microsoft Graph の REST API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Outlook、Outlook Web App、または デバイス用 OWA 内の情報を表示する状況依存のアプリ。 |[Outlook アドインと Exchange の EWS](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|.NET Framework または Java に基づかないメールボックス クライアント。 |[Exchange の EWS マネージ API、EWS、Web サービスについて学ぶ](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|EWS にアクセスするために .NET Framework を使用するメールボックス クライアント。 |[EWS マネージ API クライアント アプリケーションの概要](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|EWS にアクセスするために Java を使用するメールボックス クライアント。 |[GitHub の EWS Java API](https://github.com/OfficeDev/ews-java-api) |
|Outlook ユーザー インターフェイスをカスタマイズする、または Outlook ビジネス ロジックに依存するアプリケーション。  |[Outlook VBA リファレンス](https://msdn.microsoft.com/VBA/VBA-Outlook) |
|Exchange Online または Exchange 2013 を対象とし、以前のバージョンの Exchange からの移行に必要なアプリケーション。  |[Exchange テクノロジへの移行](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|マネージ コードの Windows PowerShell を使うカスタム管理ツール。   |[Exchange 管理シェル](management/exchange-management-shell.md) |
|Exchange データのバックアップまたは復元を行うソリューション。  |[Exchange のバックアップと復元](backup-restore/backup-and-restore-for-exchange-2013.md) |
|トランスポート パイプライン内のメッセージのアクセスをサポートする拡張機能。   |[Exchange のトランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md)  |
|モバイル デバイス用のメールボックス クライアント。   |[Exchange ActiveSync](https://technet.microsoft.com/library/aa998357.aspx) |

## <a name="exchange-interactions-with-custom-applications"></a>Exchange とカスタム アプリケーションの相互作用

アプリケーションが Exchange に格納されたデータを使用して操作できるようにする技術もあれば、Exchange サーバーの管理および制御に使用する技術もあります。多くの場合、複数のプログラミング技術や言語を使用してタスクを実行することができます。これにより、使い慣れた技術と言語をを使えるようになります。たとえば、メールの REST API、EWS、または EWS Managed API を使用して、Exchange ストア内のアイテムのプロパティを設定できます。

Exchange は、アプリケーションのアーキテクチャと機能によって、さまざまな方法でカスタム アプリケーションと対話します。その中核で Exchange は、メッセージの送信だけでなく、メールボックスの維持、フォーム ベースのアプリケーションの実行なども行います。

|Exchange の相互作用|説明|
|:-----|:-----|
|**メッセージ トランスポート**|Exchange は、メッセージを送信するアプリケーションの標準的なメール サーバーとして機能します。<br/>Exchange には、REST、EWS、EWS Managed API などのメッセージを転送する複数の API が含まれます。<br/>さらに、Exchange により応答メッセージの処理と配信が行われるときに、アプリケーションはトランスポート エージェントを使用して応答することができます。 |
|**メールボックス記憶域** |Exchange は、メールボックスに格納されたデータにアクセスするアプリケーションにのために、フォルダー、アイテム、およびプロパティの階層構造を提供します。<br/>格納された情報には、データベースとコンポーネントのオブジェクト スタイルを組み合わせて使用することでアクセスできます。<br/>データのクエリを実行すると、Exchange は、ユーザーおよびストアのアクセス許可に基づいて、格納されたデータへのアクセスを管理します。<br/>通常、メールボックス データを処理するアプリケーションでは、REST、EWS、または EWS マネージ API が使用されます。|
|**管理されたエンタープライズ サーバー** |Exchange は、Exchange サーバーとストアを管理するアプリケーションの管理サーバーとして機能します。<br/>アプリケーションは、組織全体で Exchange サーバーの現在のアクティビティと健康状態の設定、制御、監視を行えます。<br/>Exchange 管理アプリケーションは、Exchange サーバーを管理するのに Exchange 管理シェルを使用します。 |

## <a name="see-also"></a>関連項目

- 
  [Exchange 用 EWS リファレンス](https://msdn.microsoft.com/library/dn186243(v=exchg.150).aspx)
- [Office ブログの Exchange に関する情報を読む](https://www.microsoft.com/microsoft-365/blog/)
- [Exchange 2013 の 101 のサンプル コードを取得する](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [EWS マネージ API の入手 (GitHub)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Exchange Server サポート情報](https://support.microsoft.com/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)
