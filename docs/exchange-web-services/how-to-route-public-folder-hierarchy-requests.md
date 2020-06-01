---
title: パブリック フォルダー階層の要求をルーティングする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: パブリック フォルダー階層についての知識を必要とするパブリック フォルダー情報に関するすべての要求 (パブリック フォルダーの移動や更新、削除、検索など) は、特定のユーザーの既定のパブリック フォルダー階層のメールボックスにルーティングする必要があります。 そのメールボックスに要求をルーティングするには、X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を自動検出サービスから返される特定の値に設定する必要があります。
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455702"
---
# <a name="route-public-folder-hierarchy-requests"></a><span data-ttu-id="2e52b-104">パブリック フォルダー階層の要求をルーティングする</span><span class="sxs-lookup"><span data-stu-id="2e52b-104">Route public folder hierarchy requests</span></span>

<span data-ttu-id="2e52b-105">パブリック フォルダー階層についての知識を必要とするパブリック フォルダー情報に関するすべての要求 (パブリック フォルダーの移動や更新、削除、検索など) は、特定のユーザーの既定のパブリック フォルダー階層のメールボックスにルーティングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-105">All requests for public folder information that require knowledge of the public folder hierarchy, such as moving, updating, deleting, or finding public folders, need to be routed to the default public folder hierarchy mailbox for the given user.</span></span> <span data-ttu-id="2e52b-106">そのメールボックスに要求をルーティングするには、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を自動検出サービスから返される特定の値に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values returned by the Autodiscover service.</span></span> 
  
<span data-ttu-id="2e52b-107">**パブリック フォルダーの概要**</span><span class="sxs-lookup"><span data-stu-id="2e52b-107">**Overview of public folders**</span></span>

