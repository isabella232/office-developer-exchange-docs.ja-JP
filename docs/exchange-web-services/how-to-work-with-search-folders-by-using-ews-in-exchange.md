---
title: Exchange で EWS を使用して検索フォルダーを操作する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Exchange で EWS マネージ API または EWS を使用して、検索フォルダーを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: e38ff50fcdb5e42cea3f4b2e25345375f84ae6eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759105"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="cab1b-103">Exchange で EWS を使用して検索フォルダーを操作する</span><span class="sxs-lookup"><span data-stu-id="cab1b-103">How to: Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="cab1b-104">Exchange で EWS マネージ API または EWS を使用して、検索フォルダーを作成、取得、更新、削除する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="cab1b-105">検索フォルダーとは、ユーザーのメールボックスにおける永続的で「常時使用可能」な検索機能のことです。</span><span class="sxs-lookup"><span data-stu-id="cab1b-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="cab1b-106">検索フォルダーは、通常のメールボックスのフォルダーと同様の外観で、同じように動作します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="cab1b-107">ただし、アイテムそのものが含まれるのではなく、フォルダーに設定されている検索基準と一致する、検索範囲内にあるすべてのフォルダーのアイテムの「仮想」コピーが入っています。</span><span class="sxs-lookup"><span data-stu-id="cab1b-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="cab1b-108">アプリケーションとエンドユーザーのどちらも検索フォルダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="cab1b-109">アプリケーションで、同じ検索を繰り返し実行する必要がありますか。</span><span class="sxs-lookup"><span data-stu-id="cab1b-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="cab1b-110">こうしたタスクに関して、検索フォルダーは優れたツールとなります。</span><span class="sxs-lookup"><span data-stu-id="cab1b-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="cab1b-111">ユーザーに対して、クライアントの検索フォルダーにアクセスして管理する機能だけを付与するということも可能です。</span><span class="sxs-lookup"><span data-stu-id="cab1b-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="cab1b-112">どのようなシナリオであっても、EWS マネージ API と EWS を使用して、アプリケーションが検索フォルダーと十分に対話するようにできます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>
  
