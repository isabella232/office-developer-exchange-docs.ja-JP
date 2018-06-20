---
title: Exchange 2013 の自動検出の XML 要素を SOAP
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Exchange SOAP の自動検出 web サービスの XML 要素のリファレンス情報を検索します。
ms.openlocfilehash: 7201ef33060691df70b63d06b2045e1120b0610f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833517"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Exchange 2013 の自動検出の XML 要素を SOAP

Exchange SOAP の自動検出 web サービスの XML 要素のリファレンス情報を検索します。
  
このセクションのドキュメントは、クライアントとサーバー間で送信される SOAP の自動検出の XML の要素インスタンスに基づいています。 この XML インスタンス ドキュメントは、SOAP の自動検出サービスをホストする仮想ディレクトリに配置されている WSDL およびスキーマ ファイルに基づいています。 認証されたユーザーはことができます、次のいずれかのような URL を使用して、WSDL ファイルとスキーマ ファイルを参照してください。
  
- http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl またはhttp://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl: WSDL ファイルの場所です。
    
- http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd またはhttp://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd— メッセージのスキーマの場所です。
    
SOAP の自動検出の WSDL ファイルとスキーマ ファイルの場所は、Exchange のインストールによって異なります。
  
Messages.xsd スキーマ ファイルでは、自動検出の SOAP ヘッダーと SOAP 本体に送信される XML 要素について説明します。 このファイルは、特定の要求-応答のメッセージのやり取りをすることができます [XML データ構造の全般的なロードマップを提供します。 クライアントとサーバー間で送信される実際の XML 構造は、オプションとそれが使用されているコンテキストに基づきます。 スキーマ ファイルは、どのような XML が使用可能なを定義します。 実際の範囲の XML をネットワーク経由で送信されるは、どの操作が呼び出されると、要求された情報、およびサーバー側の設定に基づいています。 
  
## <a name="related-sections"></a>関連セクション
<a name="bk_RelatedSections"> </a>

- [Exchange の自動検出 web サービスの参照が SOAP します。](soap-autodiscover-web-service-reference-for-exchange.md)
    
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
    
- [Exchange ユニファイド メッセージング web サービス リファレンス](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

