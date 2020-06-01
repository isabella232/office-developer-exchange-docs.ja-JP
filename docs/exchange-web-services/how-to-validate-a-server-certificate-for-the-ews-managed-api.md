---
title: EWS マネージ API のサーバー証明書を検証する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1fe0b215-8340-4bc8-a6ce-4f591ca9e353
description: Exchange Server に EWS Managed API 要求を行うことができるように、証明書検証のコールバック メソッドを作成して参照する方法について説明します。
localization_priority: Priority
ms.openlocfilehash: 195c51ca71890d6092e4182d23990bb528d37095
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456781"
---
# <a name="validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="f24fa-103">EWS マネージ API のサーバー証明書を検証する</span><span class="sxs-lookup"><span data-stu-id="f24fa-103">Validate a server certificate for the EWS Managed API</span></span>

<span data-ttu-id="f24fa-104">Exchange Server に EWS Managed API 要求を行うことができるように、証明書検証のコールバック メソッドを作成して参照する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f24fa-104">Learn how to create and reference a certificate validation callback method so that you can make EWS Managed API requests to an Exchange server.</span></span>
  
<span data-ttu-id="f24fa-105">既定では、Exchange 2007 SP1 以降のバージョンの Exchange は、自己署名付き X509 証明書を使用して、EWS からの呼び出しを認証します。</span><span class="sxs-lookup"><span data-stu-id="f24fa-105">By default, versions of Exchange starting with Exchange 2007 SP1 use self-signed X509 certificates to authenticate calls from EWS.</span></span> <span data-ttu-id="f24fa-106">EWS マネージ API を使用している場合は、証明書検証のコールバック メソッドを作成する必要があります。作成しないと、EWS Managed API 要求は失敗します。</span><span class="sxs-lookup"><span data-stu-id="f24fa-106">When you are using the EWS Managed API, you need to create a certificate validation callback method; otherwise, EWS Managed API requests will fail.</span></span> <span data-ttu-id="f24fa-107">自動検出サービスを使用している場合、EWS マネージ API の自動検出メソッドを呼び出すと、**AutodiscoverLocalException** エラーで失敗します。</span><span class="sxs-lookup"><span data-stu-id="f24fa-107">If you are using the Autodiscover service, the call to the EWS Managed API Autodiscover method will fail with an **AutodiscoverLocalException** error.</span></span> <span data-ttu-id="f24fa-108">Web で生成された Web サービス プロキシを使用している場合は、プロキシの作成方法に応じて、検証のコールバック メソッドも作成しなければならない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f24fa-108">If you are using a web-generated web service proxy, you might also have to create a validation callback method, depending on how the proxy is created.</span></span> 
  
## <a name="prerequisites-for-creating-a-validation-callback-method"></a><span data-ttu-id="f24fa-109">検証のコールバック メソッドを作成するための前提条件</span><span class="sxs-lookup"><span data-stu-id="f24fa-109">Prerequisites for creating a validation callback method</span></span>
<span data-ttu-id="f24fa-110"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="f24fa-110"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="f24fa-111">サーバー証明書を検証するための設定を行うには、以下の条件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f24fa-111">To set up to validate a server certificate, ensure that the following are true:</span></span> 
  
- <span data-ttu-id="f24fa-p102">Exchange サーバーが EWS の自己署名証明書を使用しています。管理者がルート証明書につながる有効な証明書をインストールした場合は、検証のコールバック メソッドを作成する必要はありません。 </span><span class="sxs-lookup"><span data-stu-id="f24fa-p102">Your Exchange server is using a self-signed certificate for EWS. If the administrator has installed a valid certificate that traces to a root certificate, you do not need to create a validation callback method.</span></span> 
    
- <span data-ttu-id="f24fa-114">次の必要な.NET Framework の名前空間への参照を含むマネージ アプリケーションを作成しています。</span><span class="sxs-lookup"><span data-stu-id="f24fa-114">You are creating a managed application that includes a reference to the following required .NET Framework namespaces:</span></span> 
    
  - <span data-ttu-id="f24fa-115">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="f24fa-115">**System.Net**</span></span>
  - <span data-ttu-id="f24fa-116">**System.Net.Security**</span><span class="sxs-lookup"><span data-stu-id="f24fa-116">**System.Net.Security**</span></span>  
  - <span data-ttu-id="f24fa-117">**System.Security.Cryptography.X509Certificates**</span><span class="sxs-lookup"><span data-stu-id="f24fa-117">**System.Security.Cryptography.X509Certificates**</span></span>
    
