---
title: パブリック フォルダー コンテンツの要求をルーティングします。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: ターゲット フォルダーのコンテンツを保持するパブリック フォルダーのパブリック フォルダーのメールボックスにルーティングする必要性の内容に関連するパブリック フォルダーの情報のすべての要求。 要求をそのメールボックスに転送するには、特定の値に X AnchorMailbox X PublicFolderMailbox のヘッダーを設定する必要があります。
ms.openlocfilehash: ad36c1526a24d815ec690879d633774d429ed36c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759065"
---
# <a name="route-public-folder-content-requests"></a><span data-ttu-id="91db9-104">パブリック フォルダー コンテンツの要求をルーティングします。</span><span class="sxs-lookup"><span data-stu-id="91db9-104">Route public folder content requests</span></span>

<span data-ttu-id="91db9-105">ターゲット フォルダーのコンテンツを保持するパブリック フォルダーのパブリック フォルダーのメールボックスにルーティングする必要性の内容に関連するパブリック フォルダーの情報のすべての要求。</span><span class="sxs-lookup"><span data-stu-id="91db9-105">All requests for public folder information that involve the content of the public folder need to be routed to the public folder mailbox that holds the content for the target folder.</span></span> <span data-ttu-id="91db9-106">要求をそのメールボックスに転送するには、特定の値に**X AnchorMailbox** **X PublicFolderMailbox**のヘッダーを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="91db9-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values.</span></span> 
  
<span data-ttu-id="91db9-107">次の表では、このプロセスの概要を説明します。</span><span class="sxs-lookup"><span data-stu-id="91db9-107">The following table provides an overview of the process:</span></span>
  
<span data-ttu-id="91db9-108">**パブリック フォルダーの概要**</span><span class="sxs-lookup"><span data-stu-id="91db9-108">**Public folder overview**</span></span>

|<span data-ttu-id="91db9-109">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91db9-109">Header</span></span>|<span data-ttu-id="91db9-110">必要なもの</span><span class="sxs-lookup"><span data-stu-id="91db9-110">What do I need?</span></span>|<span data-ttu-id="91db9-111">取得する方法</span><span class="sxs-lookup"><span data-stu-id="91db9-111">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="91db9-112">**X AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="91db9-112">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="91db9-113">1。 [X PublicFolderInformation の値、X AnchorMailbox](how-to-route-public-folder-hierarchy-requests.md)のパブリック フォルダー階層メールボックスです。</span><span class="sxs-lookup"><span data-stu-id="91db9-113">1. [The X-AnchorMailbox and X-PublicFolderInformation values ](how-to-route-public-folder-hierarchy-requests.md) for the public folder hierarchy mailbox.</span></span><br/><br/><span data-ttu-id="91db9-114">2. は自動検出サービスに送信されたメールボックスのコンテンツを格納するパブリック フォルダーのメールボックスの GUID です。</span><span class="sxs-lookup"><span data-stu-id="91db9-114">2. The GUID of the public folder mailbox that contains the mailbox content, which is sent to the Autodiscover service.</span></span><br/><br/>  <span data-ttu-id="91db9-115">Autodisover の応答で**AutoDiscoverSMTPAddress**では、 **X AnchorMailbox**のヘッダーの値になります。</span><span class="sxs-lookup"><span data-stu-id="91db9-115">The **AutoDiscoverSMTPAddress** in the Autodisover response becomes the value of the **X-AnchorMailbox** header.</span></span>  <br/> <span data-ttu-id="91db9-116">![TODO](media/Ex15_PF_PFContent.png)</span><span class="sxs-lookup"><span data-stu-id="91db9-116">![TODO](media/Ex15_PF_PFContent.png)</span></span>| <span data-ttu-id="91db9-117">1.、 [EWS のマネージ API を実装して](#bk_determineguidewsma)、この資料のコード例を使用します。</span><span class="sxs-lookup"><span data-stu-id="91db9-117">1. Use the code example in this article, which [implements the EWS Managed API](#bk_determineguidewsma).</span></span> <span data-ttu-id="91db9-118">または[EWS を使用](#bk_determineguidews)し、GUID を取得するのには、結果を変換します。</span><span class="sxs-lookup"><span data-stu-id="91db9-118">Or [use EWS](#bk_determineguidews) and convert your results to obtain a GUID.</span></span><br/><br/><span data-ttu-id="91db9-119">2。 GUID とドメイン名を使用しての[自動検出要求を作成](#bk_makeautodrequest)します。</span><span class="sxs-lookup"><span data-stu-id="91db9-119">2. [Make an Autodiscover request](#bk_makeautodrequest) by using the GUID plus the domain name.</span></span><br/><br/><span data-ttu-id="91db9-120">3.[ヘッダーの値を設定](#bk_setheadervalues)するのには自動検出の応答で返される**AutoDiscoverSMTPAddress**の要素の値を使用します。</span><span class="sxs-lookup"><span data-stu-id="91db9-120">3. Use the value of the **AutoDiscoverSMTPAddress** element returned in the Autodiscover response to [populate the value of the headers](#bk_setheadervalues).</span></span>  <br/> |
|<span data-ttu-id="91db9-121">**X PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="91db9-121">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="91db9-122">作業は完了しています。X-PublicFolderMailbox の値は X-AnchorMailbox の値と同じです。</span><span class="sxs-lookup"><span data-stu-id="91db9-122">Your work is done, the X-PublicFolderMailbox value is the same as the X-AnchorMailbox value!</span></span>  <br/> |<span data-ttu-id="91db9-123">既に取得済みです。</span><span class="sxs-lookup"><span data-stu-id="91db9-123">You already have it!</span></span>  <br/> |
   
