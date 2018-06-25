---
title: パブリック フォルダー階層の要求のルーティング
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: パブリック フォルダー情報の移動、更新、削除、パブリック フォルダーの検索など、パブリック フォルダー階層の知識を必要とするすべての要求は、特定のユーザーの既定のパブリック フォルダー階層メールボックスにルーティングする必要があります。 要求をそのメールボックスに転送するには、自動検出サービスによって返される特定の値に X AnchorMailbox X PublicFolderMailbox のヘッダーを設定する必要があります。
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759058"
---
# <a name="route-public-folder-hierarchy-requests"></a><span data-ttu-id="9360d-104">パブリック フォルダー階層の要求のルーティング</span><span class="sxs-lookup"><span data-stu-id="9360d-104">Route public folder hierarchy requests</span></span>

<span data-ttu-id="9360d-105">パブリック フォルダー情報の移動、更新、削除、パブリック フォルダーの検索など、パブリック フォルダー階層の知識を必要とするすべての要求は、特定のユーザーの既定のパブリック フォルダー階層メールボックスにルーティングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9360d-105">All requests for public folder information that require knowledge of the public folder hierarchy, such as moving, updating, deleting, or finding public folders, need to be routed to the default public folder hierarchy mailbox for the given user.</span></span> <span data-ttu-id="9360d-106">要求をそのメールボックスに転送するには、自動検出サービスによって返される特定の値に**X AnchorMailbox** **X PublicFolderMailbox**のヘッダーを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9360d-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values returned by the Autodiscover service.</span></span> 
  
<span data-ttu-id="9360d-107">**パブリック フォルダーの概要**</span><span class="sxs-lookup"><span data-stu-id="9360d-107">**Overview of public folders**</span></span>

