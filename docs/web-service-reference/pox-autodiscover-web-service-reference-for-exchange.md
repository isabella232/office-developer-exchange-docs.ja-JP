---
title: Exchange の POX の自動検出 web サービスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Exchange POX の自動検出サービスに関するリファレンス情報を検索します。
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Exchange の POX の自動検出 web サービスの参照

Exchange POX の自動検出サービスに関するリファレンス情報を検索します。
  
自動検出サービスは、Exchange サーバーへの接続を作成するアプリケーションで使用される構成情報を提供します。 "標準古い XML"を使用することができます (POX) の自動検出サービスを Exchange に接続するためにクライアント アプリケーションに必要な設定を見つけるためにせず、それを囲む、SOAP エンベロープの XML ペイロードのみを含むメッセージを送信します。
  
> [!NOTE]
> バージョンの Exchange が Exchange Server 2010 で始まるを対象とするクライアントの場合は、POX の自動検出サービスではなく、SOAP の自動検出サービスを使用することをお勧めします。 Exchange 2007 を対象とするクライアントでは、POX の自動検出サービスを使用する必要があります。 .NET Framework を使用して、クライアントは、堅牢で十分にテストされた自動検出の POX クライアントが含まれているため、EWS のマネージ API を使用することをお勧めします。 EWS のマネージ API の詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。 
  
このセクションでは、POX の自動検出要求のリダイレクトと、応答で返されるユーザーの設定中にクライアントとサーバー間で送信される XML 要素に関する情報を提供します。 XML 要素の参照には、要素が表す内容の概要と要素を使用している潜在的な要素階層の説明が含まれています。 このドキュメントでは、クライアントとサーバー間で送信される XML インスタンスについて説明します。 POX の自動検出サービスには、明示的なスキーマがありません。
  
このセクションの記事では、POX の自動検出サービスを使用して、自動検出の構成情報を取得するために使用されるメッセージの説明や例を提供します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [POX の自動検出要求の交換](pox-autodiscover-request-for-exchange.md)
    
- [POX Exchange の自動検出の応答](pox-autodiscover-response-for-exchange.md)
    
- [交換の POX の自動検出の XML 要素](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)   
- [Exchange の自動検出 web サービスの参照が SOAP します。](soap-autodiscover-web-service-reference-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

