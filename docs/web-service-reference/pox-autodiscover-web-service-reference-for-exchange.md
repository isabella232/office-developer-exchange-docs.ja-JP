---
title: Exchange 用 POX 自動検出 Web サービス リファレンス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Exchange の POX 自動検出サービスに関する参照情報を検索します。
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465654"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Exchange 用 POX 自動検出 Web サービス リファレンス

Exchange の POX 自動検出サービスに関する参照情報を検索します。
  
自動検出サービスは、アプリケーションが Exchange サーバーへの接続を作成するために使用する構成情報を提供します。 "プレーン旧 XML" (POX) 自動検出サービスを使用すると、クライアントアプリケーションが Exchange に接続するために必要な設定を特定するために、XML ペイロードのみで構成されたメッセージを、それを囲む SOAP エンベロープを使用せずに送信できます。
  
> [!NOTE]
> Exchange Server 2010 以降のバージョンの Exchange を対象とするクライアントでは、POX 自動検出サービスの代わりに SOAP 自動検出サービスを使用することをお勧めします。 Exchange 2007 を対象とするクライアントは、POX 自動検出サービスを使用する必要があります。 .NET Framework を使用するクライアントには、堅牢で十分にテストされた POX 自動検出クライアントが含まれているため、EWS マネージ API を使用することをお勧めします。 EWS マネージ API の詳細については、「 [Ews マネージ api クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。 
  
このセクションでは、POX 自動検出要求のリダイレクト時にクライアントとサーバー間で送信される XML 要素、および応答で返されるユーザー設定について説明します。 XML 要素リファレンスには、要素が表す内容の概要と、要素を使用する可能性のある要素階層の説明が含まれています。 このドキュメントでは、クライアントとサーバー間で送信される XML インスタンスについて説明します。 POX 自動検出サービスには、明示的なスキーマがありません。
  
このセクションの記事では、POX 自動検出サービスを使用して自動検出構成情報を取得するために使用されるメッセージの例と説明を示します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [POX Exchange の自動検出要求](pox-autodiscover-request-for-exchange.md)
    
- [POX Exchange の自動検出応答](pox-autodiscover-response-for-exchange.md)
    
- [Exchange の POX 自動検出 XML 要素](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)   
- [Exchange 用 SOAP 自動検出 Web サービス リファレンス](soap-autodiscover-web-service-reference-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

