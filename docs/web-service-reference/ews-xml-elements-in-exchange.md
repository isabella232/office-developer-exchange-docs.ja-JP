---
title: Exchange の EWS XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Exchange 内の EWS XML 要素に関する参照情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526117"
---
# <a name="ews-xml-elements-in-exchange"></a>Exchange の EWS XML 要素

Exchange 内の EWS XML 要素に関する参照情報を検索します。
  
Exchange Web サービス (EWS) は SOAP ベースの web サービスです。これは、クライアントとサーバー間で送信される要求メッセージと応答メッセージが XML 要素で構成されることを意味します。 このセクションのドキュメントは、クライアントとサーバー間で送信される XML インスタンスに基づいています。 XML インスタンスは、EWS をホストする仮想ディレクトリにある WSDL ファイルおよびスキーマファイルで定義されています。 認証されたユーザーの場合は、次の Url を使用して WSDL およびスキーマファイルを参照でき \<yourclientaccessserver\> ます。ここで、はクライアントアクセスサーバーの名前です。
  
- http:// \<yourclientaccessserver\> /ews/サービス wsdl ファイルの場所を指定します。
    
- http:// \<yourclientaccessserver\> /ews/メッセージ .xsd-メッセージスキーマの場所。
    
- http:// \<yourclientaccessserver\> /ews/型 .xsd-types スキーマの場所。
    
EWS XML 要素を記述するスキーマファイルは、要求と応答メッセージの相互作用に使用できる XML 構造の一般的なロードマップを提供します。 クライアントとサーバー間で送信される実際の XML 構造は、呼び出される操作、要求された情報、およびサーバー側の設定によって異なります。
  
EWS WSDL ファイルサービス wsdl は、wsdl 標準に完全に準拠していません。 wsdl サービス定義は含まれていません。 これは、EWS が事前に定義されたアドレスを持つコンピューターでホストされるように設計されていないためです。 自動検出サービスを使用して、EWS エンドポイントアドレスを取得できます。 一部のクライアント側オブジェクトモデルジェネレーターは、WSDL を解析し、wsdl ファイルに WSDL サービス定義が含まれていないため、エラーが発生することがあります。 オブジェクトモデルジェネレーターでエラーが発生した場合は、プレースホルダー WSDL サービス定義を挿入できます。
  
> [!TIP]
> .NET Framework を使用してアプリケーションを開発している場合は、オブジェクトモデルジェネレーターではなく、 [EWS マネージ API](http://aka.ms/ews-managed-api-readme)を使用することをお勧めします。 EWS マネージ API には、EWS XML のシリアル化と逆シリアル化を処理するための使いやすいオブジェクトモデルが用意されています。 詳細については、「 [EWS マネージ API クライアントアプリケーションの概要](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)」を参照してください。 
  
メッセージ .xsd スキーマファイルには、SOAP 本文の最上位レベルの要素の要素定義が含まれています。 エラー応答コード以外の場合、メッセージ .xsd の定義のほとんどは操作に固有のものです。 型 .xsd スキーマには、SOAP ヘッダーの定義と、操作間で共有されるすべての共通定義が含まれています。
  
## <a name="see-also"></a>関連項目

- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange での EWS 操作](ews-operations-in-exchange.md)
- [Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
    

