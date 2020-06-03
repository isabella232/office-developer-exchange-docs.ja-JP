---
title: パブリック フォルダーのコンテンツ要求のルーティング
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: パブリック フォルダーのコンテンツを含むパブリック フォルダーの情報の要求はすべて、ターゲット フォルダーのコンテンツを保持するパブリック フォルダー メールボックスにルーティングされる必要があります。そのメールボックスへの要求をルーティングするには、X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーを特定の値に設定する必要があります。
ms.openlocfilehash: 523b9c8efc65253f7970fffeb5800e451784522d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527741"
---
# <a name="route-public-folder-content-requests"></a><span data-ttu-id="9ae8d-104">パブリック フォルダーのコンテンツ要求のルーティング</span><span class="sxs-lookup"><span data-stu-id="9ae8d-104">Route public folder content requests</span></span>

<span data-ttu-id="9ae8d-p102">パブリック フォルダーのコンテンツを含むパブリック フォルダーの情報の要求はすべて、ターゲット フォルダーのコンテンツを保持するパブリック フォルダー メールボックスにルーティングされる必要があります。そのメールボックスへの要求をルーティングするには、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーを特定の値に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p102">All requests for public folder information that involve the content of the public folder need to be routed to the public folder mailbox that holds the content for the target folder. To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values.</span></span> 
  
<span data-ttu-id="9ae8d-107">次の表では、このプロセスの概要を説明します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-107">The following table provides an overview of the process:</span></span>
  
<span data-ttu-id="9ae8d-108">**パブリック フォルダーの概要**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-108">**Public folder overview**</span></span>

