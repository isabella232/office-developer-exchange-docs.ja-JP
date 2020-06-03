---
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.assetid: 6c969133-6036-448b-af39-a3caf9917e98
description: Exchange の web サービスに関する参照情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 8bdb3d6c4244bf8e0f092f5a9ffa3de5e8f1c3c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467348"
---
# <a name="web-services-reference-for-exchange"></a>Exchange の Web サービス リファレンス

Exchange の web サービスに関する参照情報を検索します。
  
このセクションには、exchange Online に含まれる Api、Office 365 の一部としての Exchange Online、Exchange Server 2007 以降の exchange のバージョンに関するリファレンス情報が記載されています。 このセクションには次のコンテンツが含まれています。
  
- [Exchange 用 ews リファレンス](ews-reference-for-exchange.md): Exchange Web サービス (EWS) API の api リファレンスドキュメントが含まれています。 これは、メールボックス情報へのアクセスを取得するために Exchange に接続するクライアントおよびサービスを作成するための主な API です。 このコンテンツには、EWS で利用できる操作に関する情報と、Exchange から送受信されるインスタンス XML に関する情報を提供する XML 参照ドキュメントが含まれています。 
    
- [Ews マネージ api リファレンス](ews-managed-api-reference-for-exchange.md): EWS マネージ API の api リファレンスドキュメントが含まれています。 EWS マネージ API は、EWS を使用するアプリケーションを開発および拡張するための、シンプルで完全な機能を備えたインターフェイスです。 
    
- [Exchange 用の自動検出 web サービスリファレンス](autodiscover-web-service-reference-for-exchange.md): exchange によって提供される自動検出サービスの XML API リファレンスが含まれています。 自動検出 Api は、Exchange サービスエンドポイントを自動的に検出できるようにするためのプロビジョニング情報をクライアントアプリケーションに提供します。 
    
- [ユニファイドメッセージング web サービスリファレンス Exchange](unified-messaging-web-service-reference-for-exchange.md) : ユニファイドメッセージング (UM) web サービスの XML API リファレンスが含まれています。 UM web サービスは、クライアントアプリケーションに Exchange の UM 機能へのアクセスを提供します。 EWS では UM 機能も提供されることに注意してください。 
    
- [Exchange 用の EWS によって生成されたオブジェクトモデル](ews-generated-object-models-reference-for-exchange.md)— exchangewebservices 名前空間に自動生成されたプロキシクラスの API リファレンスが含まれています。 
    
    > [!NOTE]
    > .NET Framework 3.5 以降の .NET Framework のバージョンに基づくクライアントでは、ews マネージ API を使用して EWS にアクセスすることをお勧めします。 詳細については、「 [EWS マネージ API クライアントアプリケーションの概要](../exchange-web-services/get-started-with-ews-managed-api-client-applications.md)」を参照してください。 
  
使用する Api のセットの詳細については、「 [EWS クライアント設計の概要 (Exchange](../exchange-web-services/ews-client-design-overview-for-exchange.md))」を参照してください。
  
Exchange XML 参照は、クライアントとサーバーの間で送信される XML インスタンスに基づいています。 XML は、EWS および SOAP 自動検出サービス用の WSDL ファイルと XSD ファイルで記述されています。 UM web サービスと POX 自動検出サービスには、その構造を記述する公開された WSDL およびスキーマファイルがありません。 スキーマファイルが含まれていないサービスの XML リファレンスは、クライアントとサービスの間で交換されたときに、監視およびキャプチャできる XML インスタンスに基づいています。
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Exchange で Web サービスの使用を開始する](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)
    

