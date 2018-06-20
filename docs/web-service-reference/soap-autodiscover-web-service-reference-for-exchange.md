---
title: Exchange の自動検出 web サービスの参照が SOAP します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Exchange SOAP の自動検出サービスに関するリファレンス情報を検索します。
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Exchange の自動検出 web サービスの参照が SOAP します。

Exchange SOAP の自動検出サービスに関するリファレンス情報を検索します。
  
自動検出サービスは、Exchange サーバーへの接続を作成するアプリケーションで使用される構成情報を提供します。 SOAP の自動検出サービスを使用すると、アプリケーションが Exchange への接続を使用して、設定を確認するのにには、クライアント アプリケーションと Exchange サーバー間でメッセージを送信します。 POX の自動検出サービスとは異なり SOAP の自動検出サービスは多くのユーザーの設定とより詳細に制御する設定は応答の自動検出要求のバッチ処理のことができます。 
  
> [!NOTE]
> バージョンの Exchange が Exchange Server 2010 で始まるを対象とするクライアントは、SOAP の自動検出サービスではなく、POX 自動検出サービス) を使用することをお勧めします。 Exchange 2007 を対象とするクライアントでは、POX の自動検出サービスを使用する必要があります。 .NET Framework を使用して、クライアントは、堅牢で十分にテストされた自動検出の SOAP クライアントが含まれているため、EWS のマネージ API を使用することをお勧めします。 EWS のマネージ API の詳細については、 [EWS のマネージ API のクライアント アプリケーションを使い始める](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx)を参照してください。 
  
このセクションでは、SOAP の自動検出要求のリダイレクトと、応答で返されるユーザーの設定中にクライアントとサーバー間で送信される XML 要素に関する情報を提供します。 XML 要素の参照には、要素が表す内容の概要と要素が含まれている潜在的な要素階層の説明が含まれています。 
  
このセクションの記事では、クライアントとサーバー間で送信される XML インスタンスについて説明します。 これらの要素を記述するスキーマは、SOAP の自動検出サービスをホストしているサーバーの仮想ディレクトリにあります。
  
どのような操作の概要についてはこのセクションのトピックでは、WSDL 操作と操作の要求と応答の例です。 使用する機能を実行している製品のバージョンで使用できるかどうかを判断するのにはバージョン情報を使用することができます。 操作のトピックの例では、サーバーとの間に送信される SOAP メッセージに含まれる XML の構造を理解することができます。
  
このセクションでは、SOAP の自動検出サービスを使用して、自動検出の構成情報を取得するために使用されるメッセージの説明や例も提供します。 
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_InThisSection"> </a>

- [GetDomainSettings 操作 (SOAP)](getdomainsettings-operation-soap.md)
    
- [GetFederationInformation 操作 (SOAP)](getfederationinformation-operation-soap.md)
    
- [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)
    
- [GetOrganizationRelationshipSettings 操作 (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Exchange 2013 の自動検出の XML 要素を SOAP](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の自動検出 web サービスの参照](autodiscover-web-service-reference-for-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
- [自動検出を使用してコネクション ポイントを検索するには](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Exchange から自動検出を使用してユーザー設定を取得します。](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Exchange サーバーからドメインの設定を取得します。](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
    

