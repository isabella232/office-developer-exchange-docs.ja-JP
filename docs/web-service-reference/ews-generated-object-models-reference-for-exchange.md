---
title: Exchange 用に Exchange Web サービス (EWS) で生成されたオブジェクト モデル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 67d7d831-9c53-46da-80e4-18f562e71284
description: Exchange 用のアプリケーションを開発するのに EWS によって生成されるオブジェクト モデル参照を使用している場合に EWS 開発で使用できる他のオプションについて説明します。
ms.openlocfilehash: 6c97ca7973da84d96d102287b9c260409a0f57ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541435"
---
# <a name="ews-generated-object-models-for-exchange"></a>Exchange 用に EWS で生成されたオブジェクト モデル

**適用対象**: Exchange Online |Exchange Server 2013 |Office 365

wsdl.exe によって生成された Exchange Web サービス (EWS) オブジェクト モデルは、当初 Exchange 2007 を操作するのに便利なオブジェクト モデルを提供しました。 しかし、EWS マネージ API が利用できるようになると、マネージ コードを使用して作業している開発者用に多くのメリットが紹介されました。 

EWS マネージ API は、

- 直感的なオブジェクト モデルを用意します。

- クライアント側のビジネス ロジックとデータの入力規則を含みます。

- 完全にサポートされており、定期的に更新されます。

- 自動検出クライアントを含みます。

- ログ、Cookie の管理、Exchange への診断レポートの送信などのクライアント機能を実装します。

EWS wsdl.exe ベースのマネージ リファレンス ドキュメントは、生成されたオブジェクト モデルによって提供されたほとんどの機能が EWS マネージ API によって置き換えられるため廃止されました。同時に、EWS マネージ API がすべてのユーザーに適しているわけではないことも事実です。ほとんどの場合、.NET の EWS クライアントを作成するのが最善の方法ですが、次のような例外もあります。

- 使用する機能が [EWS マネージ API に実装されていない](../exchange-web-services/web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md#bk_apifeatures)場合。

- .NET 以外の開発プラットフォームを使用している場合。

EWS マネージ API を使用してアプリケーションを開発できない場合は、次の操作を実行できます。

- サード パーティ EWS クライアント API を使用する。

- 独自の EWS クライアント オブジェクト モデルを作成する。

- オブジェクト モデルのジェネレーターを使用する。ほとんどの主要なプラットフォームや言語をサポートするオブジェクト モデルのジェネレーターを見つけることができます。

オブジェクト モデルのジェネレーターを使用する場合、XML 参照を使用して、生成されたオブジェクト モデルの理解を深めることができます。オブジェクト モデルは、スキーマで説明されている XML 構造から生成されます。通常、オブジェクト モデルのジェネレーターによって作成されたクラスは、スキーマの複合型にマップします。プロパティは、通常、XML 要素にマップします。  

[ExchangeWebServices 名前空間](https://docs.microsoft.com/dotnet/api/exchangewebservices?view=exchange-ews-proxy)を表示します。

## <a name="see-also"></a>関連項目

- [Exchange の Web サービス リファレンス](web-services-reference-for-exchange.md)
- [Exchange の EWS マネージド API、EWS、Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [EWS およびその他の Exchange の Web サービスの新機能](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
