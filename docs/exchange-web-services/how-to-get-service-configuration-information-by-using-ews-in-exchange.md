---
title: Exchange EWS を使用してサービスの構成情報を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758951"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a><span data-ttu-id="78c90-103">Exchange EWS を使用してサービスの構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="78c90-103">Get service configuration information by using EWS in Exchange</span></span>

<span data-ttu-id="78c90-104">Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="78c90-104">Find out how to get service configuration information for UM, policy nudges, mail tips, and protection rules from EWS in Exchange.</span></span>
  
<span data-ttu-id="78c90-105">EWS アプリケーションは、ユニファイド メッセージング (UM)、ポリシー微調整を行うとき、メールのヒント、または保護のルールで動作しますか。</span><span class="sxs-lookup"><span data-stu-id="78c90-105">Does your EWS application work with Unified Messaging (UM), policy nudges, mail tips, or protection rules?</span></span> <span data-ttu-id="78c90-106">場合は、アプリケーションが必要なサービスの構成情報を取得するのには[GetServiceConfiguration の操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="78c90-106">If so, your application will need to call the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to get the service configuration information that it needs.</span></span> <span data-ttu-id="78c90-107">**GetServiceConfiguration**操作では、EWS のこれらの機能のそれぞれに固有の構成情報を返します。</span><span class="sxs-lookup"><span data-stu-id="78c90-107">The **GetServiceConfiguration** operation returns configuration information that is specific to each of these EWS features.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="78c90-108">EWS マネージ API はこの機能を実装していません。</span><span class="sxs-lookup"><span data-stu-id="78c90-108">The EWS Managed API does not implement this functionality.</span></span> 
  
<span data-ttu-id="78c90-109">**表 1 です。GetServiceConfiguration 操作によって返される構成情報**</span><span class="sxs-lookup"><span data-stu-id="78c90-109">**Table 1. Configuration information that the GetServiceConfiguration operation returns**</span></span>

|<span data-ttu-id="78c90-110">EWS の機能</span><span class="sxs-lookup"><span data-stu-id="78c90-110">EWS feature</span></span>|<span data-ttu-id="78c90-111">GetServiceConfiguration 操作によって返されるもの</span><span class="sxs-lookup"><span data-stu-id="78c90-111">GetServiceConfiguration operation returns…</span></span>|
|:-----|:-----|
|<span data-ttu-id="78c90-112">UM</span><span class="sxs-lookup"><span data-stu-id="78c90-112">UM</span></span>  <br/> | <ul><li><span data-ttu-id="78c90-113">UM が有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78c90-113">A value that indicates whether UM is enabled.</span></span></li><li><span data-ttu-id="78c90-114">電話での再生が有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78c90-114">A value that indicates whether play on phone is enabled.</span></span></li><li><span data-ttu-id="78c90-115">電話での再生のダイヤル文字列。</span><span class="sxs-lookup"><span data-stu-id="78c90-115">The play on phone dial string.</span></span></li></ul> |
|<span data-ttu-id="78c90-116">ポリシー微調整</span><span class="sxs-lookup"><span data-stu-id="78c90-116">Policy nudges</span></span>  <br/> | <ul><li><span data-ttu-id="78c90-117">クライアントでの表示用のポリシー微調整。</span><span class="sxs-lookup"><span data-stu-id="78c90-117">Policy nudges for display in your client.</span></span></li></ul> |
|<span data-ttu-id="78c90-118">メールのヒント</span><span class="sxs-lookup"><span data-stu-id="78c90-118">Mail tips</span></span>  <br/> | <ul><li><span data-ttu-id="78c90-119">メールのヒントが有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78c90-119">A value that indicates whether mail tips are enabled.</span></span></li><li><span data-ttu-id="78c90-120">要求あたりの最大受信者数。</span><span class="sxs-lookup"><span data-stu-id="78c90-120">The maximum number of recipients per request.</span></span></li><li><span data-ttu-id="78c90-121">最大メッセージ サイズ。</span><span class="sxs-lookup"><span data-stu-id="78c90-121">The maximum message size.</span></span></li><li><span data-ttu-id="78c90-122">多数の対象ユーザーのしきい値。</span><span class="sxs-lookup"><span data-stu-id="78c90-122">The large audience threshold.</span></span></li><li><span data-ttu-id="78c90-123">外部の受信者数を表示するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78c90-123">A value that indicates whether the number of external recipients is shown.</span></span></li><li><span data-ttu-id="78c90-124">内部ドメインの一覧。</span><span class="sxs-lookup"><span data-stu-id="78c90-124">A list of internal domains.</span></span></li><li><span data-ttu-id="78c90-125">ポリシーのヒントが有効かどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="78c90-125">A value that indicates whether policy tips are enabled.</span></span></li><li><span data-ttu-id="78c90-126">メールの受信者数が多数であると見なされるかどうかの、対象ユーザー数の最大しきい値。</span><span class="sxs-lookup"><span data-stu-id="78c90-126">The large audience cap threshold for indicating whether your mail is considered to have a large number of recipients.</span></span>  </li></ul>|
|<span data-ttu-id="78c90-127">保護ルール</span><span class="sxs-lookup"><span data-stu-id="78c90-127">Protection rules</span></span>  <br/> | <ul><li><span data-ttu-id="78c90-128">クライアントにセットアップされた保護ルール。</span><span class="sxs-lookup"><span data-stu-id="78c90-128">Protection rules setup for your client.</span></span></li><li><span data-ttu-id="78c90-129">組織内部のドメインの一覧。</span><span class="sxs-lookup"><span data-stu-id="78c90-129">A list of domains that are internal to your organization.</span></span>  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a><span data-ttu-id="78c90-130">コード例:EWS を使用して、メールのヒントのサービス構成情報を取得する</span><span class="sxs-lookup"><span data-stu-id="78c90-130">Code example: Get service configuration information for mail tips by using EWS</span></span>

<span data-ttu-id="78c90-131">次のコード例では、メールのヒントについてはサービスの構成情報を要求する[GetServiceConfiguration の操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="78c90-131">The following code example uses the [GetServiceConfiguration operation](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) to request service configuration information for mail tips.</span></span> <span data-ttu-id="78c90-132">[ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx)要素に異なる値を追加することによって、その他のサービスの構成情報を要求できます。</span><span class="sxs-lookup"><span data-stu-id="78c90-132">You can request additional service configuration information by adding more [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) elements with different values.</span></span> 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
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

## <a name="next-steps"></a><span data-ttu-id="78c90-133">次の手順</span><span class="sxs-lookup"><span data-stu-id="78c90-133">Next steps</span></span>

<span data-ttu-id="78c90-134">サービスの構成情報を要求すると後、は、それを解析できるように、XML 応答をロードするのには、 [XmlDocument クラス](http://msdn.microsoft.com/ja-jp/library/system.xml.xmldocument.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="78c90-134">After you request service configuration information, use the [XmlDocument class](http://msdn.microsoft.com/ja-jp/library/system.xml.xmldocument.aspx) to load the response XML so that you can parse it.</span></span> <span data-ttu-id="78c90-135">そして、シナリオによっては、次のいずれかの操作を行います。</span><span class="sxs-lookup"><span data-stu-id="78c90-135">Then, depending on your scenario, you can do one of the following:</span></span> 
  
- <span data-ttu-id="78c90-136">[GetMailTips 操作](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx)を使用すると、クライアント アプリケーションがユーザーに表示するのにためのメール ヒントを取得できます。</span><span class="sxs-lookup"><span data-stu-id="78c90-136">Use the [GetMailTips operation](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) to get mail tips for client applications to display to users.</span></span> 
    
- <span data-ttu-id="78c90-137">UM が有効な場合、携帯電話経由で[メールボックスのアイテムを再生する方法について説明](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx)をします。</span><span class="sxs-lookup"><span data-stu-id="78c90-137">If UM is enabled, [learn about how to play mailbox items](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) over your phone.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="78c90-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="78c90-138">See also</span></span>

- [<span data-ttu-id="78c90-139">Exchange 内の構成オプション</span><span class="sxs-lookup"><span data-stu-id="78c90-139">Configuration options for EWS in Exchange</span></span>](configuration-options-for-ews-in-exchange.md)    
- [<span data-ttu-id="78c90-140">EWS アプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="78c90-140">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="78c90-141">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="78c90-141">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

