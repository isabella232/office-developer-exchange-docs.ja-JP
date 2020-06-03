---
title: Exchange で EWS を使用して、サービス構成情報を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
ms.openlocfilehash: 7546d9524f1e004eda2bdc55687fb44beafa44af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528007"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="cbe07-103">Exchange で EWS を使用して、サービス構成情報を取得する</span><span class="sxs-lookup"><span data-stu-id="cbe07-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="cbe07-104">Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="cbe07-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="cbe07-105">EWS アプリケーションが、ユニファイド メッセージング (UM)、ポリシー微調整、メールのヒント、保護ルールと連携している場合、</span><span class="sxs-lookup"><span data-stu-id="cbe07-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="cbe07-106">アプリケーションは [GetServiceConfiguration 操作](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を呼び出して、必要なサービス構成情報を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbe07-106">If so, your application will need to call the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="cbe07-107">**GetServiceConfiguration** 操作では、EWS のこれらの機能のそれぞれに固有の構成情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="cbe07-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cbe07-108">EWS マネージ API はこの機能を実装していません。</span><span class="sxs-lookup"><span data-stu-id="cbe07-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="cbe07-109">**表 1. GetServiceConfiguration 操作によって返される構成情報**</span><span class="sxs-lookup"><span data-stu-id="cbe07-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="cbe07-110">EWS の機能</span><span class="sxs-lookup"><span data-stu-id="cbe07-110">EWS feature</span></span>|<span data-ttu-id="cbe07-111">GetServiceConfiguration 操作によって返されるもの</span><span class="sxs-lookup"><span data-stu-id="cbe07-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="cbe07-112">UM</span><span class="sxs-lookup"><span data-stu-id="cbe07-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="cbe07-113">UM が有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="cbe07-114">電話での再生が有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="cbe07-115">電話での再生のダイヤル文字列。</span><span class="sxs-lookup"><span data-stu-id="cbe07-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="cbe07-116">ポリシー微調整</span><span class="sxs-lookup"><span data-stu-id="cbe07-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="cbe07-117">クライアントでの表示用のポリシー微調整。</span><span class="sxs-lookup"><span data-stu-id="cbe07-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="cbe07-118">メールのヒント</span><span class="sxs-lookup"><span data-stu-id="cbe07-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="cbe07-119">メールのヒントが有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="cbe07-120">要求あたりの最大受信者数。</span><span class="sxs-lookup"><span data-stu-id="cbe07-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="cbe07-121">最大メッセージ サイズ。</span><span class="sxs-lookup"><span data-stu-id="cbe07-121">The maximum message size.</span></span></li><li><span data-ttu-id="cbe07-122">多数の対象ユーザーのしきい値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-122">The large audience threshold.</span></span></li><li><span data-ttu-id="cbe07-123">外部の受信者数を表示するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="cbe07-124">内部ドメインの一覧。</span><span class="sxs-lookup"><span data-stu-id="cbe07-124">A list of internal domains.</span></span></li><li><span data-ttu-id="cbe07-125">ポリシーのヒントが有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="cbe07-126">メールの受信者数が多数であると見なされるかどうかの、対象ユーザー数の最大しきい値。</span><span class="sxs-lookup"><span data-stu-id="cbe07-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="cbe07-127">保護ルール</span><span class="sxs-lookup"><span data-stu-id="cbe07-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="cbe07-128">クライアントにセットアップされた保護ルール。</span><span class="sxs-lookup"><span data-stu-id="cbe07-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="cbe07-129">組織内部のドメインの一覧。</span><span class="sxs-lookup"><span data-stu-id="cbe07-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="cbe07-130">コード例: EWS を使用して、メールのヒントのサービス構成情報を取得する</span><span class="sxs-lookup"><span data-stu-id="cbe07-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="cbe07-131">次のコード例では、[GetServiceConfiguration 操作](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を使用して、メールのヒントのサービス構成情報を要求します。</span><span class="sxs-lookup"><span data-stu-id="cbe07-131">The following code example uses the [GetServiceConfiguration operation](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="cbe07-132">別の値の [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) 要素をさらに追加して、追加のサービス構成情報を要求することができます。</span><span class="sxs-lookup"><span data-stu-id="cbe07-132">You can request additional service configuration information by adding more [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a><span data-ttu-id="cbe07-133">次の手順</span><span class="sxs-lookup"><span data-stu-id="cbe07-133">Next steps</span></span>

<span data-ttu-id="cbe07-134">サービス構成情報の要求後、[XmlDocument クラス](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx)を使用して応答 XML を読み込み、それを解析できるようにします。</span><span class="sxs-lookup"><span data-stu-id="cbe07-134">After you request service configuration information, use the [XmlDocument class](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="cbe07-135">またシナリオに応じて、次のいずれかの操作を行います。</span><span class="sxs-lookup"><span data-stu-id="cbe07-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="cbe07-136">[GetMailTips 操作](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx)を使用して、クライアント アプリケーションがユーザーに表示するためのメールのヒントを取得する。</span><span class="sxs-lookup"><span data-stu-id="cbe07-136">Use the [GetMailTips operation](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="cbe07-137">電話を介して[メールボックス アイテムを再生する方法を理解する](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) (UM が有効な場合)。</span><span class="sxs-lookup"><span data-stu-id="cbe07-137">If UM is enabled, [learn about how to play mailbox items](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="cbe07-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbe07-138">See also</span></span>

- [<span data-ttu-id="cbe07-139">Exchange 内の EWS の構成オプション</span><span class="sxs-lookup"><span data-stu-id="cbe07-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="cbe07-140">EWS アプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="cbe07-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="cbe07-141">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="cbe07-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

