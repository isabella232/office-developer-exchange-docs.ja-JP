---
title: Exchange での EWS の XML 要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Exchange EWS XML のリファレンス情報について要素を検索します。
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760354"
---
# <a name="ews-xml-elements-in-exchange"></a>Exchange での EWS の XML 要素

Exchange EWS XML のリファレンス情報について要素を検索します。
  
Exchange Web サービス (EWS) では、SOAP ベースの web サービス、クライアントとサーバー間で送信される要求と応答メッセージは、XML 要素で構成することを意味します。 このセクションのドキュメントは、クライアントとサーバー間で送信される XML インスタンスに基づいています。 XML インスタンスは、EWS をホストする仮想ディレクトリに配置されている WSDL およびスキーマ ファイルで定義されます。 次の Url を使用して、WSDL ファイルとスキーマ ファイルを参照することが認証されたユーザーの場合は、場所\<yourclientaccessserver\>は、クライアント アクセス サーバーの名前。
  
- http://\<yourclientaccessserver\>.com/ews/services.wsdl: WSDL ファイルの場所です。
    
- http://\<yourclientaccessserver\>.com/ews/messages.xsd-メッセージのスキーマの場所です。
    
- http://\<yourclientaccessserver\>.com/ews/types.xsd-タイプのスキーマの場所です。
    
EWS の XML 要素を記述するスキーマ ファイルは、要求-応答メッセージのやり取りの可能な XML データ構造の全般的なロードマップを提供します。 クライアントとサーバー間で送信される実際の XML 構造は、操作と呼ばれる、要求された情報をサーバー側の設定によって異なります。
  
EWS の WSDL ファイル、services.wsdl、完全に準拠していない標準の WSDL サービスの WSDL 定義が含まれていないためです。 これは、EWS が定義済みのアドレスを持つコンピューターでホストされるように設計されていませんので。 自動検出サービスを使用すると、EWS のエンドポイントのアドレスを取得します。 いくつかクライアント側オブジェクト モデルのジェネレーターでは、WSDL を解析し、WSDL ファイルにはサービスの WSDL 定義が含まれていないために、エラー状態が発生することができます。 オブジェクト モデルのジェネレーターには、エラーが発生すると、サービスの WSDL 定義のプレース ホルダーを挿入できます。
  
> [!TIP]
> アプリケーションを開発するのには.NET Framework を使用する場合、オブジェクト モデルのジェネレーターではなく、 [EWS のマネージ API](http://aka.ms/ews-managed-api-readme)を使用することをお勧めします。 EWS のマネージ API では、EWS の XML を逆シリアル化とシリアル化を処理するために使用するオブジェクト モデルを提供します。 詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。 
  
Messages.xsd スキーマ ファイルには、SOAP 本文内の最上位の要素の要素定義が含まれています。 エラー応答コードを除いては、messages.xsd 内の定義のほとんどは、操作に固有です。 Types.xsd スキーマには、SOAP ヘッダーの定義と操作の間で共有されているすべての一般的な定義が含まれています。
  
## <a name="see-also"></a>関連項目

- 
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)
- [Exchange での EWS の操作](ews-operations-in-exchange.md)
- [Exchange、EWS の管理 API、EWS、および web サービスを探索します。](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
    

