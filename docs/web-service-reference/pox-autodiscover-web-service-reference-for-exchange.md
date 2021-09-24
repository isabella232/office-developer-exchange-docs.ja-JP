---
title: Exchange 用 POX 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: POX 自動検出サービスの参照情報は、Exchange。
ms.openlocfilehash: b28ea64a82960a84dee06c5055ee915614f4fde7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516420"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Exchange 用 POX 自動検出 Web サービス リファレンス

POX 自動検出サービスの参照情報は、Exchange。
  
自動検出サービスは、アプリケーションがサーバーサーバーへの接続を作成するために使用する構成情報Exchangeします。 "プレーン古い XML" (POX) 自動検出サービスを使用して、XML ペイロードだけで構成されるメッセージを送信し、SOAP エンベロープを囲まなくても、クライアント アプリケーションが Exchange に接続するために必要な設定を見つけることができます。
  
> [!NOTE]
> Exchange Server 2010 からバージョンの Exchange を対象とするクライアントの場合は、POX 自動検出サービスではなく SOAP 自動検出サービスを使用することをお勧めします。 2007 Exchangeクライアントは、POX 自動検出サービスを使用する必要があります。 堅牢で十分にテストされた POX 自動検出クライアントが.NET Framework EWS マネージ API を使用するクライアントをお勧めします。 EWS マネージ API の詳細については [、「EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)マネージ API クライアント アプリケーションの概要」を参照してください。 
  
このセクションでは、POX 自動検出要求リダイレクト中にクライアントとサーバーの間で送信される XML 要素と、応答で返されるユーザー設定について説明します。 XML 要素参照には、要素が表す内容の概要と、要素を使用する潜在的な要素階層の説明が含まれます。 このドキュメントでは、クライアントとサーバーの間で送信される XML インスタンスについて説明します。 POX 自動検出サービスには、明示的なスキーマは含みません。
  
このセクションの記事では、POX 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明を示します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [POX 自動検出要求のExchange](pox-autodiscover-request-for-exchange.md)
    
- [POX 自動検出応答のExchange](pox-autodiscover-response-for-exchange.md)
    
- [POX 自動検出 XML 要素のExchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)   
- [Exchange 用 SOAP 自動検出 Web サービス リファレンス](soap-autodiscover-web-service-reference-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

