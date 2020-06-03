---
title: Exchange 用 SOAP 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Exchange の SOAP 自動検出サービスに関する参照情報を検索します。
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468426"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Exchange 用 SOAP 自動検出 Web サービス リファレンス

Exchange の SOAP 自動検出サービスに関する参照情報を検索します。
  
自動検出サービスは、アプリケーションが Exchange サーバーへの接続を作成するために使用する構成情報を提供します。 SOAP 自動検出サービスを使用して、クライアントアプリケーションと Exchange サーバーの間でメッセージを送信し、アプリケーションが Exchange への接続に使用する設定を見つけることができます。 POX 自動検出サービスとは異なり、SOAP 自動検出サービスは、多くのユーザーの設定についての自動検出要求をバッチ処理することを許可し、応答で返される設定をより細かく制御します。 
  
> [!NOTE]
> Exchange Server 2010 以降のバージョンの Exchange を対象とするクライアントの場合、SOAP 自動検出サービスを使用することをお勧めします (POX 自動検出サービスではありません)。 Exchange 2007 を対象とするクライアントは、POX 自動検出サービスを使用する必要があります。 .NET Framework を使用するクライアントは、堅牢で十分にテストされた SOAP 自動検出クライアントを含んでいるため、EWS マネージ API を使用することをお勧めします。 EWS マネージ API の詳細については、「 [Ews マネージ api クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。 
  
このセクションでは、SOAP 自動検出要求のリダイレクト時にクライアントとサーバー間で送信される XML 要素、および応答で返されるユーザー設定について説明します。 XML 要素リファレンスには、要素が表す内容の概要と、要素を含む可能性のある要素階層の説明が含まれています。 
  
このセクションの記事では、クライアントとサーバー間で送信される XML インスタンスについて説明します。 これらの要素を記述するスキーマは、SOAP 自動検出サービスをホストするサーバーの仮想ディレクトリにあります。
  
このセクションの WSDL 操作のトピックでは、操作の内容と操作の要求と応答の例について概要を説明します。 提供されているバージョン情報を使用して、使用する機能が、実行している製品バージョンで利用できるかどうかを判断できます。 また、操作のトピックの例では、サーバーとの間で送受信される SOAP メッセージに含まれる XML の構造を理解するのに役立ちます。
  
このセクションでは、SOAP 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明も示します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
    
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
    
- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
    
- [Get組織の Relationshipsettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Exchange 2013 の SOAP 自動検出 XML 要素](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目


- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [自動検出を使用して接続ポイントを検索する](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [自動検出を使用して Exchange からユーザー設定を取得する](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Exchange サーバーからドメイン設定を取得する](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

