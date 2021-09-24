---
title: Exchange テクノロジへの移行
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 946a722f-0892-4a59-9e58-a291bfb6834a
description: 以前のバージョンの Exchange から移行する場合は、この記事の情報を使用して、現在の製品バージョンでサポートされている開発テクノロジと移行するテクノロジを確認します。
ms.openlocfilehash: 3885d6789cedf5de028b64a0658b336bd021b9ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527002"
---
# <a name="migrating-to-exchange-technologies"></a>Exchange テクノロジへの移行

以前のバージョンの Exchange から移行する場合は、この記事の情報を使用して、現在の製品バージョンでサポートされている開発テクノロジと移行するテクノロジを確認します。
  
## <a name="determine-if-your-technology-is-available-in-current-versions"></a>テクノロジが現在のバージョンで使用できるかどうかを確認する

次の表を使用して、2019 年の開発テクノロジが 2019 年Exchange OnlineかExchangeします。 テクノロジがサポートされていない場合は、「[移行先のテクノロジを選択する](#bk_choose)」を参照してください。

<br/> 

**Exchange開発テクノロジと製品バージョン**

|テクノロジ|Office 365 および Exchange Online|Exchange 2019|Exchange 2016|Exchange 2013|Exchange 2010|Exchange 2007|
|:-----|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|[Office 365 API プラットフォームの概要](https://msdn.microsoft.com/library/16fbf0c0-5470-466b-aab8-a0c9074c94e2%28Office.15%29.aspx) <br/> |X  <br/> |X²  <br/> |X¹ ²  <br/> ||
|[EWS Managed API](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Web サービス (EWS)](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Outlook 用のメール アプリ](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Outlook オブジェクト モデル (OOM)](https://msdn.microsoft.com/library/75e4ad96-62a2-49d2-bc51-48ceab50634c%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Exchange Management Shell](management/exchange-management-shell.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[バックアップと復元](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[トランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md) <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Active Directory サービス インターフェイス (ADSI)  <br/> ||||||X  <br/> |
|Collaborative Data Objects for Exchange (CDOEX)  <br/> ||||||X  <br/> |
|Collaborative Data Objects for Windows 2000 (CDOSYS)  <br/> ||||||X  <br/> |
|Exchange OLE DB プロバイダー (EXOLEDB)  <br/> ||||||X  <br/> |
|Exchange ストア イベント シンク  <br/> ||||||X  <br/> |
|Incremental Change Synchronization (ICS)  <br/> ||||||X  <br/> |
|ライトウェイト ディレクトリ アクセス プロトコル (LDAP)  <br/> ||||||X  <br/> |
|[メッセージ API (MAPI)](https://msdn.microsoft.com/library/3d980b86-7001-4869-9780-121c6bfc7275%28Office.15%29.aspx) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> | 
|Outlook Web App のカスタマイズ  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Web Distributed Authoring and Versioning (WebDAV)  <br/> ||||||X  <br/> |

<a name="bk_choose"> </a>

¹REST API と Graph API には、2016 年の累積的な更新プログラム 3 Exchangeがあります。

²Only ハイブリッドのお客様は、ハイブリッド メールボックスとオンプレミス メールボックスの両方Office 365 REST API を利用できます。

## <a name="choose-a-development-technology-to-migrate-to"></a>移行先の開発テクノロジを選択する

Exchange Online または Exchange 2013 でアプリケーションが使用するテクノロジがサポートされていない場合や、Exchange でサポートされていない場合は、次の表を使用して、移行するテクノロジを決定します。
  
**推奨されるテクノロジの移行パス**

|**テクノロジ**|**2019 年Office 365、Exchange Online、Exchangeでサポートされていますか?**|**移行先**|**詳細情報**|
|:-----|:-----|:-----|:-----|
|ADSI  <br/> |はい (ただし、非推奨) <br/>|[Exchange Management Shell](management/exchange-management-shell.md)<br/> |なし。  <br/> |
|CDOEX  <br/> |いいえ  <br/> |[EWS Managed API または EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |EWS Managed API と EWS は、CDOEX が提供するものと同じ Exchange ストアにアクセスできます。CDOEX を使用して作成されたクライアント プリケーションとは異なり、EWS アプリケーションはローカルまたはリモートのコンピューター上で実行できます。  <br/> |
|CDOEXM  <br/> |いいえ <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |Exchange 管理シェルのコマンドにより、Exchange サーバー、ストレージ グループ、データベース、およびユーザーの制御は、そのコマンドに対応する CDOEXM API よりも簡単になります。さらに、カスタムの CDOEXM アプリケーションは、Exchange 管理シェルのコマンドに簡単に移行できます。  <br/> |
|CDOSYS<br/> |いいえ<br/> |[トランスポート エージェント](transport-agents/transport-agents-in-exchange-2013.md)   <br/> |トランスポート エージェントは、2010 年から始まるバージョンExchange通知ベースのアプリケーションExchange使用します。<br/><br/> CDOSYS は、現行バージョンの Windows に含まれています。CDOSYS の機能は、.NET Framework で使用できます。  <br/> |
|CDOWF  <br/> |いいえ  <br/> |[Windowsワークフローファンデーション (WWF)](https://msdn.microsoft.com/library/vstudio/ms735967%28v=vs.90%29.aspx) <br/> |WWF を使用して、2007 年に使用する高度なワークフロー Exchangeできます。   <br/> |
|ExOLEDB  <br/> |いいえ  <br/> |[EWS Managed API または EWS](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) <br/> |EWS マネージ API と EWS は、ExOLEDB が提供Exchangeストアに同じアクセスを提供します。 ExOLEDB を使用して作成されたクライアント プリケーションとは異なり、EWS アプリケーションはローカルまたはリモートのコンピューター上で実行できます。  <br/> |
|ICS  <br/> |はい (ただし、非推奨)  <br/> |EWS Managed API または EWS<br/> |EWS Managed API または EWS は、[通知のサブスクライブ](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)と[メールボックス データの同期](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)に使用できます。  <br/> |
|LDAP  <br/> |はい (ただし、非推奨)  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |なし。  <br/> |
|MAPI  <br/> |はい (ただし、非推奨)  <br/> |Office 365API プラットフォームの概要、EWS マネージ API、EWS <br/> |MAPI は現時点でサポート対象の開発テクノロジですが、最終的に、カスタムの MAPI アプリケーションは、より新しいテクノロジを使用するように再設計することが必要になります。<br/><br/>MAPI アプリケーションがメール、予定表、連絡先オブジェクト、およびターゲット Office 365、Exchange 2019²、または Exchange 2016¹ ² に対して簡単な読み取り、書き込み、および更新操作を実行している場合は、メール、予定表、連絡先に[Office 365 REST API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)を使用できます。<br/><br/>Exchange オンプレミスをターゲットにしている場合、MAPI がアクセスできるすべてのプロパティにアクセスする必要がある場合は、EWS マネージ API または EWS を使用し、スキーマ化されたプロパティまたは拡張プロパティを[使用できます](https://msdn.microsoft.com/library/68623048-060e-4602-b3fa-62617a94cf72%28Office.15%29.aspx)。<br/><br/>**メモ**: [ExtendedPropertyDefinition](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) クラスは EWS マネージ API から MAPI にアクセスし [、ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素は EWS から MAPI プロパティにアクセスできます。           |
|Outlook Web App のカスタマイズ  <br/> |いいえ  <br/> |[メール アプリ](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |なし。  <br/> |
|ストア イベント シンク  <br/> |いいえ  <br/> |EWS Managed API または EWS <br/> |EWS Managed API または EWS は、[通知のサブスクライブ](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)と[メールボックス データの同期](exchange-web-services/mailbox-synchronization-and-ews-in-exchange.md)に使用できます。<br/><br/>EWS の通知は、ストア イベント シンクが提供するものと同じ Exchange ストアへのアクセスを提供します。 EWS をVisual Studioするストア イベント対応クライアント アプリケーションの開発を効率化するために、このツールを使用できます。  <br/> |
|ストリーミング バックアップと復元  <br/> |いいえ  <br/> |[ボリューム シャドウ コピー サービス (VSS) ライター](backup-restore/backup-and-restore-for-exchange-2013.md) <br/> |なし。  <br/> |
|WebDAV  <br/> |いいえ  <br/> |Office 365API プラットフォームの概要、EWS マネージ API または EWS <br/> |WebDAV アプリケーションがメール、予定表、または連絡先オブジェクトに対して簡単な読み取り、書き込み、更新操作を実行し、Office 365、Exchange 2019²、または Exchange 2016¹ ² を対象とする場合は、メール、予定表、連絡先に[Office 365 REST API](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md)を使用できます。<br/><br/>それ以外の場合は、Exchange オンプレミスをターゲットにしている場合に、WebDAV が提供する Exchange ストア内の同じプロパティにアクセスする必要がある場合は、EWS マネージ API または EWS を使用します。  <br/> |
|WebDAV 通知  <br/> |いいえ  <br/> |EWS Managed API または EWS<br/> |EWS Managed API または EWS は、[通知のサブスクライブ](exchange-web-services/notification-subscriptions-mailbox-events-and-ews-in-exchange.md)に使用できます。  <br/> |
|Web フォーム  <br/> |いいえ  <br/> |[ASP.NET](http://www.asp.net/web-forms) <br/> |ASP.NET に切り替えて、EWS を使用してメールボックスとサーバー情報にアクセスするようにアプリケーションを更新します。  <br/> |
|WMI プロバイダー  <br/> |いいえ  <br/> |[Exchange Management Shell](management/exchange-management-shell.md) <br/> |なし。  <br/> |
   
¹REST API と Graph API には、2016 年の累積的な更新プログラム 3 Exchangeがあります。

²Only ハイブリッドのお客様は、ハイブリッド メールボックスとオンプレミス メールボックスの両方Office 365 REST API を利用できます。

## <a name="see-also"></a>関連項目

- [Outlook 用のソリューションを開発するための API またはテクノロジの選択](https://msdn.microsoft.com/library/01a46083-03d0-4333-920c-01a9f17f68cb%28Office.15%29.aspx)
- [REST API のオンプレミス アーキテクチャ要件](https://blogs.technet.microsoft.com/exchange/2016/09/26/on-premises-architectural-requirements-for-the-rest-api/)    