|<span data-ttu-id="2e52b-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e52b-108">Header</span></span>|<span data-ttu-id="2e52b-109">必要なもの</span><span class="sxs-lookup"><span data-stu-id="2e52b-109">What do I need?</span></span>|<span data-ttu-id="2e52b-110">取得する方法</span><span class="sxs-lookup"><span data-stu-id="2e52b-110">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2e52b-111">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="2e52b-111">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="2e52b-112">自動検出の SOAP 応答 [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) から得られる [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 値。これが **X-AnchorMailbox** ヘッダーの値になります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-112">The [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) value from a [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) Autodiscover SOAP response, which becomes the value of the **X-AnchorMailbox** header.</span></span><br/><br/> <span data-ttu-id="2e52b-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span><span class="sxs-lookup"><span data-stu-id="2e52b-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span></span>| <span data-ttu-id="2e52b-114">1. ユーザーのメールボックスの SMTP アドレスで **GetUserSetting** 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-114">1. Send a **GetUserSetting** request with the SMTP address for the user's mailbox.</span></span><br/><br/><span data-ttu-id="2e52b-115">2. 自動検出サービスが返す **PublicFolderInformation** 要素の値をキャッシュします。</span><span class="sxs-lookup"><span data-stu-id="2e52b-115">2. Cache the value of the **PublicFolderInformation** element that the Autodiscover service returns.</span></span> <span data-ttu-id="2e52b-116">これは、コード内に既存の自動検出呼び出しからキャッシュすることも、新しい [EWS マネージ API の GetUserSettings 呼び出し](#bk_getpfinfoewsma)または [GetUserSettings SOAP 要求](#bk_getpfinfoews)からキャッシュすることもできます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-116">This can be a cached from an existing Autodiscover call in your code, or a new [EWS Managed API GetUserSettings call](#bk_getpfinfoewsma) or a [GetUserSettings SOAP request](#bk_getpfinfoews).</span></span>  <br/><br/><span data-ttu-id="2e52b-117">3. **PublicFolderInformation** 要素を使用して、**X AnchorMailbox** ヘッダーの値を入力します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-117">3. Use the **PublicFolderInformation** element to populate the value of the **X-AnchorMailbox** header.</span></span> <span data-ttu-id="2e52b-118">**PublicFolderInformation** 要素の値は、SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2e52b-118">The value of the **PublicFolderInformation** element is an SMTP address.</span></span>  <br/> |
|<span data-ttu-id="2e52b-119">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="2e52b-119">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="2e52b-120">[POX 自動検出の応答](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx)から得られる [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) 値。これが **X-PublicFolderMailbox** ヘッダーの値になります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-120">The [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) value from a [POX Autodiscover response](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx), which becomes the value of the **X-PublicFolderMailbox** header.</span></span><br/><br/> <span data-ttu-id="2e52b-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span><span class="sxs-lookup"><span data-stu-id="2e52b-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span></span>|<span data-ttu-id="2e52b-122">1. **X-AnchorMailbox** 電子メール アドレスを使用して、[POX 自動検出サービスを呼び出します](#bk_makeautodrequest)。</span><span class="sxs-lookup"><span data-stu-id="2e52b-122">1. [Call the POX Autodiscover](#bk_makeautodrequest) service using the **X-AnchorMailbox** email address.</span></span>  <br/><br/><span data-ttu-id="2e52b-123">2. 自動検出サービスから返された **Server** 要素を使用して、**X-PublicFolderMailbox** ヘッダーの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-123">2. Use the **Server** element returned by the Autodiscover service to populate the value of the **X-PublicFolderMailbox** header.</span></span> <span data-ttu-id="2e52b-124">**X-PublicFolderMailbox** の値は、ユーザー名が GUID になる SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2e52b-124">The value of the **X-PublicFolderMailbox** is an SMTP address where the username is a GUID.</span></span>  <br/> |

<br/>

<span data-ttu-id="2e52b-125">ヘッダーの値が決定したら、それらを[パブリック フォルダー階層の要求を行うときに](#bk_setheadervalues)含めます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-125">After you have determined the header values, include them [when you make public folder hierarchy requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="2e52b-p106">この記事の手順は、パブリック フォルダー階層の要求に固有のものです。要求がパブリック フォルダー階層とコンテンツのどちらの要求かを特定するには、「[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e52b-p106">The steps in this article are specific to public folder hierarchy requests. To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a><span data-ttu-id="2e52b-128">EWS マネージ API を使用して X-AnchorMailbox ヘッダーの値を決定する</span><span class="sxs-lookup"><span data-stu-id="2e52b-128">Determine the value of the X-AnchorMailbox header by using the EWS Managed API</span></span>
<span data-ttu-id="2e52b-129"><a name="bk_getpfinfoewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="2e52b-129"><a name="bk_getpfinfoewsma"> </a></span></span>

<span data-ttu-id="2e52b-130">EWS マネージ API を使用して [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) 値を取得するには、自動検出サービスへの既存の呼び出しで返される **PublicFolderInformation** 要素の値をキャッシュするか、新しい呼び出しを行います。</span><span class="sxs-lookup"><span data-stu-id="2e52b-130">To retrieve the [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) value by using the EWS Managed API, you can either cache the value of the **PublicFolderInformation** element that an existing call to the Autodiscover service returns, or make a new call.</span></span> 
  
<span data-ttu-id="2e52b-131">新しい呼び出しを行う場合は、コードに [EWS マネージ API を使用してユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[EWS マネージ API を使用してユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)してから、次のコードを使用して **GetUserSettings** サンプル メソッドを呼び出します。こうすれば、**PublicFolderInformation** 要素の値だけを取得します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-131">If you're making a new call, you can [Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) to your code, and then call the **GetUserSettings** sample method by using the following code, which retrieves only the value of the **PublicFolderInformation** element.</span></span> <span data-ttu-id="2e52b-132">入力パラメーターとして、メールボックス ユーザーの SMTP アドレスを含めます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-132">Include the SMTP address of the mailbox user as an input parameter.</span></span> 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

<span data-ttu-id="2e52b-133">コードを実行すると、次の情報がコンソールに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-133">After running the code, the following information is displayed on the console:</span></span>
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

<span data-ttu-id="2e52b-134">この時点で **PublicFolderInformation** 値は用意できています。この値は、X-AnchorMailbox ヘッダーの値としてパブリック フォルダー階層に対する要求のすべてに含めます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-134">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a><span data-ttu-id="2e52b-135">SOAP を使用して X-AnchorMailbox ヘッダーの値を決定する</span><span class="sxs-lookup"><span data-stu-id="2e52b-135">Determine the value of the X-AnchorMailbox header using SOAP</span></span>
<span data-ttu-id="2e52b-136"><a name="bk_getpfinfoews"> </a></span><span class="sxs-lookup"><span data-stu-id="2e52b-136"><a name="bk_getpfinfoews"> </a></span></span>

<span data-ttu-id="2e52b-137">次のコード例は、SOAP 操作の [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) を使用して、**PublicFolderInformation** 値を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-137">The following code example shows how to retrieve the **PublicFolderInformation** value by using the [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) SOAP operation.</span></span> <span data-ttu-id="2e52b-138">メールボックス ユーザーは [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) 要素で指定されます。また、[RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) 要素によって応答を [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 値に制限しています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-138">The mailbox user is specified in the [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) element, and the [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) element limits the response to the [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) value.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2e52b-139">応答には、**PublicFolderInformation** 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-139">The response includes the **PublicFolderInformation** value.</span></span> 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

<span data-ttu-id="2e52b-140">この時点で **PublicFolderInformation** 値は用意できています。この値は、X-AnchorMailbox ヘッダーの値としてパブリック フォルダー階層に対する要求のすべてに含めます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-140">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a><span data-ttu-id="2e52b-141">自動検出要求によって X-PublicFolderInformation 値を決定する</span><span class="sxs-lookup"><span data-stu-id="2e52b-141">Make an Autodiscover request to determine the X-PublicFolderInformation value</span></span>
<span data-ttu-id="2e52b-142"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="2e52b-142"><a name="bk_makeautodrequest"> </a></span></span>

<span data-ttu-id="2e52b-143">**PublicFolderInformation** SMTP アドレスを使用して自動検出要求を行います。これは、**X-AnchorMailbox** 値として使用されています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-143">Make an Autodiscover request by using the **PublicFolderInformation** SMTP address, which is now being used as the **X-AnchorMailbox** value.</span></span> <span data-ttu-id="2e52b-144">「[Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)」のコード サンプルを使用して、自動検出サービスを呼び出します。このコード サンプルを使用すると、自動検出プロセスが合理化されます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-144">Use the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="2e52b-145">このコード サンプルでは、次の表に示したコマンド ライン引数を使用して **PublicFolderInformation** SMTP アドレスの POX 自動検出サービスを呼び出しています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-145">This code sample uses the command line arguments listed in the following table to call the POX Autodiscover service on the **PublicFolderInformation** SMTP address.</span></span> 
  
|<span data-ttu-id="2e52b-146">**コマンド ライン引数**</span><span class="sxs-lookup"><span data-stu-id="2e52b-146">**Command-line argument**</span></span>|<span data-ttu-id="2e52b-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="2e52b-147">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e52b-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2e52b-148">emailAddress</span></span>  <br/> |<span data-ttu-id="2e52b-149">**PublicFolderInformation** SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="2e52b-149">The **PublicFolderInformation** SMTP address.</span></span>  <br/> |
|<span data-ttu-id="2e52b-150">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="2e52b-150">-skipSOAP</span></span>  <br/> | <span data-ttu-id="2e52b-151">このシナリオに、POX 自動検出要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-151">Use POX Autodiscover requests for this scenario.</span></span>  <br/> |
|<span data-ttu-id="2e52b-152">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="2e52b-152">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="2e52b-p110">認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-p110">The mailbox user's email address, which is used for authentication. You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="2e52b-155">たとえば、SharedPublicFolder@contoso.com が **PublicFolderInformation** 要素の SMTP アドレスで、sonyaf@contoso.com がメールボックス ユーザーのときに、コマンド ライン引数は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-155">For example, when SharedPublicFolder@contoso.com is the SMTP address of the **PublicFolderInformation** element, and sonyaf@contoso.com is the mailbox user, the command-line arguments should look like this.</span></span> 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="2e52b-156">「**Exchange 2013: Get user settings with Autodiscover**」のサンプルを実行すると、最後の自動検出応答は成功し、メールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-156">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="2e52b-157">EXCH [Protocol](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[Type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) 要素に関連付けられた [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) 値が **X-PublicFolderInformation** ヘッダー値になります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-157">The [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) value associated with the EXCH [Protocol](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[Type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) element is the **X-PublicFolderInformation** header value.</span></span> 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

<span data-ttu-id="2e52b-158">また、「**Exchange 2013: Get user settings with Autodiscover**」のサンプルを使用しない場合は、[自動検出エンドポイントの一覧を生成](how-to-generate-a-list-of-autodiscover-endpoints.md)することによって **Server** 値を取得してから、正常な応答を受信するまで次の POX 自動検出要求をそれぞれの URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-158">Alternatively, if you do not want to use the **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **Server** value by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span> <span data-ttu-id="2e52b-159">SharedPublicFolder@contoso.com が **X-PublicFolderMailbox** ヘッダーの値になります。</span><span class="sxs-lookup"><span data-stu-id="2e52b-159">SharedPublicFolder@contoso.com is the value of the **X-PublicFolderMailbox** header.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="2e52b-160">自動検出プロセスの詳細については、「[Exchange の自動検出](autodiscover-for-exchange.md)」、「[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)」、および「[自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e52b-160">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="2e52b-161">X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する</span><span class="sxs-lookup"><span data-stu-id="2e52b-161">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="2e52b-162"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="2e52b-162"><a name="bk_setheadervalues"> </a></span></span>

<span data-ttu-id="2e52b-163">「[EWS マネージ API を使用して X-AnchorMailbox ヘッダーの値を決定する](#bk_getpfinfoewsma)」または「[SOAP を使用して X-AnchorMailbox ヘッダーの値を決定する](#bk_getpfinfoews)」で取得した **PublicFolderInformation** SMTP アドレスの値と、「[自動検出要求によって X-PublicFolderInformation 値を決定する](#bk_makeautodrequest)」で取得した **Server** 値を使用して、パブリック フォルダー コンテンツ要求の **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-163">Using the value of the **PublicFolderInformation** SMTP address acquired in [Determine the value of the X-AnchorMailbox header by using the EWS Managed API](#bk_getpfinfoewsma) or [Determine the value of the X-AnchorMailbox header using SOAP](#bk_getpfinfoews) and the **Server** value acquired in [Make an Autodiscover request to determine the X-PublicFolderInformation value](#bk_makeautodrequest), set the values of **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="2e52b-164">たとえば、**PublicFolderInformation** SMTP アドレスが SharedPublicFolder@contoso.com で、**Server** 値が 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com だとすると、次に示すメソッドまたは操作の呼び出し時には、次に示すヘッダーを含めます。</span><span class="sxs-lookup"><span data-stu-id="2e52b-164">For example, given a **PublicFolderInformation** SMTP address of SharedPublicFolder@contoso.com and a **Server** value of 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, include the following headers when making calls to the following methods or operations.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

<span data-ttu-id="2e52b-165">**X-AnchorMailbox ヘッダーと X-PublicFolder ヘッダーが必要なパブリック フォルダーの呼び出し**</span><span class="sxs-lookup"><span data-stu-id="2e52b-165">**Public folder calls that require the X-AnchorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="2e52b-166">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="2e52b-166">**EWS Managed API methods**</span></span>|<span data-ttu-id="2e52b-167">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="2e52b-167">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e52b-168">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="2e52b-168">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="2e52b-169">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="2e52b-169">Folder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="2e52b-170">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="2e52b-170">Folder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="2e52b-171">Folder.Move</span><span class="sxs-lookup"><span data-stu-id="2e52b-171">Folder.Move</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2e52b-172">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="2e52b-172">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="2e52b-173">FindFolder</span><span class="sxs-lookup"><span data-stu-id="2e52b-173">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="2e52b-174">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="2e52b-174">DeleteFolder</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="2e52b-175">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="2e52b-175">UpdateFolder</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="2e52b-176">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="2e52b-176">MoveFolder</span></span>](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="2e52b-177">EWS マネージ API を使用してこれらのヘッダーを追加するには、[HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="2e52b-177">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

<span data-ttu-id="2e52b-178">たとえば、次のコードは、この記事の例で取得した値に **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーが設定されている [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="2e52b-178">For example, the following code shows a [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="2e52b-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="2e52b-179">See also</span></span>

- [<span data-ttu-id="2e52b-180">Exchange での EWS を使用したパブリック フォルダー アクセス</span><span class="sxs-lookup"><span data-stu-id="2e52b-180">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="2e52b-181">パブリック フォルダー コンテンツ要求のルーティング</span><span class="sxs-lookup"><span data-stu-id="2e52b-181">Route public folder content requests</span></span>](how-to-route-public-folder-content-requests.md)    
- [<span data-ttu-id="2e52b-182">EWS マネージ API を使用してユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="2e52b-182">Get user settings by using the EWS Managed API</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