|<span data-ttu-id="9ae8d-109">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ae8d-109">Header</span></span>|<span data-ttu-id="9ae8d-110">必要なもの</span><span class="sxs-lookup"><span data-stu-id="9ae8d-110">What do I need?</span></span>|<span data-ttu-id="9ae8d-111">取得する方法</span><span class="sxs-lookup"><span data-stu-id="9ae8d-111">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9ae8d-112">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-112">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="9ae8d-113">1. パブリック フォルダー階層メールボックス用の [X-AnchorMailbox と X-PublicFolderInformation の値](how-to-route-public-folder-hierarchy-requests.md)。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-113">1. [The X-AnchorMailbox and X-PublicFolderInformation values ](how-to-route-public-folder-hierarchy-requests.md) for the public folder hierarchy mailbox.</span></span><br/><br/><span data-ttu-id="9ae8d-114">2. メールボックスのコンテンツを含むパブリック フォルダー メールボックスの GUID。これは自動検出サービスに送信されます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-114">2. The GUID of the public folder mailbox that contains the mailbox content, which is sent to the Autodiscover service.</span></span><br/><br/>  <span data-ttu-id="9ae8d-115">自動検出の応答の **AutoDiscoverSMTPAddress** が **X-AnchorMailbox** ヘッダーの値になります。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-115">The **AutoDiscoverSMTPAddress** in the Autodisover response becomes the value of the **X-AnchorMailbox** header.</span></span>  <br/> <span data-ttu-id="9ae8d-116">![TODO](media/Ex15_PF_PFContent.png)</span><span class="sxs-lookup"><span data-stu-id="9ae8d-116">![TODO](media/Ex15_PF_PFContent.png)</span></span>| <span data-ttu-id="9ae8d-117">1. この記事にある、[EWS マネージ API を実装する](#bk_determineguidewsma)コード例を使用します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-117">1. Use the code example in this article, which [implements the EWS Managed API](#bk_determineguidewsma).</span></span> <span data-ttu-id="9ae8d-118">または、[EWS を使用](#bk_determineguidews)し、結果を変換して GUID を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-118">Or [use EWS](#bk_determineguidews) and convert your results to obtain a GUID.</span></span><br/><br/><span data-ttu-id="9ae8d-119">2. GUID とドメイン名を使用して、[自動検出を要求](#bk_makeautodrequest)します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-119">2. [Make an Autodiscover request](#bk_makeautodrequest) by using the GUID plus the domain name.</span></span><br/><br/><span data-ttu-id="9ae8d-120">3. 自動検出の応答で返された **AutoDiscoverSMTPAddress** 要素の値を使用して、[ヘッダーの値を設定](#bk_setheadervalues)します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-120">3. Use the value of the **AutoDiscoverSMTPAddress** element returned in the Autodiscover response to [populate the value of the headers](#bk_setheadervalues).</span></span>  <br/> |
|<span data-ttu-id="9ae8d-121">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-121">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="9ae8d-122">作業は完了しています。X-PublicFolderMailbox の値は X-AnchorMailbox の値と同じです。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-122">Your work is done, the X-PublicFolderMailbox value is the same as the X-AnchorMailbox value!</span></span>  <br/> |<span data-ttu-id="9ae8d-123">既に取得済みです。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-123">You already have it!</span></span>  <br/> |
   
<span data-ttu-id="9ae8d-124">ヘッダーの値が決定したら、それらを[パブリック フォルダーのコンテンツ要求を行うときに](#bk_setheadervalues)含めます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-124">After you have determined the header values, include them [when you make public folder content requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="9ae8d-p104">この記事の手順は、パブリック フォルダー コンテンツの要求に固有のものです。要求がパブリック フォルダー階層かコンテンツ要求かを特定するには、「[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p104">The steps in this article are specific to public folder content requests. To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>

<span data-ttu-id="9ae8d-127"><a name="bk_determineguidewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae8d-127"><a name="bk_determineguidewsma"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a><span data-ttu-id="9ae8d-128">EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-128">Determine the GUID of the public folder mailbox by using the EWS Managed API</span></span>


<span data-ttu-id="9ae8d-129">パブリック フォルダーのコンテンツ メールボックスの GUID を特定するには、次の動作を実行する以下のコード例を使用します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-129">To determine the GUID of the public folder content mailbox, use the following code example, which does the following:</span></span> 
  
- <span data-ttu-id="9ae8d-130">[パブリック フォルダー階層の要求をルーティング](how-to-route-public-folder-hierarchy-requests.md)して取得した **X-AnchorMailbox** ヘッダーと **X-PublicFolderInformation** ヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-130">Uses the **X-AnchorMailbox** and **X-PublicFolderInformation** headers you retrieved by [routing public folder hierarchy requests](how-to-route-public-folder-hierarchy-requests.md).</span></span>
    
- <span data-ttu-id="9ae8d-131">EWS マネージ API の [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) メソッドを呼び出して、**PR_REPLICA_LIST** (0x66980102) プロパティの要求を含めます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-131">Calls the EWS Managed API [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method, and includes a request for the **PR_REPLICA_LIST** (0x66980102) property</span></span> 
    
<span data-ttu-id="9ae8d-p105">**PR_REPLICA_LIST** の値は、フォルダーのコンテンツを含むパブリック フォルダー メールボックスのメールボックス GUID を識別します。**PR_REPLICA_LIST** プロパティはバイト配列ですが、このシナリオでは GUID としてキャストされます。GUID とドメイン名が連結されて、自動検出を呼び出すためのアドレスが形成されます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p105">The **PR_REPLICA_LIST** value identifies the mailbox GUID of the public folder mailbox that has the content for the folder. The **PR_REPLICA_LIST** property is a byte array, but is cast as a GUID for this scenario. The GUID and the domain name are concatenated to form the address on which to call Autodiscover.</span></span> 
  
<span data-ttu-id="9ae8d-135">この例では、`service` をメールボックス ユーザーの [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、`PFHAnchorHeader` と `PFHMailboxHeader` を **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値、ドメインをテナントによって使用されるドメイン名とします。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-135">This example assumes that  `service` is the [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox user,  `PFHAnchorHeader` and  `PFHMailboxHeader` are the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers, and domain is the domain name used by the tenant.</span></span> 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

<span data-ttu-id="9ae8d-p106">"要求が失敗しました。基になる接続が閉じられました。SSL/TLS のセキュリティで保護されているチャネルに対する信頼関係を確立できませんでした" というエラーが発生したら、[検証コールバック メソッドの呼び出しを追加](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。そのメソッドのプレースホルダーとコメントはコード例に含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p106">If you received the error "The request failed. The underlying connection was closed: Could not establish trust relationship for the SSL/TLS secure channel", you'll need to [add a call to a validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). A placeholder and comment for that method is included in the code example.</span></span>
  
<span data-ttu-id="9ae8d-139">メールボックスの GUID がパブリック フォルダー ルートにあるすべてのパブリック フォルダーで統一されている場合、この例は、コンソール出力で[自動検出を呼び出す](#bk_makeautodrequest)ときに使用するアドレスを戻り値として示します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-139">If the mailbox GUID is the same for all the public folders under the public folder root, the example indicates the address to use when [calling Autodiscover](#bk_makeautodrequest) in the console output and as the return value.</span></span> <span data-ttu-id="9ae8d-140">メールボックスの GUID がパブリック フォルダー ルートにあるすべてのパブリック フォルダーで統一されていない場合、コンテンツ要求のフォルダーに関連付けられているアドレスで[自動検出を要求する](#bk_makeautodrequest)必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-140">If the mailbox GUID is not the same for all public folders under the public folder root, you need to [Make an Autodiscover request](#bk_makeautodrequest) on the address associated with the folder in your content request.</span></span> 

<span data-ttu-id="9ae8d-141"><a name="bk_determineguidews"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae8d-141"><a name="bk_determineguidews"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a><span data-ttu-id="9ae8d-142">EWS を使用してパブリック フォルダー メールボックスの GUID を特定する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-142">Determine the GUID of the public folder mailbox by using EWS</span></span>

<span data-ttu-id="9ae8d-p108">次のコード例では、EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 操作を使用して **PR_REPLICA_LIST** (0x66980102) プロパティの値を取得する方法を示します。[ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素の、**PropertyTag** 属性は **PR_REPLICA_LIST** プロパティの 10 進数 (26264) に、**PropertyType** 属性は **Binary** に設定します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p108">The following code example shows how retrieve the value of the **PR_REPLICA_LIST** (0x66980102) property by using the EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation. For the [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, the **PropertyTag** attribute is set to the decimal value (26264) of the **PR_REPLICA_LIST** property, and the **PropertyType** attribute is set to **Binary**.</span></span>
  
<span data-ttu-id="9ae8d-145">これは、[EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定](#bk_determineguidewsma)するために **FindFolders** メソッドを使用するときに、EWS マネージ API が送信する XML 要求です。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-145">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [determine the GUID of the public folder mailbox by using the EWS Managed API](#bk_determineguidewsma).</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="9ae8d-p109">サーバーは、**FindFolder** 要求に対して **PR_REPLICA_LIST** の拡張プロパティの値を含む [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) メッセージで応答します。プロパティの値は、Base-64 のエンコードされたバイト配列の文字列形式として EWS 応答に表れることに注意してください。応答内のいくつかのヘッダー値は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p109">The server responds to the **FindFolder** request with a [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes the value of the **PR_REPLICA_LIST** extended property. Note that the value of the property appears on the EWS response as the string format of a base-64 encoded byte array. Some header values in the response are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="9ae8d-p110">XML で返された **PR_REPLICA_LIST** の値 (MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==) を使用してメールボックス GUID を特定するには、[EWS マネージ API のコード例](#bk_determineguidewsma)で値が変換されたのと同様の形式で値を GUID に変換する必要があります。その後、GUID はドメイン名と連結されて SMTP アドレスが作成されます。このアドレスは[自動検出要求](#bk_makeautodrequest)に含まれます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p110">In order to use the value of the **PR_REPLICA_LIST** returned in the XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, to determine the mailbox GUID, the value must be converted into a GUID in a format similar to how the value is converted in the [EWS Managed API code example](#bk_determineguidewsma). The GUID is then concatenated with the domain name to create an SMTP address, which is included in the [Autodiscover request](#bk_makeautodrequest).</span></span>
  
## <a name="make-an-autodiscover-request"></a><span data-ttu-id="9ae8d-151">自動検出を要求する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-151">Make an Autodiscover request</span></span>
<span data-ttu-id="9ae8d-152"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae8d-152"><a name="bk_makeautodrequest"> </a></span></span>

<span data-ttu-id="9ae8d-153">`GetMailboxGuidAddress` メソッドによって返されたアドレスを使用して自動検出を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-153">Use the address returned by the  `GetMailboxGuidAddress` method to call Autodiscover.</span></span> <span data-ttu-id="9ae8d-154">「[Exchange 2013: 自動検出によるユーザー設定の取得](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)」のコード例を使用して、自動検出サービスを呼び出すことをお勧めします。これは、このコード例が自動検出プロセスを効率化するためです。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-154">We recommend that you use the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="9ae8d-155">このコード例では、次の表に記載されているコマンドライン引数を使用して POX 自動検出サービスを呼び出し、メールボックスの GUID に関連付けられている [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-155">This code sample uses the command-line arguments listed in the following table to call the POX Autodiscover service to retrieve the [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) value associated with the mailbox GUID.</span></span> 

  
|<span data-ttu-id="9ae8d-156">**引数**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-156">**Argument**</span></span>|<span data-ttu-id="9ae8d-157">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-157">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ae8d-158">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9ae8d-158">emailAddress</span></span>  <br/> |<span data-ttu-id="9ae8d-159">[パブリック フォルダー メールボックスの GUID を特定する](#bk_determineguidewsma)で、`GetMailboxGuidAddress` メソッドによって返されたアドレスです。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-159">The address returned by the  `GetMailboxGuidAddress` method in [Determine the GUID of the public folder mailbox](#bk_determineguidewsma).</span></span>  <br/> |
|<span data-ttu-id="9ae8d-160">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="9ae8d-160">-skipSOAP</span></span>  <br/> |<span data-ttu-id="9ae8d-161">POX 自動検出要求が必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-161">Indicates that POX Autodiscover requests are required.</span></span>  <br/> |
|<span data-ttu-id="9ae8d-162">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9ae8d-162">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="9ae8d-p112">認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p112">The mailbox user's email address, which is used for authentication. You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="9ae8d-165">たとえば、コマンドライン引数は次のようになります。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-165">For example, the command-line arguments should look like this:</span></span>
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="9ae8d-166">ここで、`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` は **GetMailboxGuidAddress** メソッドによって返されたアドレスで、`sonyaf@contoso.com` はメールボックス ユーザーです。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-166">Where `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` is the address returned by the **GetMailboxGuidAddress** method, and `sonyaf@contoso.com` is the mailbox user.</span></span> 
  
<span data-ttu-id="9ae8d-p113">**Exchange 2013: Get user settings with Autodiscover** のサンプルを実行すると、最後の自動検出応答は成功し、メールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。次の手順で使用するので、ローカルに **AutoDiscoverSMTPAddress** ユーザー設定を保存します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-p113">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID. Save the **AutoDiscoverSMTPAddress** user setting locally, as you'll use that in the next step.</span></span> 
  
<span data-ttu-id="9ae8d-169">または、**Exchange 2013: Get user settings with Autodiscover** のサンプルを使用しない場合は、[自動検出エンドポイントの一覧を生成](how-to-generate-a-list-of-autodiscover-endpoints.md)することによって **AutoDiscoverSMTPAddress** ユーザー設定を取得してから、正常な応答を受信するまで次の POX 自動検出要求をそれぞれの URL に送信します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-169">Alternatively, if you do not want to use **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **AutoDiscoverSMTPAddress** user setting by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="9ae8d-170">自動検出プロセスの詳細については、「[Exchange の自動検出](autodiscover-for-exchange.md)」、「[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)」、および「[自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-170">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="9ae8d-171">X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-171">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="9ae8d-172"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="9ae8d-172"><a name="bk_setheadervalues"> </a></span></span>

<span data-ttu-id="9ae8d-173">[自動検出要求を作成する](#bk_makeautodrequest)で取得した **AutoDiscoverSMTPAddress** の値を使用して、パブリック フォルダー コンテンツ要求に **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-173">Using the value for the **AutoDiscoverSMTPAddress** acquired in [Make an Autodiscover request](#bk_makeautodrequest), set the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="9ae8d-174">たとえば、NewPublicFolder@contoso.com の AutoDiscoverSMTPAddress が指定されている場合は、以下のメソッドまたは操作の呼び出し時に、次のヘッダーを含めます。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-174">For example, given an AutoDiscoverSMTPAddress of NewPublicFolder@contoso.com, include the following headers when making calls to the following methods or operations.</span></span>
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

<span data-ttu-id="9ae8d-175">**X-AncorMailbox ヘッダーと X-PublicFolder ヘッダーが必要なパブリック フォルダー呼び出し**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-175">**Public folder calls that require the X-AncorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="9ae8d-176">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-176">**EWS Managed API methods**</span></span>|<span data-ttu-id="9ae8d-177">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="9ae8d-177">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ae8d-178">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="9ae8d-178">Item.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-179">Item.Update</span><span class="sxs-lookup"><span data-stu-id="9ae8d-179">Item.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-180">Item.Copy</span><span class="sxs-lookup"><span data-stu-id="9ae8d-180">Item.Copy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-181">Item.Move</span><span class="sxs-lookup"><span data-stu-id="9ae8d-181">Item.Move</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-182">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="9ae8d-182">Item.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-183">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="9ae8d-183">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="9ae8d-184">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="9ae8d-184">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="9ae8d-185">CreateItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-185">CreateItem</span></span>](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-186">GetItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-186">GetItem</span></span>](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-187">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-187">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-188">CopyItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-188">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-189">MoveItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-189">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-190">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-190">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> [<span data-ttu-id="9ae8d-191">GetFolder</span><span class="sxs-lookup"><span data-stu-id="9ae8d-191">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="9ae8d-192">FindItem</span><span class="sxs-lookup"><span data-stu-id="9ae8d-192">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="9ae8d-193">EWS マネージ API を使用してこれらのヘッダーを追加するには、[HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-193">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

<span data-ttu-id="9ae8d-194">次のコードは、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーがこの記事の例で取得した値に設定されている [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を示します。</span><span class="sxs-lookup"><span data-stu-id="9ae8d-194">The following code shows a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="9ae8d-195">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ae8d-195">See also</span></span>

- [<span data-ttu-id="9ae8d-196">Exchange での EWS を使用したパブリック フォルダー アクセス</span><span class="sxs-lookup"><span data-stu-id="9ae8d-196">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="9ae8d-197">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="9ae8d-197">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="9ae8d-198">自動検出エンドポイントの一覧を生成する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-198">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [<span data-ttu-id="9ae8d-199">自動検出を使用して Exchange からユーザー設定を取得する</span><span class="sxs-lookup"><span data-stu-id="9ae8d-199">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  