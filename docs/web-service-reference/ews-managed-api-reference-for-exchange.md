---
title: Exchange Web サービス (EWS) マネージド API リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6ca36f4-a67c-4e3c-aae7-9ead7b704e15
description: EWS マネージド API に含まれる名前空間について説明します。
ms.openlocfilehash: 78797ba5124cb47da5430491d3be23bbaf0371a7
ms.sourcegitcommit: 25cbbc6707e4ec0621c5c46baf7fe49be42d3297
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/07/2018
ms.locfileid: "25440984"
---
# <a name="ews-managed-api-reference"></a>EWS マネージド API リファレンス

**適用対象**: EWS マネージド API | Exchange Online | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 | Office 365

Exchange Web サービス (EWS) マネージド API には、Microsoft.Exchange.WebServices.dll と Microsoft.Exchange.WebServices.Auth.dll の 2 つの API が含まれます。

## <a name="ews-managed-api-namespaces"></a>EWS マネージド API の名前空間

|名前空間 |説明 |
|:---------|:-----------|
|[Microsoft.Exchange.WebServices.Auth.Validation](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.auth.validation?view=exchange-ews-api) |Exchange サーバーから送信されたユーザー ID のトークンの検証に使用されるタイプとメソッドが含まれています。 Microsoft.Exchange.WebServices.Auth.Validation 名前空間は、Exchange Online および Exchange Server 2013 以降のバージョンの Exchange を対象とするクライアントに適用されます。 この名前空間は、Microsoft.Exchange.WebServices.Auth.dll API に含まれています。|
|[Microsoft.Exchange.WebServices.Autodiscover](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover?view=exchange-ews-api)|Exchange Server によってホストされる自動検出サービスとの通信に使用されるタイプが含まれています。 Active Directory Domain Services (AD DS) でサービス接続ポイント オブジェクトを検索する際にも、この名前空間を使用します。 自動検出サービスは EWS クライアントに構成情報を提供します。 これにより、クライアントは該当するサービスの URL を対象にすることができます。<br/><br/>クライアントがドメインに結合されている場合、あるいは Exchange Server 2010 で導入された SOAP 自動検出エンドポイントである場合は、この名前空間の機能を活用して、Microsoft Exchange Server 2007 で導入された POX 自動検出サービスを適用対象とし、サービス接続ポイント オブジェクトの検索を行うことができます。 この名前空間の主なタイプは [AutodiscoverService クラス](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover.autodiscoverservice?view=exchange-ews-api)になります。 この名前空間は、Microsoft.Exchange.WebServices.dll API に含まれています。|
|[Microsoft.Exchange.WebServices.Data](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data?view=exchange-ews-api)| EWS による Exchange サーバーとの通信に使用するタイプが含まれています。 この名前空間にはEWS マネージド API の中心的な機能が備わっています。 この名前空間の主なタイプは [ExchangeService クラス](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice?view=exchange-ews-api)になります。|

## <a name="see-also"></a>関連項目

- [Exchange の Web サービス リファレンス](web-services-reference-for-exchange.md)
- [Exchange の EWS マネージド API、EWS、Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [EWS およびその他の Exchange の Web サービスの新機能](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の Web サービス クライアントを開発する](../exchange-web-services/develop-web-service-clients-for-exchange.md)