|<span data-ttu-id="9360d-108">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9360d-108">Header</span></span>|<span data-ttu-id="9360d-109">必要なもの</span><span class="sxs-lookup"><span data-stu-id="9360d-109">What do I need?</span></span>|<span data-ttu-id="9360d-110">取得する方法</span><span class="sxs-lookup"><span data-stu-id="9360d-110">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9360d-111">**X AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="9360d-111">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="9360d-112">**X AnchorMailbox**ヘッダーの値になります[GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx)の自動検出の SOAP 応答から[PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx)の値です。</span><span class="sxs-lookup"><span data-stu-id="9360d-112">The [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value from a [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) Autodiscover SOAP response, which becomes the value of the **X-AnchorMailbox** header.</span></span><br/><br/> <span data-ttu-id="9360d-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span><span class="sxs-lookup"><span data-stu-id="9360d-113">![TODO](media/Ex15_PF_PFH_Anchor.png)</span></span>| <span data-ttu-id="9360d-114">1. ユーザーのメールボックスの SMTP アドレスを使用して**GetUserSetting**要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="9360d-114">1. Send a **GetUserSetting** request with the SMTP address for the user's mailbox.</span></span><br/><br/><span data-ttu-id="9360d-115">2. 自動検出サービスから返される**PublicFolderInformation**の要素の値をキャッシュします。</span><span class="sxs-lookup"><span data-stu-id="9360d-115">2. Cache the value of the **PublicFolderInformation** element that the Autodiscover service returns.</span></span> <span data-ttu-id="9360d-116">コード、または新しい[EWS マネージ API の GetUserSettings を呼び出す](#bk_getpfinfoewsma) [GetUserSettings の SOAP 要求](#bk_getpfinfoews)に既存の自動検出要求のキャッシュされていることができます。</span><span class="sxs-lookup"><span data-stu-id="9360d-116">This can be a cached from an existing Autodiscover call in your code, or a new [EWS Managed API GetUserSettings call](#bk_getpfinfoewsma) or a [GetUserSettings SOAP request](#bk_getpfinfoews).</span></span>  <br/><br/><span data-ttu-id="9360d-117">3. **X AnchorMailbox**のヘッダーの値を設定するのに**PublicFolderInformation**要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="9360d-117">3. Use the **PublicFolderInformation** element to populate the value of the **X-AnchorMailbox** header.</span></span> <span data-ttu-id="9360d-118">**PublicFolderInformation**要素の値は、SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9360d-118">The value of the **PublicFolderInformation** element is an SMTP address.</span></span>  <br/> |
|<span data-ttu-id="9360d-119">**X PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="9360d-119">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="9360d-120">[サーバー](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx)の値は、 [POX の自動検出の応答](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx)、 **X PublicFolderMailbox**のヘッダーの値となります。</span><span class="sxs-lookup"><span data-stu-id="9360d-120">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value from a [POX Autodiscover response](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), which becomes the value of the **X-PublicFolderMailbox** header.</span></span><br/><br/> <span data-ttu-id="9360d-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span><span class="sxs-lookup"><span data-stu-id="9360d-121">![TODO](media/Ex15_PF_PFH_PFMailbox.png)</span></span>|<span data-ttu-id="9360d-122">1。 POX の自動検出サービスの[呼び出し](#bk_makeautodrequest) **X AnchorMailbox**の電子メール アドレスを使用します。</span><span class="sxs-lookup"><span data-stu-id="9360d-122">1. [Call the POX Autodiscover](#bk_makeautodrequest) service using the **X-AnchorMailbox** email address.</span></span>  <br/><br/><span data-ttu-id="9360d-123">2. **X PublicFolderMailbox**のヘッダーの値を設定するのには、自動検出サービスによって返される**サーバー**の要素を使用します。</span><span class="sxs-lookup"><span data-stu-id="9360d-123">2. Use the **Server** element returned by the Autodiscover service to populate the value of the **X-PublicFolderMailbox** header.</span></span> <span data-ttu-id="9360d-124">**X PublicFolderMailbox**の値は、ユーザー名と GUID がある SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9360d-124">The value of the **X-PublicFolderMailbox** is an SMTP address where the username is a GUID.</span></span>  <br/> |

<br/>

<span data-ttu-id="9360d-125">ヘッダーの値を確認した後は、[パブリック フォルダー階層の要求を作成するとき](#bk_setheadervalues)に含めます。</span><span class="sxs-lookup"><span data-stu-id="9360d-125">After you have determined the header values, include them [when you make public folder hierarchy requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="9360d-126">この資料の手順は、パブリック フォルダー階層の要求に固有です。</span><span class="sxs-lookup"><span data-stu-id="9360d-126">The steps in this article are specific to public folder hierarchy requests.</span></span> <span data-ttu-id="9360d-127">要求は、パブリック フォルダー階層またはコンテンツの要求かどうかを確認するのには、[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9360d-127">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a><span data-ttu-id="9360d-128">EWS マネージ API を使用して X-AnchorMailbox ヘッダーの値を決定する</span><span class="sxs-lookup"><span data-stu-id="9360d-128">Determine the value of the X-AnchorMailbox header by using the EWS Managed API</span></span>
<span data-ttu-id="9360d-129"><a name="bk_getpfinfoewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="9360d-129"></span></span>

<span data-ttu-id="9360d-130">[PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx)の値を取得するには、EWS のマネージ API を使用して、自動検出サービスへの既存の呼び出しが返されると、 **PublicFolderInformation**要素の値をキャッシュするか、新しい呼び出しを実行します。</span><span class="sxs-lookup"><span data-stu-id="9360d-130">To retrieve the [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) value by using the EWS Managed API, you can either cache the value of the **PublicFolderInformation** element that an existing call to the Autodiscover service returns, or make a new call.</span></span> 
  
<span data-ttu-id="9360d-131">新しい呼び出しを作成する場合、 **GetUserSettings**を取得する次のコードを使用してメソッドのサンプル コード、およびその後の呼び出しに[EWS のマネージ API を使用してユーザー設定の取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)を[EWS のマネージ API を使用してユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)することができます。**PublicFolderInformation**要素の値のみです。</span><span class="sxs-lookup"><span data-stu-id="9360d-131">If you're making a new call, you can [Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[Get user settings by using the EWS Managed API](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) to your code, and then call the **GetUserSettings** sample method by using the following code, which retrieves only the value of the **PublicFolderInformation** element.</span></span> <span data-ttu-id="9360d-132">入力パラメーターとしてメールボックスのユーザーの SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9360d-132">Include the SMTP address of the mailbox user as an input parameter.</span></span> 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

<span data-ttu-id="9360d-133">コードを実行すると、次の情報がコンソールに表示されます。</span><span class="sxs-lookup"><span data-stu-id="9360d-133">After running the code, the following information is displayed on the console:</span></span>
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

<span data-ttu-id="9360d-134">これで**PublicFolderInformation**の値がある場合は、パブリック フォルダー階層のすべての要求で X AnchorMailbox ヘッダーの値として含まれます。</span><span class="sxs-lookup"><span data-stu-id="9360d-134">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a><span data-ttu-id="9360d-135">SOAP を使用して X-AnchorMailbox ヘッダーの値を決定する</span><span class="sxs-lookup"><span data-stu-id="9360d-135">Determine the value of the X-AnchorMailbox header using SOAP</span></span>
<span data-ttu-id="9360d-136"><a name="bk_getpfinfoews"> </a></span><span class="sxs-lookup"><span data-stu-id="9360d-136"></span></span>

<span data-ttu-id="9360d-137">[GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP 操作を使用して、 **PublicFolderInformation**値を取得する方法を次のコード例に示します。</span><span class="sxs-lookup"><span data-stu-id="9360d-137">The following code example shows how to retrieve the **PublicFolderInformation** value by using the [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP operation.</span></span> <span data-ttu-id="9360d-138">メールボックス ユーザーが[メールボックス](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx)要素で指定されているし、 [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx)要素は、 [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx)の値への応答を制限します。</span><span class="sxs-lookup"><span data-stu-id="9360d-138">The mailbox user is specified in the [Mailbox](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) element, and the [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) element limits the response to the [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) value.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

<span data-ttu-id="9360d-139">応答には、 **PublicFolderInformation**の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9360d-139">The response includes the **PublicFolderInformation** value.</span></span> 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

<span data-ttu-id="9360d-140">これで**PublicFolderInformation**の値がある場合は、パブリック フォルダー階層のすべての要求で X AnchorMailbox ヘッダーの値として含まれます。</span><span class="sxs-lookup"><span data-stu-id="9360d-140">Now that you have the **PublicFolderInformation** value, include it as the value for the X-AnchorMailbox header in all public folder hierarchy requests.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a><span data-ttu-id="9360d-141">自動検出要求によって X-PublicFolderInformation 値を決定する</span><span class="sxs-lookup"><span data-stu-id="9360d-141">Make an Autodiscover request to determine the X-PublicFolderInformation value</span></span>
<span data-ttu-id="9360d-142"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="9360d-142"></span></span>

<span data-ttu-id="9360d-143">**X AnchorMailbox**の値として使用しています**PublicFolderInformation**の SMTP アドレスを使用して、自動検出要求を行います。</span><span class="sxs-lookup"><span data-stu-id="9360d-143">Make an Autodiscover request by using the **PublicFolderInformation** SMTP address, which is now being used as the **X-AnchorMailbox** value.</span></span> <span data-ttu-id="9360d-144">使用、 [Exchange 2013: 自動検出とユーザー設定を取得する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)の自動検出プロセスを合理化するために自動検出サービスを呼び出すためのコード サンプルです。</span><span class="sxs-lookup"><span data-stu-id="9360d-144">Use the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="9360d-145">このコード サンプルでは、次の表に記載されているコマンドライン引数を使用して、 **PublicFolderInformation**の SMTP アドレスの POX の自動検出サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="9360d-145">This code sample uses the command line arguments listed in the following table to call the POX Autodiscover service on the **PublicFolderInformation** SMTP address.</span></span> 
  
|<span data-ttu-id="9360d-146">**コマンドライン引数**</span><span class="sxs-lookup"><span data-stu-id="9360d-146">**Command-line argument**</span></span>|<span data-ttu-id="9360d-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="9360d-147">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9360d-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9360d-148">emailAddress</span></span>  <br/> |<span data-ttu-id="9360d-149">**PublicFolderInformation** SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9360d-149">The **PublicFolderInformation** SMTP address.</span></span>  <br/> |
|<span data-ttu-id="9360d-150">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="9360d-150">-skipSOAP</span></span>  <br/> | <span data-ttu-id="9360d-151"> このシナリオに、POX 自動検出要求を使用します。</span><span class="sxs-lookup"><span data-stu-id="9360d-151">Use POX Autodiscover requests for this scenario.</span></span>  <br/> |
|<span data-ttu-id="9360d-152">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9360d-152">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="9360d-p110">認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="9360d-p110">The mailbox user's email address, which is used for authentication. You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="9360d-155">たとえば、SharedPublicFolder@contoso.com、 **PublicFolderInformation**要素の SMTP アドレスは、sonyaf@contoso.com メールボックス ユーザー、コマンドライン引数する必要がありますこれのようになります。</span><span class="sxs-lookup"><span data-stu-id="9360d-155">For example, when SharedPublicFolder@contoso.com is the SMTP address of the **PublicFolderInformation** element, and sonyaf@contoso.com is the mailbox user, the command-line arguments should look like this.</span></span> 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="9360d-156">実行すると、 **Exchange 2013: 自動検出とユーザー設定を取得する**サンプルでは、最後の自動検出応答する必要がありますが成功してメールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9360d-156">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="9360d-157">EXCH[プロトコル](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)の[種類](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx)の要素に関連付けられている[サーバー](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx)の値は、 **X PublicFolderInformation**のヘッダーの値です。</span><span class="sxs-lookup"><span data-stu-id="9360d-157">The [Server](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) value associated with the EXCH [Protocol](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)[Type](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) element is the **X-PublicFolderInformation** header value.</span></span> 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

<span data-ttu-id="9360d-158">またはを使用したくない場合、 **Exchange 2013: 自動検出でユーザー設定を取得する**サンプルでは、[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)に、次の POX の自動検出を送信し、**サーバー**の値を取得できます正常な応答を受信するまでは、各 URL に要求します。</span><span class="sxs-lookup"><span data-stu-id="9360d-158">Alternatively, if you do not want to use the **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **Server** value by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span> <span data-ttu-id="9360d-159">SharedPublicFolder@contoso.com は、 **X PublicFolderMailbox**のヘッダーの値です。</span><span class="sxs-lookup"><span data-stu-id="9360d-159">SharedPublicFolder@contoso.com is the value of the **X-PublicFolderMailbox** header.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="9360d-160">自動検出プロセスの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)、[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)、および[ユーザー設定の自動検出を使用して Exchange からの取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9360d-160">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="9360d-161">X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する</span><span class="sxs-lookup"><span data-stu-id="9360d-161">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="9360d-162"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="9360d-162"></span></span>

<span data-ttu-id="9360d-163">[EWS のマネージ API を使用して X AnchorMailbox ヘッダーの値を決定する](#bk_getpfinfoewsma)または[SOAP を使用して X AnchorMailbox ヘッダーの値を決定](#bk_getpfinfoews)し、**サーバーで取得した**PublicFolderInformation** SMTP アドレスの値を使用します。** [X PublicFolderInformation の値を確認するのには、自動検出要求を行う](#bk_makeautodrequest)で取得した値、パブリック フォルダー コンテンツ要求の**X AnchorMailbox** **X PublicFolderMailbox**ヘッダーの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="9360d-163">Using the value of the **PublicFolderInformation** SMTP address acquired in [Determine the value of the X-AnchorMailbox header by using the EWS Managed API](#bk_getpfinfoewsma) or [Determine the value of the X-AnchorMailbox header using SOAP](#bk_getpfinfoews) and the **Server** value acquired in [Make an Autodiscover request to determine the X-PublicFolderInformation value](#bk_makeautodrequest), set the values of **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="9360d-164">たとえば、 **PublicFolderInformation** SMTP アドレスは SharedPublicFolder@contoso.com と 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com の**サーバー**の値を指定するには、次のヘッダーには、次の呼び出しを実行するときメソッドまたは操作します。</span><span class="sxs-lookup"><span data-stu-id="9360d-164">For example, given a **PublicFolderInformation** SMTP address of SharedPublicFolder@contoso.com and a **Server** value of 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, include the following headers when making calls to the following methods or operations.</span></span> 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

<span data-ttu-id="9360d-165">**X AnchorMailbox と X-パブリック フォルダーのヘッダーを必要とするパブリック フォルダーの呼び出し**</span><span class="sxs-lookup"><span data-stu-id="9360d-165">**Public folder calls that require the X-AnchorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="9360d-166">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="9360d-166">**EWS Managed API methods**</span></span>|<span data-ttu-id="9360d-167">**EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="9360d-167">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9360d-168">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="9360d-168">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9360d-169">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="9360d-169">Folder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9360d-170">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="9360d-170">Folder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9360d-171">Folder.Move</span><span class="sxs-lookup"><span data-stu-id="9360d-171">Folder.Move</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9360d-172">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="9360d-172">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [<span data-ttu-id="9360d-173">FindFolder</span><span class="sxs-lookup"><span data-stu-id="9360d-173">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [<span data-ttu-id="9360d-174">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="9360d-174">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [<span data-ttu-id="9360d-175">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9360d-175">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [<span data-ttu-id="9360d-176">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="9360d-176">MoveFolder</span></span>](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="9360d-177">EWS のマネージ API を使用して、これらのヘッダーを追加するには、 [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx)メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="9360d-177">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

<span data-ttu-id="9360d-178">たとえば、次のコードでは、この資料の例で取得した値に設定し、 **X AnchorMailbox** **X PublicFolderMailbox**のヘッダーを持つ[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="9360d-178">For example, the following code shows a [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="see-also"></a><span data-ttu-id="9360d-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="9360d-179">See also</span></span>

- [<span data-ttu-id="9360d-180">Exchange での EWS を使用したパブリック フォルダー アクセス</span><span class="sxs-lookup"><span data-stu-id="9360d-180">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="9360d-181">パブリック フォルダー コンテンツの要求をルーティングします。</span><span class="sxs-lookup"><span data-stu-id="9360d-181">Route public folder content requests</span></span>](how-to-route-public-folder-content-requests.md)    
- [<span data-ttu-id="9360d-182">EWS のマネージ API を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="9360d-182">Get user settings by using the EWS Managed API</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

