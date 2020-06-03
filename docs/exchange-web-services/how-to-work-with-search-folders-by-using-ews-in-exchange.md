---
title: Exchange で EWS を使用して検索フォルダーを操作する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Exchange で EWS マネージ API または EWS を使用して、検索フォルダーを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: 880c14bc99c4f6c674d4f7566036c4b8f5f19e55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456368"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="62187-103">Exchange で EWS を使用して検索フォルダーを操作する</span><span class="sxs-lookup"><span data-stu-id="62187-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="62187-104">Exchange で EWS マネージ API または EWS を使用して、検索フォルダーを作成、取得、更新、削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="62187-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="62187-105">検索フォルダーとは、ユーザーのメールボックスにおける永続的で「常時使用可能」な検索機能のことです。</span><span class="sxs-lookup"><span data-stu-id="62187-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="62187-106">検索フォルダーは、通常のメールボックスのフォルダーと同様の外観で、同じように動作します。</span><span class="sxs-lookup"><span data-stu-id="62187-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="62187-107">ただし、アイテムそのものが含まれるのではなく、フォルダーに設定されている検索基準と一致する、検索範囲内にあるすべてのフォルダーのアイテムの「仮想」コピーが入っています。</span><span class="sxs-lookup"><span data-stu-id="62187-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="62187-108">アプリケーションとエンドユーザーのどちらも検索フォルダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="62187-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="62187-109">アプリケーションで、同じ検索を繰り返し実行する必要がありますか。</span><span class="sxs-lookup"><span data-stu-id="62187-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="62187-110">こうしたタスクに関して、検索フォルダーは優れたツールとなります。</span><span class="sxs-lookup"><span data-stu-id="62187-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="62187-111">ユーザーに対して、クライアントの検索フォルダーにアクセスして管理する機能だけを付与するということも可能です。</span><span class="sxs-lookup"><span data-stu-id="62187-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="62187-112">どのようなシナリオであっても、EWS マネージ API と EWS を使用して、アプリケーションが検索フォルダーと十分に対話するようにできます。</span><span class="sxs-lookup"><span data-stu-id="62187-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>

> [!NOTE] 
> <span data-ttu-id="62187-113">この記事は、Outlook をオンラインモードで使用している場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="62187-113">This article applies only when using Outlook in online mode.</span></span> <span data-ttu-id="62187-114">検索フォルダーは同期されません。そのため、オンラインモードで作成された検索フォルダーは、キャッシュモードでは表示されません。</span><span class="sxs-lookup"><span data-stu-id="62187-114">Search folders do not sync; therefore, search folders created in online mode will not appear in cached mode.</span></span>
  
