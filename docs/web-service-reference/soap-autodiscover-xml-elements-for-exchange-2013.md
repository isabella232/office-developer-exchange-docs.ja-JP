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
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353393"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Exchange 2013 の自動検出の XML 要素を SOAP

Exchange SOAP の自動検出 web サービスの XML 要素のリファレンス情報を検索します。
  
このセクションのドキュメントは、クライアントとサーバー間で送信される SOAP の自動検出の XML の要素インスタンスに基づいています。 この XML インスタンス ドキュメントは、SOAP の自動検出サービスをホストする仮想ディレクトリに配置されている WSDL およびスキーマ ファイルに基づいています。 認証されたユーザーはことができます、次のいずれかのような URL を使用して、WSDL ファイルとスキーマ ファイルを参照してください。
  
- WSDL ファイルの場所:`http://<yourclientaccessserver>.com/autodiscover/services.wsdl`または`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- メッセージ スキーマの場所:`http://<yourclientaccessserver>.com/autodiscover/messages.xsd`または`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
SOAP の自動検出の WSDL ファイルとスキーマ ファイルの場所は、Exchange のインストールによって異なります。
  
Messages.xsd スキーマ ファイルでは、自動検出の SOAP ヘッダーと SOAP 本体に送信される XML 要素について説明します。 このファイルは、特定の要求-応答のメッセージのやり取りをすることができます [XML データ構造の全般的なロードマップを提供します。 クライアントとサーバー間で送信される実際の XML 構造は、オプションとそれが使用されているコンテキストに基づきます。 スキーマ ファイルは、どのような XML が使用可能なを定義します。 実際の範囲の XML をネットワーク経由で送信されるは、どの操作が呼び出されると、要求された情報、およびサーバー側の設定に基づいています。 
  
## <a name="related-sections"></a>関連情報

- [Exchange の自動検出 web サービスの参照が SOAP します。](soap-autodiscover-web-service-reference-for-exchange.md)    
- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)    
- [Exchange ユニファイド メッセージング web サービス リファレンス](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