<span data-ttu-id="cab1b-113">**表 1. 検索フォルダーを処理するための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="cab1b-113">**Table 1.  EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="cab1b-114">**目的…**</span><span class="sxs-lookup"><span data-stu-id="cab1b-114">**If you want to…**</span></span>|<span data-ttu-id="cab1b-115">**EWS マネージ API で使用するもの**</span><span class="sxs-lookup"><span data-stu-id="cab1b-115">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="cab1b-116">**EWS で使用するもの**</span><span class="sxs-lookup"><span data-stu-id="cab1b-116">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cab1b-117">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="cab1b-117">Create a search folder</span></span>  <br/> |[<span data-ttu-id="cab1b-118">SearchFolder.Save</span><span class="sxs-lookup"><span data-stu-id="cab1b-118">SearchFolder.Save</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="cab1b-119">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-119">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="cab1b-120">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="cab1b-120">Get a search folder</span></span>  <br/> |[<span data-ttu-id="cab1b-121">SearchFolder.Bind</span><span class="sxs-lookup"><span data-stu-id="cab1b-121">SearchFolder.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="cab1b-122">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-122">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="cab1b-123">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="cab1b-123">Update a search folder</span></span>  <br/> |[<span data-ttu-id="cab1b-124">SearchFolder.Update</span><span class="sxs-lookup"><span data-stu-id="cab1b-124">SearchFolder.Update</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="cab1b-125">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-125">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="cab1b-126">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="cab1b-126">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="cab1b-127">SearchFolder.Delete</span><span class="sxs-lookup"><span data-stu-id="cab1b-127">SearchFolder.Delete</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="cab1b-128">DeleteFolder 操作 </span><span class="sxs-lookup"><span data-stu-id="cab1b-128">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="cab1b-129">検索フォルダーを操作するために把握しておくべき主要な概念</span><span class="sxs-lookup"><span data-stu-id="cab1b-129">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="cab1b-130"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-130"></span></span>

<span data-ttu-id="cab1b-131">検索フォルダーを操作する前に、検索フィルターのしくみについて理解しておきます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-131">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="cab1b-132">検索フォルダーは、検索フィルターに基づいて条件を表現します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-132">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="cab1b-133">検索フォルダー用の検索フィルターは、[検索操作用の検索フィルター](how-to-use-search-filters-with-ews-in-exchange.md)と同じように構成します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-133">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="cab1b-134">EWS マネージ API を使用して検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="cab1b-134">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="cab1b-135"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-135"></span></span>

<span data-ttu-id="cab1b-136">基本的には、EWS マネージ API を使用して検索フォルダーを作成する方法は、通常のフォルダーを作成する方法と同じです。</span><span class="sxs-lookup"><span data-stu-id="cab1b-136">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="cab1b-137">ただし、[Folder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)を使用するのではなく、[SearchFolder クラス](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)を使用し、[SearchParameters プロパティ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx)を設定して検索条件を構成します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-137">However, instead of using the [Folder class](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="cab1b-p104">次の例では、ユーザーの上司である sadie@contoso.com によって送信された、受信トレイとそのサブフォルダーにあるすべてのメッセージを検索する検索フォルダーを作成します。このフォルダーは、ユーザーのメールボックス内に [検索フォルダー] フォルダーの子として作成されます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-p104">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com. The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="cab1b-140">ユーザーのメールボックス内の任意のフォルダーの子として検索フォルダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-140">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="cab1b-141">ただし、新しく作成したフォルダーを Outlook の [検索フォルダー] の下に表示する場合は、[検索フォルダー] の既知のフォルダーの下に作成します。そのためには [WellKnownFolderName 列挙体](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)の **SearchFolders** 値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-141">You can create a search folder as a child of any folder in the user's mailbox. However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumerationhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="cab1b-142">この例では、**ExchangeService** オブジェクトは [Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) プロパティと [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) プロパティの有効な値で初期化されているものとします。</span><span class="sxs-lookup"><span data-stu-id="cab1b-142">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="cab1b-143">EWS を使用して検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="cab1b-143">Create a search folder by using EWS</span></span>
<span data-ttu-id="cab1b-144"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-144"></span></span>

<span data-ttu-id="cab1b-145">EWS を使用する場合、[CreateFolder 操作](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) に [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素を設定して、検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-145">If you are using EWS, use the [CreateFolder operation](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="cab1b-146">次の要求例では、ユーザーの上司である sadie@contoso.com によって送信された、受信トレイとそのサブフォルダーにあるすべてのメッセージを検索するための検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-146">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com. The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span> <span data-ttu-id="cab1b-147">このフォルダーは、ユーザーのメールボックス内の [検索フォルダー] フォルダーに作成されます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-147">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cab1b-148">ユーザーのメールボックス内の任意のフォルダーの子として検索フォルダーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-148">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="cab1b-149">ただし、新しく作成したフォルダーを Outlook の [検索フォルダー] の下に表示する場合には、[検索フォルダー] の既知のフォルダーの下に作成します。そのためには [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 要素の **Id** 属性に **searchfolders** 値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-149">You can create a search folder as a child of any folder in the user's mailbox. However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="cab1b-150">サーバーは、[CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cab1b-150">The server responds with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="cab1b-151">EWS マネージ API を使用して検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="cab1b-151">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="cab1b-152"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-152"></span></span>

<span data-ttu-id="cab1b-153">[ExchangeService.FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して、検索フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-153">Use the [ExchangeService.FindFolders](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="cab1b-154">ただし、結果に検索フォルダーだけを含めることはできません。結果を処理するときにこの点を覚えておくことができます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-154">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="cab1b-155">[SearchFolder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) メソッドを使用して、検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-155">Use the [SearchFolder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="cab1b-p109">次の例では、[検索フォルダー] フォルダーの最初の 10 フォルダーを検索します。それぞれが検索フォルダーかどうかを判別し、検索フォルダーであれば取得して、検索対象のフォルダー数を表示します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-p109">The following example finds the first 10 folders in the Search Folders folder. It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
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

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="cab1b-158">EWS を使用して検索フォルダーを取得する</span><span class="sxs-lookup"><span data-stu-id="cab1b-158">Get a search folder by using EWS</span></span>
<span data-ttu-id="cab1b-159"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-159"></span></span>

<span data-ttu-id="cab1b-160">EWS を使用する場合、[FindFolder 操作](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)を使用して検索フォルダーを検索し、[GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)で検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-160">If you're using EWS, use the [FindFolder operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="cab1b-161">検索フォルダーの正常な **GetFolder** 応答には、[SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cab1b-161">A successful **GetFolder** response for a search folder will contain a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="cab1b-162">次の要求例は、[検索フォルダー] フォルダーの最初の 10 フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-162">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="cab1b-163">サーバーは、1 つの検索フォルダーを示す次の応答を返します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-163">The server returns the following response, which shows one search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="cab1b-164">次の要求例では、検索フォルダーを取得する **GetFolder** 操作要求の先ほどの応答に含まれている [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 要素の値を使用します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-164">The following example of a request uses the value of the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="cab1b-165">サーバーは、以下の応答を、検索フォルダーのファースト クラスのプロパティすべてと一緒に返します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-165">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="cab1b-166">EWS マネージ API を使用して検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="cab1b-166">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="cab1b-167"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-167"></span></span>

<span data-ttu-id="cab1b-168">[Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS マネージ API メソッドを **SearchFolder** オブジェクトに対して使用し、検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-168">Use the [Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="cab1b-169">次の例は、「From Manager」という表示名の検索フォルダーの検索条件を更新します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-169">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
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

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="cab1b-170">EWS を使用して検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="cab1b-170">Update a search folder by using EWS</span></span>
<span data-ttu-id="cab1b-171"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-171"></span></span>

<span data-ttu-id="cab1b-172">EWS を使用する場合、[UpdateFolder 操作](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)に [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) 要素を設定して、検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-172">If you’re using EWS, use the [UpdateFolder operation](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](http://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder. The following request example updates the search criteria on the "From Manager" search folder.</span></span> <span data-ttu-id="cab1b-173">次の要求例は、「From Manager」という検索フォルダーの検索条件を更新します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-173">If you’re using EWS, use the UpdateFolder operation with a SearchFolder element to update a search folder. The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="cab1b-174">サーバーは、[UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cab1b-174">The server responds with an [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="cab1b-175">EWS マネージ API を使用して検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="cab1b-175">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="cab1b-176"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-176"></span></span>

<span data-ttu-id="cab1b-177">[Folder.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS マネージ API メソッドを **SearchFolder** オブジェクトに対して使用し、検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-177">Use the [Folder.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="cab1b-178">次の例は、「From Manager」という表示名の検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-178">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="cab1b-179">削除されたフォルダーは、[削除済みアイテム] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-179">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
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

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="cab1b-180">EWS を使用して検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="cab1b-180">Delete a search folder by using EWS</span></span>
<span data-ttu-id="cab1b-181"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="cab1b-181"></span></span>

<span data-ttu-id="cab1b-182">EWS を使用する場合、[DeleteFolder 操作](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)を使用して、検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-182">If you're using EWS, use the [DeleteFolder operation](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="cab1b-183">次の例は、検索フォルダーを削除し、[削除済みアイテム] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="cab1b-183">If you’re using EWS, use the DeleteFolder operation to delete a search folder. The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="cab1b-184">サーバーは、[DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) メッセージで応答します。このメッセージには、成功したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cab1b-184">The server responds with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cab1b-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="cab1b-185">See also</span></span>


- [<span data-ttu-id="cab1b-186">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="cab1b-186">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="cab1b-187">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="cab1b-187">How to: Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)
    
- [<span data-ttu-id="cab1b-188">SearchFolder クラス</span><span class="sxs-lookup"><span data-stu-id="cab1b-188">SearchFolder class</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="cab1b-189">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-189">CreateFolder operation</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)
    
- [<span data-ttu-id="cab1b-190">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-190">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="cab1b-191">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-191">GetFolder operation</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    
- [<span data-ttu-id="cab1b-192">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cab1b-192">UpdateFolder operation</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)
    
- [<span data-ttu-id="cab1b-193">DeleteFolder 操作 </span><span class="sxs-lookup"><span data-stu-id="cab1b-193">DeleteFolder operation</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