<span data-ttu-id="62187-115">**表 1. 検索フォルダーを処理するための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="62187-115">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="62187-116">目的…</span><span class="sxs-lookup"><span data-stu-id="62187-116">If you want to…</span></span>|<span data-ttu-id="62187-117">EWS マネージ API で使用するもの</span><span class="sxs-lookup"><span data-stu-id="62187-117">In the EWS Managed API, use…</span></span>|<span data-ttu-id="62187-118">EWS で使用するもの</span><span class="sxs-lookup"><span data-stu-id="62187-118">In EWS, use…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="62187-119">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="62187-119">Create a search folder</span></span>  <br/> |[<span data-ttu-id="62187-120">SearchFolder.Save</span><span class="sxs-lookup"><span data-stu-id="62187-120">SearchFolder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="62187-121">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-121">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="62187-122">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="62187-122">Get a search folder</span></span>  <br/> |[<span data-ttu-id="62187-123">SearchFolder.Bind</span><span class="sxs-lookup"><span data-stu-id="62187-123">SearchFolder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="62187-124">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-124">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="62187-125">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="62187-125">Update a search folder</span></span>  <br/> |[<span data-ttu-id="62187-126">SearchFolder.Update</span><span class="sxs-lookup"><span data-stu-id="62187-126">SearchFolder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="62187-127">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-127">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="62187-128">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="62187-128">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="62187-129">SearchFolder.Delete</span><span class="sxs-lookup"><span data-stu-id="62187-129">SearchFolder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="62187-130">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-130">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="62187-131">検索フォルダーを操作するために把握しておくべき主要な概念</span><span class="sxs-lookup"><span data-stu-id="62187-131">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="62187-132"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-132"><a name="bk_CoreConcepts"> </a></span></span>

<span data-ttu-id="62187-133">検索フォルダーを操作する前に、検索フィルターのしくみについて理解しておきます。</span><span class="sxs-lookup"><span data-stu-id="62187-133">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="62187-134">検索フォルダーは、検索フィルターに基づいて条件を表現します。</span><span class="sxs-lookup"><span data-stu-id="62187-134">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="62187-135">検索フォルダー用の検索フィルターは、[検索操作用の検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)と同じように構成します。</span><span class="sxs-lookup"><span data-stu-id="62187-135">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="62187-136">EWS マネージ API を使用して検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="62187-136">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="62187-137"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-137"><a name="bk_CreateEWSMA"> </a></span></span>

<span data-ttu-id="62187-138">基本的には、EWS マネージ API を使用して検索フォルダーを作成する方法は、通常のフォルダーを作成する方法と同じです。</span><span class="sxs-lookup"><span data-stu-id="62187-138">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="62187-139">ただし、[Folder クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)を使用するのではなく、[SearchFolder クラス](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)を使用し、[SearchParameters プロパティ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx)を設定して検索条件を構成します。</span><span class="sxs-lookup"><span data-stu-id="62187-139">However, instead of using the [Folder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="62187-p105">次の例では、ユーザーの上司である sadie@contoso.com によって送信された、受信トレイとそのサブフォルダーにあるすべてのメッセージを検索する検索フォルダーを作成します。このフォルダーは、ユーザーのメールボックス内に [検索フォルダー] フォルダーの子として作成されます。</span><span class="sxs-lookup"><span data-stu-id="62187-p105">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com. The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="62187-142">ユーザーのメールボックス内の任意のフォルダーの子として検索フォルダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="62187-142">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="62187-143">ただし、新しく作成したフォルダーを Outlook の [検索フォルダー] の下に表示する場合は、[検索フォルダー] の既知のフォルダーの下に作成します。そのためには [WellKnownFolderName 列挙体](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)の **SearchFolders** 値を使用します。</span><span class="sxs-lookup"><span data-stu-id="62187-143">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="62187-144">この例では、**ExchangeService** オブジェクトは [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="62187-144">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void CreateSearchFolder(ExchangeService service)
{
    // Create the folder.
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "From Manager";
    // Create a search filter to express the criteria
    // for the folder.
    EmailAddress manager = new EmailAddress("sadie@contoso.com");
    SearchFilter.IsEqualTo fromManagerFilter =
        new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
    // Set the search filter.
    searchFolder.SearchParameters.SearchFilter = fromManagerFilter;
    // Set the folder to search.
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    // Set the search traversal. Deep will search all subfolders.
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    // Call Save to make the EWS call to create the folder.
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="62187-145">EWS を使用して検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="62187-145">Create a search folder by using EWS</span></span>
<span data-ttu-id="62187-146"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-146"><a name="bk_CreateEWS"> </a></span></span>

<span data-ttu-id="62187-147">EWS を使用する場合、[CreateFolder 操作](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) に [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素を設定して、検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="62187-147">If you are using EWS, use the [CreateFolder operation](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="62187-148">次の要求例では、ユーザーの上司である sadie@contoso.com によって送信された、受信トレイとそのサブフォルダーにあるすべてのメッセージを検索するための検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="62187-148">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="62187-149">このフォルダーは、ユーザーのメールボックス内の [検索フォルダー] フォルダーに作成されます。</span><span class="sxs-lookup"><span data-stu-id="62187-149">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="62187-150">ユーザーのメールボックス内の任意のフォルダーの子として検索フォルダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="62187-150">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="62187-151">ただし、新しく作成したフォルダーを Outlook の [検索フォルダー] の下に表示する場合には、[検索フォルダー] の既知のフォルダーの下に作成します。そのためには [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 要素の **Id** 属性に **searchfolders** 値を使用します。</span><span class="sxs-lookup"><span data-stu-id="62187-151">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderId>
      <m:Folders>
        <t:SearchFolder>
          <t:DisplayName>From Manager</t:DisplayName>
          <t:SearchParameters Traversal="Deep">
            <t:Restriction>
              <t:IsEqualTo>
                <t:FieldURI FieldURI="message:Sender" />
                <t:FieldURIOrConstant>
                  <t:Constant Value="sadie@contoso.com" />
                </t:FieldURIOrConstant>
              </t:IsEqualTo>
            </t:Restriction>
            <t:BaseFolderIds>
              <t:DistinguishedFolderId Id="inbox" />
            </t:BaseFolderIds>
          </t:SearchParameters>
        </t:SearchFolder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="62187-152">サーバーは、[CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="62187-152">The server responds with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="62187-153">EWS マネージ API を使用して検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="62187-153">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="62187-154"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-154"><a name="bk_RetrieveEWSMA"> </a></span></span>

<span data-ttu-id="62187-155">[ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して、検索フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="62187-155">Use the [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="62187-156">ただし、結果に検索フォルダーだけを含めることはできません。結果を処理するときにこの点を覚えておくことができます。</span><span class="sxs-lookup"><span data-stu-id="62187-156">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="62187-157">[SearchFolder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) メソッドを使用して、検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="62187-157">Use the [SearchFolder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="62187-p110">次の例では、[検索フォルダー] フォルダーの最初の 10 フォルダーを検索します。それぞれが検索フォルダーかどうかを判別し、検索フォルダーであれば取得して、検索対象のフォルダー数を表示します。</span><span class="sxs-lookup"><span data-stu-id="62187-p110">The following example finds the first 10 folders in the Search Folders folder. It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void GetSearchFolders(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You can't request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder)
            {
                Console.WriteLine("{0} is a search folder.", folder.DisplayName);
                // In order to access the SearchParameters property,
                // you have to bind to the folder. SearchParameters are not
                // returned in FindFolders results.
                SearchFolder searchFolder = SearchFolder.Bind(service, folder.Id);
                Console.WriteLine("Number of folders searched: {0}.",
                    searchFolder.SearchParameters.RootFolderIds.Count);
            }
            else
            {
                Console.WriteLine("{0} is NOT a search folder.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="62187-160">EWS を使用して検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="62187-160">Get a search folder by using EWS</span></span>
<span data-ttu-id="62187-161"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-161"><a name="bk_RetrieveEWS"> </a></span></span>

<span data-ttu-id="62187-162">EWS を使用する場合、[FindFolder 操作](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)を使用して検索フォルダーを検索し、[GetFolder 操作](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)で検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="62187-162">If you're using EWS, use the [FindFolder operation](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="62187-163">検索フォルダーの正常な **GetFolder** 応答には、[SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="62187-163">A successful **GetFolder** response for a search folder will contain a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="62187-164">次の要求例は、[検索フォルダー] フォルダーの最初の 10 フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="62187-164">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="62187-165">サーバーは、1 つの検索フォルダーを示す次の応答を返します。</span><span class="sxs-lookup"><span data-stu-id="62187-165">The server returns the following response, which shows one search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Folders>
              <t:SearchFolder>
                <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
                <t:DisplayName>From Manager</t:DisplayName>
              </t:SearchFolder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="62187-166">次の要求例では、検索フォルダーを取得する **GetFolder** 操作要求の先ほどの応答に含まれている [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 要素の値を使用します。</span><span class="sxs-lookup"><span data-stu-id="62187-166">The following example of a request uses the value of the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="62187-167">サーバーは、以下の応答を、検索フォルダーのファースト クラスのプロパティすべてと一緒に返します。</span><span class="sxs-lookup"><span data-stu-id="62187-167">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:SearchFolder>
              <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
              <t:ParentFolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>From Manager</t:DisplayName>
              <t:TotalCount>8</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:UnreadCount>0</t:UnreadCount>
              <t:SearchParameters Traversal="Deep">
                <t:Restriction>
                  <t:IsEqualTo>
                    <t:FieldURI FieldURI="message:Sender" />
                    <t:FieldURIOrConstant>
                      <t:Constant Value="/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=8d84a3f4cbb34d48838a3aecf99795c0-Sadie" />
                    </t:FieldURIOrConstant>
                  </t:IsEqualTo>
                </t:Restriction>
                <t:BaseFolderIds>
                  <t:FolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
                </t:BaseFolderIds>
              </t:SearchParameters>
            </t:SearchFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="62187-168">EWS マネージ API を使用して検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="62187-168">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="62187-169"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-169"><a name="bk_UpdateEWSMA"> </a></span></span>

<span data-ttu-id="62187-170">[Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS マネージ API メソッドを **SearchFolder** オブジェクトに対して使用し、検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="62187-170">Use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="62187-171">次の例は、「From Manager」という表示名の検索フォルダーの検索条件を更新します。</span><span class="sxs-lookup"><span data-stu-id="62187-171">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void UpdateSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                SearchFolder searchFolder = folder as SearchFolder;
                EmailAddress newManager = new EmailAddress("hope@contoso.com");
                SearchFilter.IsEqualTo newManagerFilter =
                    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, newManager);
                searchFolder.SearchParameters.SearchFilter = newManagerFilter;
                searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
                searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
                searchFolder.Update();
                Console.WriteLine("\"{0}\" folder updated.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="62187-172">EWS を使用して検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="62187-172">Update a search folder by using EWS</span></span>
<span data-ttu-id="62187-173"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-173"><a name="bk_UpdateEWS"> </a></span></span>

<span data-ttu-id="62187-174">EWS を使用する場合、[UpdateFolder 操作](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)に [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素を設定して、検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="62187-174">If you're using EWS, use the [UpdateFolder operation](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="62187-175">次の要求例は、「From Manager」という検索フォルダーの検索条件を更新します。</span><span class="sxs-lookup"><span data-stu-id="62187-175">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:SearchParameters" />
              <t:SearchFolder>
                <t:SearchParameters Traversal="Deep">
                  <t:Restriction>
                    <t:IsEqualTo>
                      <t:FieldURI FieldURI="message:Sender" />
                      <t:FieldURIOrConstant>
                        <t:Constant Value="hope@contoso.com" />
                      </t:FieldURIOrConstant>
                    </t:IsEqualTo>
                  </t:Restriction>
                  <t:BaseFolderIds>
                    <t:DistinguishedFolderId Id="inbox" />
                  </t:BaseFolderIds>
                </t:SearchParameters>
              </t:SearchFolder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="62187-176">サーバーは、[UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="62187-176">The server responds with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="62187-177">EWS マネージ API を使用して検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="62187-177">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="62187-178"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-178"><a name="bk_DeleteEWSMA"> </a></span></span>

<span data-ttu-id="62187-179">[Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS マネージ API メソッドを **SearchFolder** オブジェクトに対して使用し、検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="62187-179">Use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="62187-180">次の例は、「From Manager」という表示名の検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="62187-180">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="62187-181">削除されたフォルダーは、[削除済みアイテム] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="62187-181">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void DeleteSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                folder.Delete(DeleteMode.MoveToDeletedItems);
                Console.WriteLine("\"{0}\" folder deleted.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="62187-182">EWS を使用して検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="62187-182">Delete a search folder by using EWS</span></span>
<span data-ttu-id="62187-183"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="62187-183"><a name="bk_DeleteEWS"> </a></span></span>

<span data-ttu-id="62187-184">EWS を使用する場合、[DeleteFolder 操作](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用して、検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="62187-184">If you're using EWS, use the [DeleteFolder operation](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="62187-185">次の例は、検索フォルダーを削除し、[削除済みアイテム] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="62187-185">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="MoveToDeletedItems">
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="62187-186">サーバーは、[DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="62187-186">The server responds with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="62187-187">関連項目</span><span class="sxs-lookup"><span data-stu-id="62187-187">See also</span></span>

- [<span data-ttu-id="62187-188">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="62187-188">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)   
- [<span data-ttu-id="62187-189">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="62187-189">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="62187-190">SearchFolder クラス</span><span class="sxs-lookup"><span data-stu-id="62187-190">SearchFolder class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="62187-191">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-191">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)    
- [<span data-ttu-id="62187-192">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-192">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="62187-193">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-193">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)    
- [<span data-ttu-id="62187-194">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="62187-194">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)    
- [<span data-ttu-id="62187-195">DeleteFolder 操作 </span><span class="sxs-lookup"><span data-stu-id="62187-195">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

