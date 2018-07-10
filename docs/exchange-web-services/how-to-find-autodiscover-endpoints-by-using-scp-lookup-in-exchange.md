---
title: Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Active Directory ドメイン サービス (AD DS) での自動検出 SCP オブジェクトを検索し、Exchange の自動検出サービスで使用する自動検出エンドポイントの Url を探す場合に使用する方法を確認します。
ms.openlocfilehash: 59fd316d0aa0feea81b60c279040da018c51b47d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758943"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a><span data-ttu-id="13e84-103">Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。</span><span class="sxs-lookup"><span data-stu-id="13e84-103">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>

<span data-ttu-id="13e84-104">Active Directory ドメイン サービス (AD DS) での自動検出 SCP オブジェクトを検索し、Exchange の自動検出サービスで使用する自動検出エンドポイントの Url を探す場合に使用する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="13e84-104">Find out how to locate Autodiscover SCP objects in Active Directory Domain Services (AD DS) and use them to find Autodiscover endpoint URLs to use with the Exchange Autodiscover service.</span></span>
  
<span data-ttu-id="13e84-105">自動検出では、Exchange サーバー上のメールボックスに接続するために必要な情報を取得するために簡単です。</span><span class="sxs-lookup"><span data-stu-id="13e84-105">Autodiscover makes it easy to retrieve information that you need to connect to mailboxes on Exchange servers.</span></span> <span data-ttu-id="13e84-106">ただし、自動検出を使用するには、自動検出サーバーの設定を取得しているユーザーに適切なを検索する方法が必要です。</span><span class="sxs-lookup"><span data-stu-id="13e84-106">However, in order to use Autodiscover, you need a way to find Autodiscover servers that are appropriate for the user you're retrieving settings for.</span></span> <span data-ttu-id="13e84-107">AD DS 内のサービス接続ポイント (SCP) オブジェクトは、ドメインに参加しているクライアントが自動検出サーバーを検索する簡単な方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="13e84-107">Service connection point (SCP) objects in AD DS provide an easy way for domain-joined clients to look up Autodiscover servers.</span></span> 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a><span data-ttu-id="13e84-108">自動検出エンドポイントを検出できるようにセットアップする</span><span class="sxs-lookup"><span data-stu-id="13e84-108">Get set up to find Autodiscover endpoints</span></span>
<span data-ttu-id="13e84-109"><a name="bk_PreReqs"> </a></span><span class="sxs-lookup"><span data-stu-id="13e84-109"></span></span>

<span data-ttu-id="13e84-110">AD DS では、自動検出 SCP オブジェクトを探し、次にアクセスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="13e84-110">To locate Autodiscover SCP objects in AD DS, you need to have access to the following:</span></span>
  
- <span data-ttu-id="13e84-111">Exchange 2007 SP1 以降の Exchange オンプレミス バージョンを実行しているサーバー。</span><span class="sxs-lookup"><span data-stu-id="13e84-111">A server that is running a version of Exchange on-premises starting with Exchange 2007 SP1.</span></span>
    
- <span data-ttu-id="13e84-112">Exchange サーバーがインストールされているドメインに参加しているクライアント コンピューター。</span><span class="sxs-lookup"><span data-stu-id="13e84-112">A client computer that is joined to the domain that the Exchange server is installed in.</span></span>
    
- <span data-ttu-id="13e84-113">Exchange サーバーにメールボックスがあるユーザー アカウント。 </span><span class="sxs-lookup"><span data-stu-id="13e84-113">A user account that has a mailbox on the Exchange server.</span></span> 
    
<span data-ttu-id="13e84-114">また、作業を開始する前にする必要があります理解するいくつかの基本的な概念です。</span><span class="sxs-lookup"><span data-stu-id="13e84-114">Also, before you begin, you'll want to be familiar some basic concepts.</span></span> <span data-ttu-id="13e84-115">役に立つことがわかりますいくつかのリソースを次に示します。</span><span class="sxs-lookup"><span data-stu-id="13e84-115">The following are some resources that you'll find helpful.</span></span>
  
