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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758943"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a>Exchange SCP のルックアップを使用して自動検出エンドポイントを検索します。

Active Directory ドメイン サービス (AD DS) での自動検出 SCP オブジェクトを検索し、Exchange の自動検出サービスで使用する自動検出エンドポイントの Url を探す場合に使用する方法を確認します。
  
自動検出では、Exchange サーバー上のメールボックスに接続するために必要な情報を取得するために簡単です。 ただし、自動検出を使用するには、自動検出サーバーの設定を取得しているユーザーに適切なを検索する方法が必要です。 AD DS 内のサービス接続ポイント (SCP) オブジェクトは、ドメインに参加しているクライアントが自動検出サーバーを検索する簡単な方法を提供します。 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a>自動検出エンドポイントを検出できるようにセットアップする
<a name="bk_PreReqs"> </a>

AD DS では、自動検出 SCP オブジェクトを探し、次にアクセスする必要があります。
  
- Exchange 2007 SP1 以降の Exchange オンプレミス バージョンを実行しているサーバー。
    
- Exchange サーバーがインストールされているドメインに参加しているクライアント コンピューター。
    
- Exchange サーバーにメールボックスがあるユーザー アカウント。  
    
また、作業を開始する前にする必要があります理解するいくつかの基本的な概念です。 役に立つことがわかりますいくつかのリソースを次に示します。
  
**表 1 です。SCP オブジェクトから自動検出エンドポイントを検索するための関連記事**

|**この記事を読む**|**について説明しています.**|
|:-----|:-----|
|[Exchange の自動検出](autodiscover-for-exchange.md) <br/> |自動検出サービスの動作方法。  <br/> |
|[サービス接続ポイントの発行](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |SCP オブジェクトを使用してサービス固有のデータを発行する方法。  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a>AD DS 内の自動検出 SCP オブジェクトを検索します。
<a name="bk_LocateScpObjects"> </a>

AD DS で公開されている自動検出エンドポイントを検索するための第一歩は、自動検出 SCP オブジェクトを検索します。 Exchange では、自動検出の 2 種類の SCP オブジェクトを発行します。
  
- **SCP ポインター** : ユーザーのドメインの自動検出 SCP オブジェクトの検索に使用する特定の LDAP サーバーをポイントするための情報が含まれます。 SCP ポインターには、次の GUID がスタンプされて: 67661d7F-8 個の FC 4-4fa7-BFAC-E1D7794C1F68 です。 
    
- **SCP Url**自動検出エンドポイントの Url が含まれます。 SCP Url には次の GUID を持つスタンプ: 77378F46-2 C 66-4aa9-A6A6-3E7A48B19596 です。 
    
### <a name="to-locate-autodiscover-scp-objects"></a>自動検出 SCP オブジェクトを見つけるには

1. ルート ドメインの構成名前付けコンテキストへのパスを取得するのには AD DS の dse サービスのエントリの**configurationNamingContext**プロパティを参照してください。 [DirectoryEntry](http://msdn2.microsoft.com/EN-US/library/z9cddzaa)クラス、または AD DS にアクセスできる他の任意の API を使用してこれを行うことができます。 
    
2. 構成名前付けコンテキストの SCP オブジェクトをいずれか、SCP ポインターの GUID を持つか、SCP URL に GUID**キーワード**のプロパティを検索します。 
    
3. SCP オブジェクトを SCP ポインターと同じエントリの [**キーワード**] プロパティを確認することでユーザーのドメインのスコープを検索したことを確認`"Domain=<domain>"`。 などのユーザーの電子メール アドレスが elvin@contoso.com の場合は、するを検索、SCP ポインターと同じである**キーワード**プロパティのエントリを`"Domain=contoso.com"`。 一致する SCP ポインターがある場合 SCP オブジェクトのセットを破棄して、手順 1 のルート DSE のエントリに接続するサーバーとして、 **serviceBindingInformation**プロパティの値を使用して最初からやり直す。 
    
4. SCP ポインターは任意のドメインのスコープを確認し、名前を付けて、 **serviceBindingInformation**プロパティの値「フォールバック」のサーバーでは、現在のサーバーは提供しませんいずれかの場合にユーザーのドメインを対象にした SCP ポインターがない場合は、結果です。 
    
5. 対象ドメインをスコープとする SCP ポインターがまったく見つからなくなれば、次の手順に進めます。次の手順では、結果から自動検出エンドポイントの優先順位を付けた一覧を生成します。
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a>自動検出エンドポイントの優先順位を付けた一覧を生成する
<a name="bk_GenerateList"> </a>

見つけた一連の SCP オブジェクトを使用して、優先順位を付けた自動検出エンドポイント URL の一覧を生成できます。そのためには次の手順を実行します。
  
1. クライアント コンピューターの Active Directory サイト名を取得します。
    
2. SCP オブジェクトを検出すると、一連の SCP URL ごとに**キーワード**のプロパティを確認し、次の規則に基づく URL に優先順位を割り当てます。 
    
  - **キーワード**プロパティに値が含まれているかどうか`"Site=<site name>"`、`<site name>`と等しいが、前の手順で取得したサイトのアクティブなディレクトリの名前は、URL 1 の優先順位を割り当てます。 
    
  - **Keywords**プロパティで始まる値を持つエントリが含まれていない場合は、 `"Site="`、2 の優先順位の URL を割り当てます。 
    
  - **キーワード**のプロパティに値が含まれているかどうか`"Site=<site name>`、`<site name>`はないと同じ、前の手順で取得する Active Directory サイトの名前を 3 の優先順位の URL を割り当てます。 
    
## <a name="code-example-performing-an-scp-lookup"></a>コード例:SCP 参照
<a name="bk_CodeExample"> </a>

次のコード例では、自動検出 SCP オブジェクトを検索し、エンドポイントの自動検出の優先順位の一覧を生成する方法が表示されます。
  
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

## <a name="next-steps"></a>次の手順
<a name="bk_NextSteps"> </a>

自動検出プロセスの次の手順では、見つかった URL に対して自動検出要求を送信します。その際、優先順位 1 の URL、優先順位 2 の URL、最後に優先順位 3 の URL の順に送信します。自動検出要求を送信し、応答を処理する方法の詳細については、以下の資料を参照してください。
  
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [自動検出のエラー メッセージの処理](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a>関連項目

- [Exchange の自動検出](autodiscover-for-exchange.md)   
- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)
    

