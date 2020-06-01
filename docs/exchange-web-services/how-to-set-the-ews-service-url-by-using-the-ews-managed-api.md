---
title: EWS マネージ API を使用して EWS サービス URL を設定する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: cddf6525-1c04-484b-a911-56c2f0f1f7b6
description: EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 5ba79b48d4eb4fec62110448c5924de16b67ce10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456739"
---
# <a name="set-the-ews-service-url-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して EWS サービス URL を設定する

EWS マネージ API アプリケーションでの EWS サービス URL の設定方法について説明します。
  
サービス URL は、Exchange が Exchange Web サービス (EWS) との通信に使用するアドレスです。 このアドレスを認識していて、[EWS と通信する](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)ための適切なアクセス権のある EWS マネージ API アプリケーションは、[ExchangeService クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)の呼び出しを行えます。 オンプレミス Exchange サーバーのサービス URL は、たとえば次のようになります。 
  
```HTML
https://computer.domain.contoso.com/EWS/Exchange.asmx
```

アプリケーションで EWS URL を設定するには、2 とおりの方法があります。[自動検出サービス](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)を使用して URL を取得することをお勧めします。大規模なサーバー フォレストでは、メールボックスが別のサーバーに移行されると、URL が変わることがあるからです。ただし、自動検出の呼び出しはある程度時間がかかることがあるため、短時間に複数の呼び出しを行う必要がある場合は、アプリケーションの速度が低下することがあります。したがって、自動検出から取得した URL 値をキャッシュし、キャッシュされたこの値を使用して EWS サービス URL を手動で設定した方がよい場合があります。この方法をとれば、アプリケーションのパフォーマンスが向上します。ただし、サーバーの値が変わった場合に備えて、キャッシュされた値を自動検出を使用して定期的に更新するようにしてください。 
  
## <a name="set-the-ews-service-url-by-using-the-autodiscover-service"></a>自動検出サービスを使用して EWS サービス URL を設定する
<a name="bk_SetURLusingAutoDiscover"> </a>

[AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) メソッドは、メール アドレスを使用して [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) エンドポイントを設定し、**ExchangeService** プロキシ クラスに含まれるどのメソッドもアプリケーションが使用できるようにします。 次の例に、**AutodiscoverURL** メソッドの使用方法を示します。 
  
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
- [Exchange アプリケーションの開発環境をセットアップする](setting-up-your-exchange-application-development-environment.md)   
- [Exchange で EWS へのアクセスを制御する](how-to-control-access-to-ews-in-exchange.md) 
- [EWS マネージ API を使用して EWS と通信する](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)  
- [自動検出を使用して接続ポイントを検索する](how-to-use-autodiscover-to-find-connection-points.md)
    

