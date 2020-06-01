---
title: Exchange 2013 の SOAP 自動検出 XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Exchange の SOAP 自動検出 web サービスの XML 要素参照情報を検索します。
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465185"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Exchange 2013 の SOAP 自動検出 XML 要素

Exchange の SOAP 自動検出 web サービスの XML 要素参照情報を検索します。
  
このセクションのドキュメントは、クライアントとサーバー間で送信される SOAP 自動検出 XML 要素のインスタンスに基づいています。 この XML インスタンスドキュメントは、SOAP 自動検出サービスをホストする仮想ディレクトリにある WSDL ファイルおよびスキーマファイルに基づいています。 認証されたユーザーは、次のいずれかのような URL を使用して、WSDL およびスキーマファイルを参照できます。
  
- WSDL ファイルの場所を指定し `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ます。`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- メッセージスキーマの場所を指定し `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ます。`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
SOAP 自動検出の WSDL ファイルおよびスキーマファイルの場所は、Exchange のインストールによって異なります。
  
メッセージ .xsd スキーマファイルは、自動検出 SOAP ヘッダーと SOAP 本文で送信できる XML 要素について説明します。 このファイルは、特定の要求と応答メッセージの相互作用に対して XML 構造をどのように使用できるかについての一般的なロードマップを提供します。 クライアントとサーバー間で送信される実際の XML 構造は、オプションと使用されるコンテキストに基づいています。 スキーマファイルでは、可能な XML が定義されています。 ネットワーク上で送信される実際の XML の範囲は、呼び出された操作、要求された情報、およびサーバー側の設定に基づいています。 
  
## <a name="related-sections"></a>関連情報

- [Exchange 用 SOAP 自動検出 Web サービス リファレンス](soap-autodiscover-web-service-reference-for-exchange.md)    
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)    
- [Exchange 用ユニファイドメッセージング web サービスのリファレンス](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

