---
title: Exchange 用 SOAP 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: SOAP 自動検出サービスの参照情報は、Exchange。
ms.openlocfilehash: 488862f5797abfd71d33c916fa96970ab300a2c0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521355"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Exchange 用 SOAP 自動検出 Web サービス リファレンス

SOAP 自動検出サービスの参照情報は、Exchange。
  
自動検出サービスは、アプリケーションがサーバーサーバーへの接続を作成するために使用する構成情報Exchangeします。 SOAP 自動検出サービスを使用して、クライアント アプリケーションと Exchange サーバーの間でメッセージを送信して、アプリケーションが Exchange に接続するために使用する設定を特定できます。 POX 自動検出サービスとは異なり、SOAP 自動検出サービスでは、多くのユーザーの設定に対するバッチ処理された自動検出要求と、応答で返される設定の詳細な制御が可能です。 
  
> [!NOTE]
> Exchange Server 2010 から Exchange のバージョンを対象とするクライアントの場合は、(POX 自動検出サービスではなく) SOAP 自動検出サービスを使用することをお勧めします。 2007 Exchangeクライアントは、POX 自動検出サービスを使用する必要があります。 堅牢で十分にテストされた SOAP 自動検出クライアントが.NET Framework EWS マネージ API を使用するクライアントをお勧めします。 EWS マネージ API の詳細については [、「EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)マネージ API クライアント アプリケーションの概要」を参照してください。 
  
このセクションでは、SOAP 自動検出要求リダイレクト中にクライアントとサーバーの間で送信される XML 要素と、応答で返されるユーザー設定について説明します。 XML 要素参照には、要素が表す内容の概要と、要素を含む潜在的な要素階層の説明が含まれます。 
  
このセクションの記事では、クライアントとサーバーの間で送信される XML インスタンスについて説明します。 これらの要素を記述するスキーマは、SOAP 自動検出サービスをホストするサーバーの仮想ディレクトリにあります。
  
このセクションの WSDL 操作のトピックでは、操作の動作の概要と、操作の要求と応答の例を示します。 提供されたバージョン情報を使用して、使用する機能が実行中の製品バージョンで使用できるかどうかを判断できます。 操作のトピックの例は、サーバーとの間で送信される SOAP メッセージに含まれる XML の構造を理解するのにも役立ちます。
  
このセクションでは、SOAP 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明も示します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
    
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
    
- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
    
- [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [SOAP 自動検出 XML 要素 (2013 Exchange)](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目


- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [自動検出を使用して接続ポイントを検索する](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [自動検出を使用して Exchange からユーザー設定を取得する](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Exchange サーバーからドメイン設定を取得する](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

