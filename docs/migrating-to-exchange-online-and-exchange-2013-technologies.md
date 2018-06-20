---
title: 交換テクノロジへの移行
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: Exchange の以前のバージョンから移行する場合、この資料の情報を使用して、開発技術は、現在の製品バージョンでは、サポートされてし、どちらのテクノロジに移行します。
ms.openlocfilehash: 82362b7bcdb79d6ca43603335d51a8bd8c1df239
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759226"
---
# <a name="migrating-to-exchange-technologies"></a>交換テクノロジへの移行

Exchange の以前のバージョンから移行する場合、この資料の情報を使用して、開発技術は、現在の製品バージョンでは、サポートされてし、どちらのテクノロジに移行します。
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>テクノロジーは、現在のバージョンで利用可能なかどうかを決定します。

かどうかの開発テクノロジがサポートされている Exchange オンラインまたは Exchange 2013 を決定するのにには、次の表を使用します。 テクノロジがサポートされていない場合は、[開発技術への移行の選択](#bk_choose)を参照してください。

<br/> 

**Exchange 開発テクノロジや製品バージョン**

|テクノロジ|Office 365 および Exchange オンライン|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|
|[Office 365 API プラットフォームの概要](http://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> ||||
|[EWS Managed API](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Web サービス (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Outlook 用メール アプリ](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |||
|[Outlook オブジェクト モデル (OOM)](http://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange 管理シェル](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[バックアップと復元](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |
|[トランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |
|Active Directory サービス インターフェイス (ADSI)  <br/> ||||X  <br/> |
|Collaborative Data Objects for Exchange (CDOEX)  <br/> ||||X  <br/> |
|Collaborative Data Objects for Windows 2000 (CDOSYS)  <br/> ||||X  <br/> |
|Exchange OLE DB プロバイダー (EXOLEDB)  <br/> ||||X  <br/> |
|Exchange ストア イベント シンク  <br/> ||||X  <br/> |
|Incremental Change Synchronization (ICS)  <br/> ||||X  <br/> |
|ライトウェイト ディレクトリ アクセス プロトコル (LDAP)  <br/> ||||X  <br/> |
|[メッセージ API (MAPI)](http://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Outlook Web App のカスタマイズ  <br/> |||X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||X  <br/> |

<a name="bk_choose"> </a>

## <a name="choose-a-development-technology-to-migrate-to"></a>移行先の開発テクノロジを選択する

アプリケーションを使用してテクノロジがサポートされていないか、オンラインまたは Exchange 2013 Exchange deemphasized 場合、は、テクノロジへの移行を決定するのには次の表を使用します。
  
**テクノロジーの推奨される移行パス**

|**テクノロジー**|**Office 365 は、オンラインでの Exchange および Exchange 2013 でサポートされているでしょうか。**|**移行します。**|**詳細情報**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |はい (ただし、非推奨) <br/>|[Exchange 管理シェル](management/exchange-management-shell.md)<br/> |なし  <br/> |
|CDOEX  <br/> |いいえ  <br/> |[EWS はマネージ API または EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |EWS Managed API と EWS は、CDOEX が提供するものと同じ Exchange ストアにアクセスできます。CDOEX を使用して作成されたクライアント プリケーションとは異なり、EWS アプリケーションはローカルまたはリモートのコンピューター上で実行できます。  <br/> |
|CDOEXM  <br/> |いいえ <br/> |[Exchange 管理シェル](management/exchange-management-shell.md) <br/> |Exchange 管理シェルのコマンドにより、Exchange サーバー、ストレージ グループ、データベース、およびユーザーの制御は、そのコマンドに対応する CDOEXM API よりも簡単になります。さらに、カスタムの CDOEXM アプリケーションは、Exchange 管理シェルのコマンドに簡単に移行できます。  <br/> |
|CDOSYS<br/> |いいえ<br/> |[トランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |Exchange が Exchange 2010 以降のバージョンで動作する、通知ベースのアプリケーション用には、トランスポート エージェントを使用します。<br/><br/> CDOSYS は、現行バージョンの Windows に含まれています。CDOSYS の機能は、.NET Framework で使用できます。  <br/> |
|CDOWF  <br/> |いいえ  <br/> |[Windows ワークフロー Foundation (WWF)](http://msdn.microsoft.com/en-us/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |WWF を使用すると、Exchange 2007 を操作する高度なワークフロー アプリケーションを作成します。   <br/> |
|ExOLEDB  <br/> |いいえ  <br/> |[EWS はマネージ API または EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |EWS のマネージ API および EWS は、ExOLEDB を提供する Exchange ストアへのアクセスを提供します。 ExOLEDB を使用して構築された、クライアント アプリケーションとは異なり、ローカルまたはリモート コンピューターで EWS アプリケーションを実行できます。  <br/> |
|ICS  <br/> |はい (ただし、非推奨)  <br/> |EWS はマネージ API または EWS<br/> |EWS のマネージ API または EWS を使用するには、[通知をサブスクライブ](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)し、[メールボックスのデータを同期](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)します。  <br/> |
|LDAP  <br/> |はい (ただし、非推奨)  <br/> |[Exchange 管理シェル](management/exchange-management-shell.md) <br/> |なし  <br/> |
|MAPI  <br/> |はい (ただし、非推奨)  <br/> |Office 365 の Api プラットフォームの概要、EWS マネージ API では、EWS <br/> |MAPI は現時点でサポート対象の開発テクノロジですが、最終的に、カスタムの MAPI アプリケーションは、より新しいテクノロジを使用するように再設計することが必要になります。<br/><br/>単純な読み取り、書き込み、およびメール、予定表、または連絡先オブジェクト、および Office 365 のターゲットの更新操作は、MAPI アプリケーションが実行している場合は、[メール、カレンダー、および連絡先の Office 365 の REST Api](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)を使用できます。<br/><br/>交換設置を対象としている場合は、MAPI にアクセスできるすべてのプロパティにアクセスする必要があります、EWS のマネージ API または EWS およびいずれか、[またはスキーマのプロパティの拡張プロパティ](http://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)を使用できます。<br/><br/>**注**: [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx)クラスは、EWS のマネージ API から MAPI へアクセスを提供し、 [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)要素は、EWS の MAPI プロパティにアクセスを提供します。           |
|Outlook Web App のカスタマイズ  <br/> |いいえ  <br/> |[メール アプリケーション](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |なし  <br/> |
|ストア イベント シンク  <br/> |いいえ  <br/> |EWS はマネージ API または EWS <br/> |EWS のマネージ API または EWS を使用するには、[通知をサブスクライブ](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)し、[メールボックスのデータを同期](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)します。<br/><br/>EWS での通知では、ストア イベント シンクを提供する Exchange ストアへのアクセスを提供します。 Visual Studio ツールを使用すると、EWS を使用するストア イベントに対応したクライアント アプリケーションの開発を合理化します。  <br/> |
|ストリーミング バックアップと復元  <br/> |いいえ  <br/> |[ボリューム シャドウ コピー サービス (VSS) ライター](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |なし  <br/> |
|WebDAV  <br/> |いいえ  <br/> |Office 365 の Api プラットフォームの概要、EWS のマネージ API または EWS <br/> |WebDAV アプリケーションは、単純な読み取り、書き込み、およびメール、予定表、または連絡先オブジェクトは、更新操作を実行して、Office 365 を対象とするが場合、は、[メール、カレンダー、および連絡先の Office 365 の REST Api](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)を使用します。<br/><br/>それ以外の場合、Exchange の設置型を対象としているし、Exchange ストア内の同じプロパティにアクセスする必要がある場合、WebDAV が用意されています、EWS のマネージ API または EWS を使用します。  <br/> |
|WebDAV 通知  <br/> |いいえ  <br/> |EWS はマネージ API または EWS<br/> |EWS のマネージ API または EWS を使用するには、[通知を](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)サブスクライブします。  <br/> |
|Web フォーム  <br/> |いいえ  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |ASP.NET に切り替えて、EWS を使用してメールボックスとサーバー情報にアクセスするようにアプリケーションを更新します。  <br/> |
|WMI プロバイダー  <br/> |いいえ  <br/> |[Exchange 管理シェル](management/exchange-management-shell.md) <br/> |なし。  <br/> |
   
## <a name="see-also"></a>関連項目

- [API または Outlook のソリューションを開発するためのテクノロジーを選択](http://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
    