<span data-ttu-id="13e84-116">**表 1 です。SCP オブジェクトから自動検出エンドポイントを検索するための関連記事**</span><span class="sxs-lookup"><span data-stu-id="13e84-116">**Table 1. Related articles for finding Autodiscover endpoints from SCP objects**</span></span>

|<span data-ttu-id="13e84-117">**この記事を読む**</span><span class="sxs-lookup"><span data-stu-id="13e84-117">**Read this article**</span></span>|<span data-ttu-id="13e84-118">**について説明しています.**</span><span class="sxs-lookup"><span data-stu-id="13e84-118">**To learn about…**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13e84-119">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="13e84-119">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="13e84-120">自動検出サービスの動作方法。</span><span class="sxs-lookup"><span data-stu-id="13e84-120">How the Autodiscover service works.</span></span>  <br/> |
|[<span data-ttu-id="13e84-121">サービス接続ポイントの発行</span><span class="sxs-lookup"><span data-stu-id="13e84-121">Publishing with Service Connection Points</span></span>](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |<span data-ttu-id="13e84-122">SCP オブジェクトを使用してサービス固有のデータを発行する方法。</span><span class="sxs-lookup"><span data-stu-id="13e84-122">How SCP objects are used to publish service-specific data.</span></span>  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a><span data-ttu-id="13e84-123">AD DS 内の自動検出 SCP オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="13e84-123">Locate Autodiscover SCP objects in AD DS</span></span>
<span data-ttu-id="13e84-124"><a name="bk_LocateScpObjects"> </a></span><span class="sxs-lookup"><span data-stu-id="13e84-124"></span></span>

<span data-ttu-id="13e84-125">AD DS で公開されている自動検出エンドポイントを検索するための第一歩は、自動検出 SCP オブジェクトを検索します。</span><span class="sxs-lookup"><span data-stu-id="13e84-125">The first step toward finding Autodiscover endpoints published in AD DS is to locate the Autodiscover SCP objects.</span></span> <span data-ttu-id="13e84-126">Exchange では、自動検出の 2 種類の SCP オブジェクトを発行します。</span><span class="sxs-lookup"><span data-stu-id="13e84-126">Exchange publishes two types of SCP objects for Autodiscover:</span></span>
  
- <span data-ttu-id="13e84-127">**SCP ポインター** : ユーザーのドメインの自動検出 SCP オブジェクトの検索に使用する特定の LDAP サーバーをポイントするための情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="13e84-127">**SCP pointers** — These contain information that points to specific LDAP servers that should be used to locate Autodiscover SCP objects for the user's domain.</span></span> <span data-ttu-id="13e84-128">SCP ポインターには、次の GUID がスタンプされて: 67661d7F-8 個の FC 4-4fa7-BFAC-E1D7794C1F68 です。</span><span class="sxs-lookup"><span data-stu-id="13e84-128">SCP pointers are stamped with the following GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span></span> 
    
- <span data-ttu-id="13e84-129">**SCP Url**自動検出エンドポイントの Url が含まれます。</span><span class="sxs-lookup"><span data-stu-id="13e84-129">**SCP URLs** — These contain URLs for Autodiscover endpoints.</span></span> <span data-ttu-id="13e84-130">SCP Url には次の GUID を持つスタンプ: 77378F46-2 C 66-4aa9-A6A6-3E7A48B19596 です。</span><span class="sxs-lookup"><span data-stu-id="13e84-130">SCP URLs are stamped with the following GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span></span> 
    
### <a name="to-locate-autodiscover-scp-objects"></a><span data-ttu-id="13e84-131">自動検出 SCP オブジェクトを見つけるには</span><span class="sxs-lookup"><span data-stu-id="13e84-131">To locate Autodiscover SCP objects</span></span>

1. <span data-ttu-id="13e84-132">ルート ドメインの構成名前付けコンテキストへのパスを取得するのには AD DS の dse サービスのエントリの**configurationNamingContext**プロパティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="13e84-132">Read the **configurationNamingContext** property of the root DSE entry in AD DS to get the path to the configuration naming context for the domain.</span></span> <span data-ttu-id="13e84-133">[DirectoryEntry](http://msdn2.microsoft.com/ja-jp/library/z9cddzaa)クラス、または AD DS にアクセスできる他の任意の API を使用してこれを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="13e84-133">You can do this by using the [DirectoryEntry](http://msdn2.microsoft.com/ja-jp/library/z9cddzaa) class, or any other API that can acces AD DS.</span></span> 
    
2. <span data-ttu-id="13e84-134">構成名前付けコンテキストの SCP オブジェクトをいずれか、SCP ポインターの GUID を持つか、SCP URL に GUID**キーワード**のプロパティを検索します。</span><span class="sxs-lookup"><span data-stu-id="13e84-134">Search for SCP objects in the configuration naming context that have either the SCP pointer GUID or the SCP URL GUID in the **keywords** property.</span></span> 
    
3. <span data-ttu-id="13e84-135">SCP オブジェクトを SCP ポインターと同じエントリの [**キーワード**] プロパティを確認することでユーザーのドメインのスコープを検索したことを確認`"Domain=<domain>"`。</span><span class="sxs-lookup"><span data-stu-id="13e84-135">Check the SCP objects you found for an SCP pointer that is scoped to the user's domain by checking the **keywords** property for an entry equal to `"Domain=<domain>"`.</span></span> <span data-ttu-id="13e84-136">などのユーザーの電子メール アドレスが elvin@contoso.com の場合は、するを検索、SCP ポインターと同じである**キーワード**プロパティのエントリを`"Domain=contoso.com"`。</span><span class="sxs-lookup"><span data-stu-id="13e84-136">For example, if the user's email address is elvin@contoso.com, you would look for an SCP pointer with an entry in the **keywords** property that is equal to `"Domain=contoso.com"`.</span></span> <span data-ttu-id="13e84-137">一致する SCP ポインターがある場合 SCP オブジェクトのセットを破棄して、手順 1 のルート DSE のエントリに接続するサーバーとして、 **serviceBindingInformation**プロパティの値を使用して最初からやり直す。</span><span class="sxs-lookup"><span data-stu-id="13e84-137">If a matching SCP pointer is found, discard the set of SCP objects and start over at step 1 using the value of the **serviceBindingInformation** property as the server to connect to for the Root DSE entry.</span></span> 
    
4. <span data-ttu-id="13e84-138">SCP ポインターは任意のドメインのスコープを確認し、名前を付けて、 **serviceBindingInformation**プロパティの値「フォールバック」のサーバーでは、現在のサーバーは提供しませんいずれかの場合にユーザーのドメインを対象にした SCP ポインターがない場合は、結果です。</span><span class="sxs-lookup"><span data-stu-id="13e84-138">If you don't find any SCP pointers scoped to the user's domain, check for any SCP pointers that aren't scoped to any domain, and save the value of the **serviceBindingInformation** property as a "fallback" server, in case the current server doesn't give you any results.</span></span> 
    
5. <span data-ttu-id="13e84-139">対象ドメインをスコープとする SCP ポインターがまったく見つからなくなれば、次の手順に進めます。次の手順では、結果から自動検出エンドポイントの優先順位を付けた一覧を生成します。</span><span class="sxs-lookup"><span data-stu-id="13e84-139">If you didn't find any SCP pointers scoped to the domain, you're ready to move on to the next step: generating a prioritized list of Autodiscover endpoints from your results.</span></span>
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a><span data-ttu-id="13e84-140">自動検出エンドポイントの優先順位を付けた一覧を生成する</span><span class="sxs-lookup"><span data-stu-id="13e84-140">Generate a prioritized list of Autodiscover endpoints</span></span>
<span data-ttu-id="13e84-141"><a name="bk_GenerateList"> </a></span><span class="sxs-lookup"><span data-stu-id="13e84-141"></span></span>

<span data-ttu-id="13e84-142">見つけた一連の SCP オブジェクトを使用して、優先順位を付けた自動検出エンドポイント URL の一覧を生成できます。そのためには次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="13e84-142">You can generate a prioritized list of Autodiscover endpoint URLs, using the set of SCP objects that you located, by doing the following:</span></span>
  
1. <span data-ttu-id="13e84-143">クライアント コンピューターの Active Directory サイト名を取得します。</span><span class="sxs-lookup"><span data-stu-id="13e84-143">Get the Active Directory site name of the client computer.</span></span>
    
2. <span data-ttu-id="13e84-144">SCP オブジェクトを検出すると、一連の SCP URL ごとに**キーワード**のプロパティを確認し、次の規則に基づく URL に優先順位を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="13e84-144">Check the **keywords** property on each SCP URL in the set of SCP objects you found, and assign a priority to the URL based on the following rules:</span></span> 
    
  - <span data-ttu-id="13e84-145">**キーワード**プロパティに値が含まれているかどうか`"Site=<site name>"`、`<site name>`と等しいが、前の手順で取得したサイトのアクティブなディレクトリの名前は、URL 1 の優先順位を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="13e84-145">If the **keywords** property contains a value of `"Site=<site name>"`, where `<site name>` equals the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 1.</span></span> 
    
  - <span data-ttu-id="13e84-146">**Keywords**プロパティで始まる値を持つエントリが含まれていない場合は、 `"Site="`、2 の優先順位の URL を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="13e84-146">If the **keywords** property does not contain an entry with a value that starts with `"Site="`, assign the URL a priority of 2.</span></span> 
    
  - <span data-ttu-id="13e84-147">**キーワード**のプロパティに値が含まれているかどうか`"Site=<site name>`、`<site name>`はないと同じ、前の手順で取得する Active Directory サイトの名前を 3 の優先順位の URL を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="13e84-147">If the **keywords** property contains a value of `"Site=<site name>`, where `<site name>` does not equal the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 3.</span></span> 
    
## <a name="code-example-performing-an-scp-lookup"></a><span data-ttu-id="13e84-148">コード例:SCP 参照</span><span class="sxs-lookup"><span data-stu-id="13e84-148">Code example: Performing an SCP lookup</span></span>
<span data-ttu-id="13e84-149"><a name="bk_CodeExample"> </a></span><span class="sxs-lookup"><span data-stu-id="13e84-149"></span></span>

<span data-ttu-id="13e84-150">次のコード例では、自動検出 SCP オブジェクトを検索し、エンドポイントの自動検出の優先順位の一覧を生成する方法が表示されます。</span><span class="sxs-lookup"><span data-stu-id="13e84-150">In the following code example, you'll see how to locate Autodiscover SCP objects and generate a prioritized list of Autodiscover endpoints.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.DirectoryServices;
using System.DirectoryServices.ActiveDirectory;
namespace ScpLookup
{
    // This sample is for demonstration purposes only. Before you run this sample, make sure 
    // that the code meets the coding requirements of your organization. 
    class Program
    {
        static void Main(string[] args)
        {
            string domain = args[0];
            Console.WriteLine("Performing SCP lookup for {0}.", domain);
            List<string> scpUrls = GetScpUrls(null, domain);
            Console.WriteLine("\nOrdered List of Autodiscover endpoints:");
            foreach (string url in scpUrls)
            {
                Console.WriteLine("  {0}", url);
            }
            Console.WriteLine("SCP lookup done.");
        }
        // GUID for SCP URL keyword.
        private const string ScpUrlGuidString = @"77378F46-2C66-4aa9-A6A6-3E7A48B19596";
        // GUID for SCP pointer keyword.
        private const string ScpPtrGuidString = @"67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68";
        static List<string> GetScpUrls(string ldapServer, string domain)
        {
            // Create a new list to return.
            List<string> scpUrlList = new List<string>();
            string rootDSEPath = null;
            // If ldapServer is null/empty, use LDAP://RootDSE to
            // connect to Active Directory Domain Services (AD DS). Otherwise, use
            // LDAP://SERVERNAME/RootDSE to connect to a specific server.
            if (string.IsNullOrEmpty(ldapServer))
            {
                rootDSEPath = "LDAP://RootDSE";
            }
            else
            {
                rootDSEPath = ldapServer + "/RootDSE";
            }
            SearchResultCollection scpEntries = null;
            try
            {
                // Get the root directory entry.
                DirectoryEntry rootDSE = new DirectoryEntry(rootDSEPath);
                // Get the configuration path.
                string configPath = rootDSE.Properties["configurationNamingContext"].Value as string;
                // Get the configuration entry.
                DirectoryEntry configEntry = new DirectoryEntry("LDAP://" + configPath);
                // Create a search object for the configuration entry.
                DirectorySearcher configSearch = new DirectorySearcher(configEntry);
                // Set the search filter to find SCP URLs and SCP pointers.
                configSearch.Filter = "(&amp;(objectClass=serviceConnectionPoint)" +
                    "(|(keywords=" + ScpPtrGuidString + ")(keywords=" + ScpUrlGuidString + ")))";
                // Specify which properties you want to retrieve.
                configSearch.PropertiesToLoad.Add("keywords");
                configSearch.PropertiesToLoad.Add("serviceBindingInformation");
                scpEntries = configSearch.FindAll();
            }
            catch (Exception ex)
            {
                Console.WriteLine("SCP lookup failed with: ");
                Console.WriteLine(ex.ToString());
            }
            // If no SCP entries were found, then exit.
            if (scpEntries == null || scpEntries.Count <= 0)
            {
                Console.WriteLine("No SCP records found.");
                return null;
            }
            string fallBackLdapPath = null;
            // Check for SCP pointers.
            foreach (SearchResult scpEntry in scpEntries)
            {
                ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                if (CollectionContainsExactValue(entryKeywords, ScpPtrGuidString))
                {
                    string ptrLdapPath = scpEntry.Properties["serviceBindingInformation"][0] as string;
                    // Determine whether this pointer is scoped to the user's domain.
                    if (CollectionContainsExactValue(entryKeywords, "Domain=" + domain))
                    {
                        Console.WriteLine("Found SCP pointer for " + domain + " in " + scpEntry.Path);
                        // Restart SCP lookup with the server assigned for the domain.
                        Console.WriteLine("Restarting SCP lookup in " + ptrLdapPath);
                        return GetScpUrls(ptrLdapPath, domain);
                    }
                    else
                    {
                        // Save the first SCP pointer that is not scoped to a domain as a fallback
                        // in case you do not get any results from this server.
                        if (entryKeywords.Count == 1 &amp;&amp; string.IsNullOrEmpty(fallBackLdapPath))
                        {
                            fallBackLdapPath = ptrLdapPath;
                            Console.WriteLine("Saved fallback SCP pointer: " + fallBackLdapPath);
                        }
                    }
                }
            }
            string computerSiteName = null;
            try
            {
                // Get the name of the ActiveDirectorySite the computer
                // belongs to (if it belongs to one).
                ActiveDirectorySite site = ActiveDirectorySite.GetComputerSite();
                computerSiteName = site.Name;
                Console.WriteLine("Local computer in site: " + computerSiteName);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Unable to get computer site name.");
                Console.WriteLine(ex.ToString());
            }
            if (!string.IsNullOrEmpty(computerSiteName))
            {
                // Scan the search results for SCP URLs.
                // SCP URLs fit into three tiers:
                //   Priority 1: The URL is scoped to the computer's Active Directory site.
                //   Priority 2: The URL is not scoped to any Active Directory site.
                //   Priority 3: The URL is scoped to a different Active Directory site.
                // Temporary lists to hold priority 2 and 3 URLs.
                List<string> priorityTwoUrls = new List<string>();
                List<string> priorityThreeUrls = new List<string>();
                foreach (SearchResult scpEntry in scpEntries)
                {
                    ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                    // Check for SCP URLs.
                    if (CollectionContainsExactValue(entryKeywords, ScpUrlGuidString))
                    {
                        string scpUrlPath = scpEntry.Properties["adsPath"][0] as string;
                        Console.WriteLine("SCP URL found at {0}", scpUrlPath);
                        string scpUrl = scpEntry.Properties["serviceBindingInformation"][0] as string;
                        scpUrl = scpUrl.ToLower();
                        // Determine whether this entry is scoped to the computer's site.
                        if (CollectionContainsExactValue(entryKeywords, "Site=" + computerSiteName))
                        {
                            // Priority 1.
                            if (!scpUrlList.Contains(scpUrl.ToLower()))
                            {
                                Console.WriteLine("Adding priority 1 SCP URL: {0}", scpUrl.ToLower());
                                scpUrlList.Add(scpUrl);
                            }
                            else
                            {
                                Console.WriteLine("Priority 1 SCP URL already found: {0}", scpUrl);
                            }
                        }
                        else
                        {
                            // Determine whether this is a priority 2 or 3 URL.
                            if (CollectionContainsPrefixValue(entryKeywords, "Site="))
                            {
                                // Priority 3.
                                if (!priorityThreeUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 3 SCP URL: {0}", scpUrl);
                                    priorityThreeUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 3 SCP URL already found: {0}", scpUrl);
                                }
                            }
                            else
                            {
                                // Priority 2.
                                if (!priorityTwoUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 2 SCP URL: {0}", scpUrl);
                                    priorityTwoUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 2 SCP URL already found: {0}", scpUrl);
                                }
                            }
                        }
                    }
                }
                // Now add the priority 2 URLs into the main list.
                foreach (string priorityTwoUrl in priorityTwoUrls)
                {
                    // If the URL is already in the list as a priority 1, 
                    // don't add it again.
                    if (!scpUrlList.Contains(priorityTwoUrl))
                    {
                        scpUrlList.Add(priorityTwoUrl);
                    }
                }
                // Now add the priority 3 URLs into the main list.
                foreach (string priorityThreeUrl in priorityThreeUrls)
                {
                    // If the URL is already in the list as a priority 1
                    // or priority 2, don't add it again.
                    if (!scpUrlList.Contains(priorityThreeUrl))
                    {
                        scpUrlList.Add(priorityThreeUrl);
                    }
                }
                // If after all this, you still have no URLs in your list,
                // try the fallback SCP pointer, if you have one.
                if (scpUrlList.Count == 0 &amp;&amp; fallBackLdapPath != null)
                {
                    return GetScpUrls(fallBackLdapPath, domain);
                }
            }
            return scpUrlList;
        }
        private static bool CollectionContainsExactValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (string.Compare(value, entry, true) == 0)
                        return true;
                }
            }
            return false;
        }
        private static bool CollectionContainsPrefixValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (entry.StartsWith(value))
                        return true;
                }
            }
            return false;
        }
    }
}
```

## <a name="next-steps"></a><span data-ttu-id="13e84-151">次の手順</span><span class="sxs-lookup"><span data-stu-id="13e84-151">Next steps</span></span>
<span data-ttu-id="13e84-152"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="13e84-152"></span></span>

<span data-ttu-id="13e84-p108">自動検出プロセスの次の手順では、見つかった URL に対して自動検出要求を送信します。その際、優先順位 1 の URL、優先順位 2 の URL、最後に優先順位 3 の URL の順に送信します。自動検出要求を送信し、応答を処理する方法の詳細については、以下の資料を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13e84-p108">The next step in the Autodiscover process is to send Autodiscover requests to the URLs that you found, starting with priority 1 URLs, then priority 2 URLs, and finally priority 3 URLs. To learn more about how to send Autodiscover requests and handle responses, read the following articles:</span></span>
  
- [<span data-ttu-id="13e84-155">Exchange から自動検出を使用してユーザー設定を取得します。</span><span class="sxs-lookup"><span data-stu-id="13e84-155">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="13e84-156">自動検出のエラー メッセージの処理</span><span class="sxs-lookup"><span data-stu-id="13e84-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a><span data-ttu-id="13e84-157">関連項目</span><span class="sxs-lookup"><span data-stu-id="13e84-157">See also</span></span>

- [<span data-ttu-id="13e84-158">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="13e84-158">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)   
- [<span data-ttu-id="13e84-159">EWS アプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="13e84-159">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    