<span data-ttu-id="91db9-124">ヘッダーの値を確認した後は、[パブリック フォルダー コンテンツの要求を作成するとき](#bk_setheadervalues)に含めます。</span><span class="sxs-lookup"><span data-stu-id="91db9-124">After you have determined the header values, include them [when you make public folder content requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="91db9-125">この資料の手順は、パブリック フォルダーのコンテンツ要求に固有です。</span><span class="sxs-lookup"><span data-stu-id="91db9-125">The steps in this article are specific to public folder content requests.</span></span> <span data-ttu-id="91db9-126">要求は、パブリック フォルダー階層またはコンテンツの要求かどうかを確認するのには、[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91db9-126">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a><span data-ttu-id="91db9-127">EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定する</span><span class="sxs-lookup"><span data-stu-id="91db9-127">Determine the GUID of the public folder mailbox by using the EWS Managed API</span></span>
<span data-ttu-id="91db9-128"><a name="bk_determineguidewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="91db9-128"></span></span>

<span data-ttu-id="91db9-129">パブリック フォルダー コンテンツ メールボックスの GUID を特定するには、次の動作を実行する以下のコード例を使用します。 </span><span class="sxs-lookup"><span data-stu-id="91db9-129">To determine the GUID of the public folder content mailbox, use the following code example, which does the following:</span></span> 
  
- <span data-ttu-id="91db9-130">[パブリック フォルダー階層構造のルーティングの要求](how-to-route-public-folder-hierarchy-requests.md)によって取得した**X AnchorMailbox**と**X PublicFolderInformation**のヘッダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="91db9-130">Uses the **X-AnchorMailbox** and **X-PublicFolderInformation** headers you retrieved by [routing public folder hierarchy requests](how-to-route-public-folder-hierarchy-requests.md).</span></span>
    
- <span data-ttu-id="91db9-131">EWS のマネージ API の[FindFolders](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)メソッドを呼び出すし、 **PR_REPLICA_LIST** (0x66980102) のプロパティが要求されています</span><span class="sxs-lookup"><span data-stu-id="91db9-131">Calls the EWS Managed API [FindFolders](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method, and includes a request for the **PR_REPLICA_LIST** (0x66980102) property</span></span> 
    
<span data-ttu-id="91db9-132">**PR_REPLICA_LIST**値は、メールボックス フォルダーの内容を持つパブリック フォルダーのメールボックスの GUID を指定します。</span><span class="sxs-lookup"><span data-stu-id="91db9-132">The **PR_REPLICA_LIST** value identifies the mailbox GUID of the public folder mailbox that has the content for the folder.</span></span> <span data-ttu-id="91db9-133">**PR_REPLICA_LIST**プロパティは、バイト配列が、このシナリオでは、GUID としてキャストします。</span><span class="sxs-lookup"><span data-stu-id="91db9-133">The **PR_REPLICA_LIST** property is a byte array, but is cast as a GUID for this scenario.</span></span> <span data-ttu-id="91db9-134">GUID とドメイン名は、自動検出を呼び出す対象となるアドレスをフォームに連結されます。</span><span class="sxs-lookup"><span data-stu-id="91db9-134">The GUID and the domain name are concatenated to form the address on which to call Autodiscover.</span></span> 
  
<span data-ttu-id="91db9-135">この例では、 `service` 、 [ExchangeService](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)のオブジェクト、メールボックス ユーザーは、`PFHAnchorHeader`と`PFHMailboxHeader` **X AnchorMailbox**と**X PublicFolderMailbox**のヘッダーの値は、ドメインで使用するドメイン名とは、テナント。</span><span class="sxs-lookup"><span data-stu-id="91db9-135">This example assumes that  `service` is the [ExchangeService](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox user,  `PFHAnchorHeader` and  `PFHMailboxHeader` are the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers, and domain is the domain name used by the tenant.</span></span> 
  
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

<span data-ttu-id="91db9-136">"要求が失敗しましたエラーが発生する場合。</span><span class="sxs-lookup"><span data-stu-id="91db9-136">If you received the error "The request failed.</span></span> <span data-ttu-id="91db9-137">基になる接続が閉じられました: SSL と TLS のセキュリティで保護されたチャネルに対する信頼関係を確立できませんでした」、[検証のコールバック メソッドへの呼び出しを追加](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="91db9-137">The underlying connection was closed: Could not establish trust relationship for the SSL/TLS secure channel", you'll need to [add a call to a validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> <span data-ttu-id="91db9-138">コードの例では、プレース ホルダーとそのメソッドのコメントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="91db9-138">A placeholder and comment for that method is included in the code example.</span></span>
  
<span data-ttu-id="91db9-139">メールボックス GUID が同じパブリック フォルダーのルートの下のすべてのパブリック フォルダーの場合は、例は、[自動検出を呼び出すこと](#bk_makeautodrequest)をコンソールに出力するときと、戻り値として使用するアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="91db9-139">If the mailbox GUID is the same for all the public folders under the public folder root, the example indicates the address to use when [calling Autodiscover](#bk_makeautodrequest) in the console output and as the return value.</span></span> <span data-ttu-id="91db9-140">メールボックス GUID は、同じパブリック フォルダーのルートの下のすべてのパブリック フォルダーではありません、場合[自動検出要求を作成](#bk_makeautodrequest)するのにはコンテンツ要求内のフォルダーに関連付けられているアドレスにします。</span><span class="sxs-lookup"><span data-stu-id="91db9-140">If the mailbox GUID is not the same for all public folders under the public folder root, you need to [Make an Autodiscover request](#bk_makeautodrequest) on the address associated with the folder in your content request.</span></span> 
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a><span data-ttu-id="91db9-141">EWS を使用してパブリック フォルダー メールボックスの GUID を特定する</span><span class="sxs-lookup"><span data-stu-id="91db9-141">Determine the GUID of the public folder mailbox by using EWS</span></span>
<span data-ttu-id="91db9-142"><a name="bk_determineguidews"> </a></span><span class="sxs-lookup"><span data-stu-id="91db9-142"></span></span>

<span data-ttu-id="91db9-143">次のコード例は、EWS [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)操作を使用して**PR_REPLICA_LIST** (0x66980102) プロパティの値を取得する方法です。</span><span class="sxs-lookup"><span data-stu-id="91db9-143">The following code example shows how retrieve the value of the **PR_REPLICA_LIST** (0x66980102) property by using the EWS [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="91db9-144">[ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)要素の**PropertyTag**属性は、 **PR_REPLICA_LIST**プロパティの 10 進値 (26264) に設定されてし、**バイナリ**を**登録するとき**の属性を設定します。</span><span class="sxs-lookup"><span data-stu-id="91db9-144">For the [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, the **PropertyTag** attribute is set to the decimal value (26264) of the **PR_REPLICA_LIST** property, and the **PropertyType** attribute is set to **Binary**.</span></span>
  
<span data-ttu-id="91db9-145">EWS のマネージ API は、 [EWS のマネージ API を使用してパブリック フォルダーのメールボックスの GUID を確認](#bk_determineguidewsma)するのには**FindFolders**メソッドを使用する場合を送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="91db9-145">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [determine the GUID of the public folder mailbox by using the EWS Managed API](#bk_determineguidewsma).</span></span>
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="91db9-146">サーバーは、 **PR_REPLICA_LIST**の拡張プロパティの値を含む[FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx)メッセージの**FindFolder**要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="91db9-146">The server responds to the **FindFolder** request with a [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes the value of the **PR_REPLICA_LIST** extended property.</span></span> <span data-ttu-id="91db9-147">ベース 64 の文字列形式として EWS の応答のプロパティの値が表示されるノートには、バイト配列がエンコードされています。</span><span class="sxs-lookup"><span data-stu-id="91db9-147">Note that the value of the property appears on the EWS response as the string format of a base-64 encoded byte array.</span></span> <span data-ttu-id="91db9-148">読みやすさのいくつかの応答ヘッダーの値に短縮されます。</span><span class="sxs-lookup"><span data-stu-id="91db9-148">Some header values in the response are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="91db9-149">XML、MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA で返される**PR_REPLICA_LIST**の値を使用するのには = =、メールボックス GUID を特定するには、値の値を変換する方法と同様の形式で GUID に変換する必要があります、[EWS のマネージ API のコード例](#bk_determineguidewsma)です。</span><span class="sxs-lookup"><span data-stu-id="91db9-149">In order to use the value of the **PR_REPLICA_LIST** returned in the XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, to determine the mailbox GUID, the value must be converted into a GUID in a format similar to how the value is converted in the [EWS Managed API code example](#bk_determineguidewsma).</span></span> <span data-ttu-id="91db9-150">GUID は、[自動検出要求](#bk_makeautodrequest)に含まれている SMTP アドレスを作成するドメイン名とし、連結されます。</span><span class="sxs-lookup"><span data-stu-id="91db9-150">The GUID is then concatenated with the domain name to create an SMTP address, which is included in the [Autodiscover request](#bk_makeautodrequest).</span></span>
  
## <a name="make-an-autodiscover-request"></a><span data-ttu-id="91db9-151">自動検出要求を作成する</span><span class="sxs-lookup"><span data-stu-id="91db9-151">Make an Autodiscover request</span></span>
<span data-ttu-id="91db9-152"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="91db9-152"></span></span>

<span data-ttu-id="91db9-153">によって返されるアドレスを使用して、`GetMailboxGuidAddress`自動検出を呼び出すメソッドです。</span><span class="sxs-lookup"><span data-stu-id="91db9-153">Use the address returned by the  `GetMailboxGuidAddress` method to call Autodiscover.</span></span> <span data-ttu-id="91db9-154">使用することをお勧め、 [Exchange 2013: 自動検出でユーザー設定を取得する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)の自動検出プロセスを合理化するために自動検出サービスを呼び出すためのコード サンプルです。</span><span class="sxs-lookup"><span data-stu-id="91db9-154">We recommend that you use the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="91db9-155">このコード サンプルでは、次の表に記載されているコマンドライン引数を使用して、メールボックス GUID に関連付けられている[AutoDiscoverSMTPAddress](http://msdn.microsoft.com/ja-jp/library/office/dn750991%28v=exchg.150%29.aspx)の値を取得するのには POX の自動検出サービスを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="91db9-155">This code sample uses the command-line arguments listed in the following table to call the POX Autodiscover service to retrieve the [AutoDiscoverSMTPAddress](http://msdn.microsoft.com/ja-jp/library/office/dn750991%28v=exchg.150%29.aspx) value associated with the mailbox GUID.</span></span> 
  
|<span data-ttu-id="91db9-156">**引数**</span><span class="sxs-lookup"><span data-stu-id="91db9-156">**Argument**</span></span>|<span data-ttu-id="91db9-157">**説明**</span><span class="sxs-lookup"><span data-stu-id="91db9-157">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91db9-158">emailAddress</span><span class="sxs-lookup"><span data-stu-id="91db9-158">emailAddress</span></span>  <br/> |<span data-ttu-id="91db9-159">によって返されるアドレス、`GetMailboxGuidAddress`メソッドで[パブリック フォルダーのメールボックスの GUID を指定](http://msdn.microsoft.com/library/bk_determineguidewsma.aspx)します。</span><span class="sxs-lookup"><span data-stu-id="91db9-159">The address returned by the  `GetMailboxGuidAddress` method in [Determine the GUID of the public folder mailbox](http://msdn.microsoft.com/library/bk_determineguidewsma.aspx).</span></span>  <br/> |
|<span data-ttu-id="91db9-160">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="91db9-160">-skipSOAP</span></span>  <br/> |<span data-ttu-id="91db9-161">POX 自動検出要求が必要であることを示します。</span><span class="sxs-lookup"><span data-stu-id="91db9-161">Indicates that POX Autodiscover requests are required.</span></span>  <br/> |
|<span data-ttu-id="91db9-162">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="91db9-162">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="91db9-p112">認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="91db9-p112">The mailbox user's email address, which is used for authentication. You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="91db9-165">たとえば、コマンドラインの引数の場合は、次のようになります。</span><span class="sxs-lookup"><span data-stu-id="91db9-165">For example, the command-line arguments should look like this:</span></span>
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="91db9-166">`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` 、 **GetMailboxGuidAddress**メソッドによって返されるアドレスと`sonyaf@contoso.com`は、メールボックス ユーザーです。</span><span class="sxs-lookup"><span data-stu-id="91db9-166">Where `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` is the address returned by the **GetMailboxGuidAddress** method, and `sonyaf@contoso.com` is the mailbox user.</span></span> 
  
<span data-ttu-id="91db9-167">実行すると、 **Exchange 2013: 自動検出とユーザー設定を取得する**サンプルでは、最後の自動検出応答する必要がありますが成功してメールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="91db9-167">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="91db9-168">**AutoDiscoverSMTPAddress**ユーザーは、ローカルで設定を保存するとを使用する次の手順でします。</span><span class="sxs-lookup"><span data-stu-id="91db9-168">Save the **AutoDiscoverSMTPAddress** user setting locally, as you'll use that in the next step.</span></span> 
  
<span data-ttu-id="91db9-169">またはを使用したくない場合**Exchange 2013: 自動検出とユーザー設定を取得する**サンプルでは、 **AutoDiscoverSMTPAddress**のユーザーによって[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)に設定して、次に送信を取得できますPOX 正常な応答を受信するまでは、各 URL に要求を自動検出します。</span><span class="sxs-lookup"><span data-stu-id="91db9-169">Alternatively, if you do not want to use **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **AutoDiscoverSMTPAddress** user setting by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="91db9-170">自動検出プロセスの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)、[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)、および[ユーザー設定の自動検出を使用して Exchange からの取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91db9-170">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="91db9-171">X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する</span><span class="sxs-lookup"><span data-stu-id="91db9-171">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="91db9-172"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="91db9-172"></span></span>

<span data-ttu-id="91db9-173">取得には[、自動検出要求を行う](#bk_makeautodrequest)には、 **AutoDiscoverSMTPAddress**の値を使用して、パブリック フォルダーのコンテンツ要求に**X AnchorMailbox** **X PublicFolderMailbox**のヘッダーの値を設定します。</span><span class="sxs-lookup"><span data-stu-id="91db9-173">Using the value for the **AutoDiscoverSMTPAddress** acquired in [Make an Autodiscover request](#bk_makeautodrequest), set the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="91db9-174">たとえば、NewPublicFolder@contoso.com の AutoDiscoverSMTPAddress が指定されている場合は、以下のメソッドの呼び出しまたは操作を行うときに、次のヘッダーを含めます。</span><span class="sxs-lookup"><span data-stu-id="91db9-174">For example, given an AutoDiscoverSMTPAddress of NewPublicFolder@contoso.com, include the following headers when making calls to the following methods or operations.</span></span>
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

<span data-ttu-id="91db9-175">**X AncorMailbox と X-パブリック フォルダーのヘッダーを必要とするパブリック フォルダーの呼び出し**</span><span class="sxs-lookup"><span data-stu-id="91db9-175">**Public folder calls that require the X-AncorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="91db9-176">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="91db9-176">**EWS Managed API methods**</span></span>|<span data-ttu-id="91db9-177">**EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="91db9-177">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91db9-178">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="91db9-178">Item.Bind</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-179">Item.Update</span><span class="sxs-lookup"><span data-stu-id="91db9-179">Item.Update</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-180">Item.Copy</span><span class="sxs-lookup"><span data-stu-id="91db9-180">Item.Copy</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-181">Item.Move</span><span class="sxs-lookup"><span data-stu-id="91db9-181">Item.Move</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-182">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="91db9-182">Item.Delete</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-183">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="91db9-183">Folder.Bind</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="91db9-184">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="91db9-184">Folder.FindItems</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="91db9-185">CreateItem</span><span class="sxs-lookup"><span data-stu-id="91db9-185">CreateItem</span></span>](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-186">GetItem</span><span class="sxs-lookup"><span data-stu-id="91db9-186">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-187">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="91db9-187">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-188">CopyItem</span><span class="sxs-lookup"><span data-stu-id="91db9-188">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-189">MoveItem</span><span class="sxs-lookup"><span data-stu-id="91db9-189">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-190">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="91db9-190">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-191">GetFolder</span><span class="sxs-lookup"><span data-stu-id="91db9-191">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="91db9-192">FindItem</span><span class="sxs-lookup"><span data-stu-id="91db9-192">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="91db9-193">EWS のマネージ API を使用して、これらのヘッダーを追加するには、 [HttpHeaders.Add](http://msdn.microsoft.com/ja-jp/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx)メソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="91db9-193">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](http://msdn.microsoft.com/ja-jp/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

<span data-ttu-id="91db9-194">次のコードは、この資料の例で取得した値に設定し、 **X AnchorMailbox** **X PublicFolderMailbox**のヘッダーで[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="91db9-194">The following code shows a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="see-also"></a><span data-ttu-id="91db9-195">関連項目</span><span class="sxs-lookup"><span data-stu-id="91db9-195">See also</span></span>

- [<span data-ttu-id="91db9-196">Exchange での EWS を使用したパブリック フォルダー アクセス</span><span class="sxs-lookup"><span data-stu-id="91db9-196">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="91db9-197">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="91db9-197">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="91db9-198">自動検出エンドポイントの一覧を生成します。</span><span class="sxs-lookup"><span data-stu-id="91db9-198">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [<span data-ttu-id="91db9-199">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="91db9-199">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

