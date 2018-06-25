---
title: EWS のマネージ API を使用して、EWS のサービスの URL を設定します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
ms.openlocfilehash: e1a414f7c6f13bd61a58403c9d2be546c0226a69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759051"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>EWS のマネージ API を使用して、EWS のサービスの URL を設定します。

EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
  
サービスの URL は、Exchange は、Exchange Web サービス (EWS) との通信に使用するアドレスです。 EWS のマネージ API アプリケーションはこのアドレスを持ち、 [EWS を使って通信](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)するために適切なアクセス権を持つ後、 [ExchangeService クラス](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)への呼び出しが行えます。 オンプレミスの Exchange サーバーのサービスの URL は、次のようになります。 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

いくつかの方法では、アプリケーションでは、EWS の URL を設定できます。 [自動検出サービス](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)を使用して、URL を取得する別のサーバーにメールボックスを移行する場合、大規模なフォレスト内のサーバー、URL を変更することをお勧めします。 ただし、自動検出を呼び出す時間がかかることができ、キャッシュすることができます、時間の短い期間に複数の呼び出しを実行する必要がある場合、アプリケーションの速度が低下するため URL の値自動検出からを取得し、キャッシュされたこの va の EWS のサービスの URL を手動で設定lue。 これにより、アプリケーションのパフォーマンスが向上します。だけで自動検出を使用して、サーバーの値が変更された場合でも定期的にキャッシュされた値を更新することを確認します。 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>自動検出サービスを使用して EWS サービス URL を設定する
<a name="bk_SetURLusingAutoDiscover"> </a>

[AutodiscoverUrl](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx)メソッドでは、 [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)エンドポイントを設定するのには電子メール アドレスを使用し、 **ExchangeService**プロキシ クラスに含まれるすべてのメソッドを使用するアプリケーションを有効にします。 次の例では、 **AutodiscoverURL**メソッドを使用する方法を示します。 
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.AutodiscoverUrl("User1@contoso.com");

```

## <a name="set-the-exchange-service-url-manually"></a>Exchange サービス URL を手動で設定する
<a name="bk_SetURLmanually"> </a>

次の例は、キャッシュされた値を使用して EWS サービス URL を設定する方法を示しています。これを行う前に、自動検出サービスを使用して EWS URL を必ず取得するようにしてください。
  
```cs
// Create the binding.
ExchangeService service = new ExchangeService();
// Set the credentials for the on-premises server.
service.Credentials = new WebCredentials("user1@contoso.com", "password");
// Set the URL.
service.Url = new Uri("https://computername.domain.contoso.com/EWS/Exchange.asmx");

```

## <a name="see-also"></a>関連項目

- [EWS マネージ API クライアント アプリケーションの概要](get-started-with-ews-managed-api-client-applications.md)   
- [Exchange アプリケーションの開発環境を設定します。](setting-up-your-exchange-application-development-environment.md)   
- [Exchange EWS へのアクセスを制御します。](how-to-control-access-to-ews-in-exchange.md) 
- [EWS のマネージ API を使用して通信 EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [自動検出を使用してコネクション ポイントを検索するには](how-to-use-autodiscover-to-find-connection-points.md)
    

