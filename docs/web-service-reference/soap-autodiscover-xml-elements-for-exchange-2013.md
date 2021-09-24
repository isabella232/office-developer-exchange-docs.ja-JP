---
title: SOAP 自動検出 XML 要素 (2013 Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: SOAP 自動検出 Web サービスの XML 要素参照情報は、次のExchange。
ms.openlocfilehash: 5dcf4d6cd7a2b0b2987e59530dfbaae7b9993242
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539095"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>SOAP 自動検出 XML 要素 (2013 Exchange)

SOAP 自動検出 Web サービスの XML 要素参照情報は、次のExchange。
  
このセクションのドキュメントは、クライアントとサーバーの間で送信される SOAP 自動検出 XML 要素インスタンスに基づいて作成されます。 この XML インスタンスのドキュメントは、SOAP 自動検出サービスをホストする仮想ディレクトリにある WSDL ファイルとスキーマ ファイルに基づいて作成されます。 認証されたユーザーは、次のいずれかの URL を使用して WSDL ファイルとスキーマ ファイルを参照できます。
  
- WSDL ファイルの場所: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` または `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- メッセージ スキーマの場所: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` または `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
SOAP 自動検出 WSDL ファイルとスキーマ ファイルの場所は、インストールの種類によってExchangeされます。
  
messages.xsd スキーマ ファイルは、自動検出 SOAP ヘッダーと SOAP 本文で送信できる XML 要素について説明します。 このファイルは、特定の要求と応答メッセージのやり取りに対して XML 構造が可能な一般的なロードマップを提供します。 クライアントとサーバーの間で送信される実際の XML 構造は、オプションと使用されるコンテキストに基づいて行います。 スキーマ ファイルは、可能な XML を定義します。 ワイヤーを使用して送信される XML の実際の範囲は、呼び出される操作、要求された情報、およびサーバー側の設定に基づいて行います。 
  
## <a name="related-sections"></a>関連情報

- [Exchange 用 SOAP 自動検出 Web サービス リファレンス](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)    
- [ユニファイド メッセージング Web サービスの参照Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 用自動検出 Web サービス リファレンス](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