## <a name="example-callback-method-to-validate-a-server-certificate-for-the-ews-managed-api"></a><span data-ttu-id="f24fa-118">例: EWS マネージ API のサーバー証明書を検証するコールバック メソッド</span><span class="sxs-lookup"><span data-stu-id="f24fa-118">Example: Callback method to validate a server certificate for the EWS Managed API</span></span>
<span data-ttu-id="f24fa-119"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="f24fa-119"><a name="bk_example"> </a></span></span>

<span data-ttu-id="f24fa-p103">次のコード例は、EWS Managed API の X509 証明書の検証のコールバック メソッドを作成する方法を示します。このメソッドは、X509 証明書を検証し、次の条件のいずれかを満たす場合にのみ true を返します。 </span><span class="sxs-lookup"><span data-stu-id="f24fa-p103">The following code example shows how to create an X509 certificate validation callback method for the EWS Managed API. This method will validate an X509 certificate and only return true when either of the following criteria are met:</span></span> 
  
- <span data-ttu-id="f24fa-122">証明書が有効で、有効なルート証明書に戻ります。</span><span class="sxs-lookup"><span data-stu-id="f24fa-122">The certificate is valid and traces back to a valid root certificate.</span></span>    
- <span data-ttu-id="f24fa-123">証明書が有効で、それを返したサーバーによって自己署名されます。</span><span class="sxs-lookup"><span data-stu-id="f24fa-123">The certificate is valid and is self-signed by the server that returned it.</span></span> 
    
> [!IMPORTANT]
> <span data-ttu-id="f24fa-p104">この例の証明書検証のコールバック メソッドでは、EWS Managed API アプリケーションの開発およびテストのための十分なセキュリティを提供します。ただし、ユーザーが展開したアプリケーションのための十分なセキュリティを提供しない可能性があります。使用する証明書検証のコールバック メソッドが組織のセキュリティ要件を満たしていることを必ず確認してください。</span><span class="sxs-lookup"><span data-stu-id="f24fa-p104">The certificate validation callback method in this example provides sufficient security for development and testing of EWS Managed API applications. However, it might not provide sufficient security for your deployed application. You should always make sure that the certificate validation callback method that you use meets the security requirements of your organization.</span></span> 
  
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

<span data-ttu-id="f24fa-127">.NET の **System.Net** 名前空間で **ServicePointManager** クラスを使用し、**ServerCertificateValidationCallback** プロパティを設定することで、検証のコールバック メソッドをフックします。</span><span class="sxs-lookup"><span data-stu-id="f24fa-127">You use the **ServicePointManager** class in the .NET **System.Net** namespace to hook up a validation callback method by setting the **ServerCertificateValidationCallback** property.</span></span> <span data-ttu-id="f24fa-128">次の例に似たコードを使用して、**ServerCertificateValidationCallback** プロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="f24fa-128">You can use code similar to the following code example to set the **ServerCertificateValidationCallback** property.</span></span> 
  
```cs
ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;

```

## <a name="next-steps"></a><span data-ttu-id="f24fa-129">次の手順</span><span class="sxs-lookup"><span data-stu-id="f24fa-129">Next steps</span></span>
<span data-ttu-id="f24fa-130"><a name="bk_example"> </a></span><span class="sxs-lookup"><span data-stu-id="f24fa-130"><a name="bk_example"> </a></span></span>

<span data-ttu-id="f24fa-p106">EWS Managed API の検証のコールバック メソッドを作成した後で、自動検出サービスを使用して、接続ポイント、およびユーザーとドメインの設定を Exchange Server から取得できます。詳細については、以下の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f24fa-p106">After you have created the validation callback method for the EWS Managed API, you can use the Autodiscover service to get connection points and user and domain settings from an Exchange server. For more information, see the following articles:</span></span>
  
- [<span data-ttu-id="f24fa-133">自動検出を使用して接続ポイントを検索する</span><span class="sxs-lookup"><span data-stu-id="f24fa-133">Use Autodiscover to find connection points</span></span>](how-to-use-autodiscover-to-find-connection-points.md)
    
- [<span data-ttu-id="f24fa-134">自動検出を使用して Exchange からユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="f24fa-134">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="f24fa-135">Exchange サーバーからドメイン設定を取得する</span><span class="sxs-lookup"><span data-stu-id="f24fa-135">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
## <a name="see-also"></a><span data-ttu-id="f24fa-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f24fa-136">See also</span></span>

- [<span data-ttu-id="f24fa-137">EWS アプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="f24fa-137">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)  
- [<span data-ttu-id="f24fa-138">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="f24fa-138">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    

