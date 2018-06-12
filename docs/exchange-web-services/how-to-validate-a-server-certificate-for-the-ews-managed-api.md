---
title: EWS のマネージ API のサーバー証明書を検証します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Exchange Server に EWS Managed API 要求を行うことができるように、証明書検証のコールバック メソッドを作成して参照する方法について説明します。
ms.openlocfilehash: 13d7c51e55308b9e9997697a075c8a9e6b4f10d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759067"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a>EWS のマネージ API のサーバー証明書を検証します。

Exchange Server に EWS Managed API 要求を行うことができるように、証明書検証のコールバック メソッドを作成して参照する方法について説明します。
  
既定では、Exchange が Exchange 2007 SP1 以降のバージョンを使用して、自己署名付き X509 EWS からの呼び出しを認証する証明書です。 EWS のマネージ API を使用している、証明書検証のコールバック メソッドを作成する必要があります。それ以外の場合、EWS のマネージ API の要求は失敗します。 自動検出サービスを使用する場合、EWS のマネージ API 自動検出メソッドへの呼び出しが**AutodiscoverLocalException**エラーで失敗します。 Web で生成された web サービス プロキシを使用する場合もあります、プロキシを作成する方法によって、検証コールバック メソッドを作成します。 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a>検証のコールバック メソッドを作成するための前提条件
<a name="bk_prereq"> </a>

サーバー証明書を検証するための設定を行うには、以下の条件を満たしていることを確認します。  
  
- Exchange サーバーが EWS の自己署名証明書を使用しています。管理者がルート証明書につながる有効な証明書をインストールした場合は、検証のコールバック メソッドを作成する必要はありません。  
    
- 次の必要な.NET Framework の名前空間への参照を含むマネージ アプリケーションを作成しています。  
    
  - **System.Net**
  - **System.Net.Security**  
  - **System.Security.Cryptography.X509Certificates**
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a>例:EWS Managed API のサーバー証明書を検証するコールバック メソッド
<a name="bk_example"> </a>

次のコード例は、EWS Managed API の X509 証明書の検証のコールバック メソッドを作成する方法を示します。このメソッドは、X509 証明書を検証し、次の条件のいずれかを満たす場合にのみ true を返します。  
  
- 証明書が有効で、有効なルート証明書に戻ります。    
- 証明書が有効で、それを返したサーバーによって自己署名されます。  
    
> [!IMPORTANT]
> この例の証明書検証のコールバック メソッドでは、EWS Managed API アプリケーションの開発およびテストのための十分なセキュリティを提供します。ただし、ユーザーが展開したアプリケーションのための十分なセキュリティを提供しない可能性があります。使用する証明書検証のコールバック メソッドが組織のセキュリティ要件を満たしていることを必ず確認してください。 
  
```cs
      private static bool CertificateValidationCallBack(
         object sender,
         System.Security.Cryptography.X509Certificates.X509Certificate certificate,
         System.Security.Cryptography.X509Certificates.X509Chain chain,
         System.Net.Security.SslPolicyErrors sslPolicyErrors)
    {
      // If the certificate is a valid, signed certificate, return true.
      if (sslPolicyErrors == System.Net.Security.SslPolicyErrors.None)
      {
        return true;
      }
      // If there are errors in the certificate chain, look at each error to determine the cause.
      if ((sslPolicyErrors &amp; System.Net.Security.SslPolicyErrors.RemoteCertificateChainErrors) != 0)
      {
        if (chain != null &amp;&amp; chain.ChainStatus != null)
        {
          foreach (System.Security.Cryptography.X509Certificates.X509ChainStatus status in chain.ChainStatus)
          {
            if ((certificate.Subject == certificate.Issuer) &amp;&amp;
               (status.Status == System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.UntrustedRoot))
            {
              // Self-signed certificates with an untrusted root are valid. 
              continue;
            }
            else
            {
              if (status.Status != System.Security.Cryptography.X509Certificates.X509ChainStatusFlags.NoError)
              {
                // If there are any other errors in the certificate chain, the certificate is invalid,
             // so the method returns false.
                return false;
              }
            }
          }
        }
        // When processing reaches this line, the only errors in the certificate chain are 
    // untrusted root errors for self-signed certificates. These certificates are valid
    // for default Exchange server installations, so return true.
        return true;
      }
      else
      {
     // In all other cases, return false.
        return false;
      }
    }

```

.NET **System.Net**名前空間の**ServicePointManager**クラスを使用すると、 **ServerCertificateValidationCallback**プロパティを設定することにより、検証のコールバック メソッドをフックします。 **ServerCertificateValidationCallback**プロパティを設定するのにコード例を次のようなコードを使用できます。 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a>次の手順
<a name="bk_example"> </a>

EWS Managed API の検証のコールバック メソッドを作成した後で、自動検出サービスを使用して、接続ポイント、およびユーザーとドメインの設定を Exchange Server から取得できます。詳細については、以下の記事を参照してください。
  
- [自動検出を使用してコネクション ポイントを検索するには](how-to-use-autodiscover-to-find-connection-points.md)
    
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Exchange サーバーからドメインの設定を取得します。](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a>関連項目

- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)  
- [Exchange で Web サービスの使用を開始する](start-using-web-services-in-exchange.md)
    

