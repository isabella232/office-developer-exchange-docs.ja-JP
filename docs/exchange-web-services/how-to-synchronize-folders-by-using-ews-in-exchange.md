---
title: Exchange で EWS を使用してフォルダーを同期させる
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。
ms.openlocfilehash: 4b0686134d642da34b2890a0e692e3d03e4a9fb1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759066"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a><span data-ttu-id="df702-103">Exchange で EWS を使用してフォルダーを同期させる</span><span class="sxs-lookup"><span data-stu-id="df702-103">How to: Synchronize folders by using EWS in Exchange</span></span>

<span data-ttu-id="df702-104">クライアントを同期させるために、EWS マネージ API または EWS を使用して、フォルダーの一覧、または変更されたフォルダーの一覧を取得する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="df702-104">Find out how to use the EWS Managed API or EWS to get a list of folders, or a list of folders that have changed, in order to synchronize your client.</span></span>
  
<span data-ttu-id="df702-p101">Exchange の EWS では、アイテムの同期とフォルダーの同期を使用して、クライアントとサーバー間でメールボックスのコンテンツを同期します。フォルダー同期では、ルート フォルダーにあるフォルダーの初期一覧が取得され、その後時間の経過とともに、それらのフォルダーに対して行われた変更が取得され、新しいフォルダーも取得されます。</span><span class="sxs-lookup"><span data-stu-id="df702-p101">EWS in Exchange uses item synchronization and folder synchronization to sync mailbox content between the client and server. Folder synchronization gets the initial list of folders from a root folder and then, over time, gets changes that were made to those folders and gets new folders as well.</span></span>
  
<span data-ttu-id="df702-107">EWS マネージ API を使用してフォルダー同期を行う場合は、まず [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) メソッドを使用して[ルート フォルダー内のフォルダーの初期一覧を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)します。</span><span class="sxs-lookup"><span data-stu-id="df702-107">If you're performing folder synchronization by using the EWS Managed API, you first [get the initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) by using the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="df702-108">次に、後続の呼び出し時に _cSyncState_ パラメーターの値を更新して、新しいフォルダーと変更されたフォルダーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="df702-108">You then update the value of the  _cSyncState_ parameter during subsequent calls to get the list of new and changed folders.</span></span> 
  
<span data-ttu-id="df702-109">EWS を使用してフォルダー同期を行うには、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用して[ルート フォルダー内のフォルダーの初期一覧](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest)を要求し、応答を解析します。その後ある時点で、[ルート フォルダー内のフォルダーに対する変更を取得](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)し、応答を解析します。</span><span class="sxs-lookup"><span data-stu-id="df702-109">To perform folder synchronization by using EWS, you request the [initial list of folders in the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation, parse the response, and then at some point in the future [get the changes to the folders in the root](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews), and parse the response. After the client receives the list of initial or changed folders, it makes updates locally. How and when you retrieve changes in the future depends on the synchronization design pattern your application is using.</span></span> <span data-ttu-id="df702-110">クライアントは、初期のフォルダーまたは変更されたフォルダーの一覧を受信した後、[ローカルに更新を実行](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)します。</span><span class="sxs-lookup"><span data-stu-id="df702-110">After the client receives the list of initial or changed folders, it [makes updates locally](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="df702-111">今後いつどのように変更を取得するかは、アプリケーションが使用している[同期デザイン パターン](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns)によって異なります。</span><span class="sxs-lookup"><span data-stu-id="df702-111">How and when you retrieve changes in the future depends on the [synchronization design pattern](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) your application is using.</span></span> 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="df702-112">EWS マネージ API を使用してすべてのフォルダーまたは変更されたフォルダーの一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="df702-112">Get the list of all folders or changed folders by using the EWS Managed API</span></span>
<span data-ttu-id="df702-113"><a name="bk_cesyncinitialewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="df702-113"></span></span>

<span data-ttu-id="df702-114">次のコード例は、ルート フォルダー内のフォルダーの初期一覧を取得した後、ルート フォルダー内のフォルダーに対して前回の同期後に行われた変更の一覧を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-114">The following code example shows how to get an initial list of folders in a root folder and then get a list of changes to folders in the root folder that have occurred since the previous synchronization.</span></span> <span data-ttu-id="df702-115">[ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) メソッドへの最初の呼び出し時に、_cSyncState_ 値を null に設定します。</span><span class="sxs-lookup"><span data-stu-id="df702-115">During the initial call to the [ExchangeService.SyncFolderHierarchy](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) method, set the  _cSyncState_ value to null.</span></span> <span data-ttu-id="df702-116">メソッドが完了したら、次の **SyncFolderHierarchy** メソッド呼び出しで使用するために _cSyncState_ 値をローカルに保存します。</span><span class="sxs-lookup"><span data-stu-id="df702-116">When the method completes, save the  _cSyncState_ value locally to use in the next **SyncFolderHierarchy** method call.</span></span> <span data-ttu-id="df702-117">最初の呼び出しと後続の呼び出しの両方で、変更がなくなるまで、**SyncFolderHierarchy** メソッドの連続呼び出しを使用して、10 回のバッチ処理でフォルダーが取得されます。</span><span class="sxs-lookup"><span data-stu-id="df702-117">In both the initial call and the subsequent calls, the folders are retrieved in batches of ten, by using successive calls to the **SyncFolderHierarchy** method, until no more changes remain.</span></span> <span data-ttu-id="df702-118">次の例は、_propertySet_ パラメーターを IdOnly に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。</span><span class="sxs-lookup"><span data-stu-id="df702-118">This example sets the _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a [synchronization best practice. In this example, we assume that service is a valid ExchangeService](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) object binding and that cSyncState represents the sync state that was returned by a prior call to SyncFolderItems.</span></span> <span data-ttu-id="df702-119">この例では、**service** は有効な **ExchangeService** オブジェクト バインドであり、_cSyncState_ は前の **SyncFolderHierarchy** 呼び出しによって返された同期状態を表すものとします。</span><span class="sxs-lookup"><span data-stu-id="df702-119">This example sets the _propertySet_ parameter to IdOnly to reduce calls to the Exchange database, which is a synchronization best practice. In this example, we assume that **service** is a valid **ExchangeService** object binding and that cSyncState represents the sync state that was returned by a prior call to **SyncFolderItems**.</span></span> 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

<span data-ttu-id="df702-120">サーバー上の新しいフォルダーまたは変更されたフォルダーの一覧を取得した後、[クライアント上のフォルダーを作成または更新します](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)。</span><span class="sxs-lookup"><span data-stu-id="df702-120">After you retrieve the list of new or changed folders on the server, [create or update the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a><span data-ttu-id="df702-121">EWS を使用してフォルダーの初期一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="df702-121">Get the initial list of folders by using EWS</span></span>
<span data-ttu-id="df702-122"><a name="bk_cesyncewsrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="df702-122"></span></span>

<span data-ttu-id="df702-123">次の例は、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用して初期フォルダー階層を取得するための XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-123">The following example shows an XML request to get the initial folder hierarchy by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="df702-124">これは、[SyncFolderHierarchy メソッドを使用して初期フォルダーの一覧を取得する](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)ときに EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="df702-124">This is also the XML request that the EWS Managed API sends when [retrieving the list of initial folders by using the SyncFolderHierarchy method](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="df702-125">[SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) 操作の [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素は、これが最初の同期であるために含まれません。</span><span class="sxs-lookup"><span data-stu-id="df702-125">The [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element of the [SyncFolderHierarchy](http://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) operation is not included because this is the initial synchronization.</span></span> <span data-ttu-id="df702-126">次の例は、[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定して、Exchange データベースの呼び出し回数を減らしています。これは[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。</span><span class="sxs-lookup"><span data-stu-id="df702-126">This example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** to reduce calls to the Exchange database, which is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="df702-127">次の例は、サーバーが [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作要求を処理した後に返す XML 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-127">The following example shows the XML response that the server returns after it processes the [GetItem](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="df702-128">最初の応答には、すべてのフォルダーで [Create](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) 要素が含まれます。最初の同期ではすべてのフォルダーが新規と見なされるからです。</span><span class="sxs-lookup"><span data-stu-id="df702-128">The initial response includes [Create](http://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elements for all folders because all folders are considered new during an initial synchronization.</span></span> <span data-ttu-id="df702-129">一部の属性と要素の値は、読みやすくするために短くなっています。また、いくつかの **Create** 要素ブロックは、簡潔にするために削除されています。</span><span class="sxs-lookup"><span data-stu-id="df702-129">The values of some attributes and elements have been shortened for readability, and some **Create** element blocks were removed for brevity.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="df702-130">サーバー上の新しいフォルダーの一覧を受信した後、[クライアント上にフォルダーを作成](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)します。</span><span class="sxs-lookup"><span data-stu-id="df702-130">After you retrieve the list of new folders on the server, [create the folders on the client](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a><span data-ttu-id="df702-131">EWS を使用して前回の同期以降の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="df702-131">Get the changes since the last sync by using EWS</span></span>
<span data-ttu-id="df702-132"><a name="bk_cesyncrespews"> </a></span><span class="sxs-lookup"><span data-stu-id="df702-132"></span></span>

<span data-ttu-id="df702-133">次の例は、[SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) 操作を使用してルート フォルダー内のフォルダーに対する変更の一覧を取得するための XML 要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-133">The following example shows the XML request to get the list of changes to folders in the root folder by using the [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="df702-134">これは、[ルート フォルダーに対する変更の一覧を取得する](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma)ときに EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="df702-134">This is also the XML request that the EWS Managed API sends when [retrieving the list of changes to the root folder](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma).</span></span> <span data-ttu-id="df702-135">この例では、[SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素の値を前回の応答で返された値に設定しています。</span><span class="sxs-lookup"><span data-stu-id="df702-135">This example sets the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element value to the value returned in the previous response.</span></span> <span data-ttu-id="df702-136">また、この例では、返される追加のプロパティを示すために、デモの目的で [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** ではなく **AllProperties** に設定しています。</span><span class="sxs-lookup"><span data-stu-id="df702-136">And for demonstration purposes, this example sets the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **AllProperties** instead of **IdOnly** to show the additional properties returned.</span></span> <span data-ttu-id="df702-137">[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) 要素を **IdOnly** に設定することが、[同期のベスト プラクティス](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)です。</span><span class="sxs-lookup"><span data-stu-id="df702-137">Setting the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element to **IdOnly** is a [synchronization best practice](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices).</span></span> <span data-ttu-id="df702-138">**SyncState** の値は、読みやすくするために短くなっています。</span><span class="sxs-lookup"><span data-stu-id="df702-138">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="df702-139">次の例は、サーバーがクライアントからの [SyncFolderHierarchy 操作](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx)要求を処理した後に返す XML 応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-139">The following example shows the XML response that is returned by the server after it parses the request from the client.</span></span> <span data-ttu-id="df702-140">この応答は、前回の同期以降 1 つのフォルダーが更新され、1 つのフォルダーが作成されて、1 つのフォルダーが削除されたことを示しています。</span><span class="sxs-lookup"><span data-stu-id="df702-140">This response indicates that one folder was updated, one folder was created, and one folder was deleted since the prior synchronization.</span></span> <span data-ttu-id="df702-141">[SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) 要素の値、**Id** 属性、および **ChangeKey** 属性は、読みやすくするために短くなっています。</span><span class="sxs-lookup"><span data-stu-id="df702-141">The value of the [SyncState](http://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) element, **Id** attributes, and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
<span data-ttu-id="df702-142">要求に **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) が含まれていたことを思い出してください。</span><span class="sxs-lookup"><span data-stu-id="df702-142">Remember that the request included the **AllProperties**[BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx).</span></span> <span data-ttu-id="df702-143">これは単にデモの目的のためです。</span><span class="sxs-lookup"><span data-stu-id="df702-143">This is just for demonstration purposes.</span></span> <span data-ttu-id="df702-144">運用環境では、**BaseShape** 要素を **IdOnly** に設定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="df702-144">Remember that the request included the **AllProperties** BaseShape. This is just for demonstration purposes. We recommend that you set the **BaseShape** element to IdOnly in production.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
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
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
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
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a><span data-ttu-id="df702-145">クライアントを更新する</span><span class="sxs-lookup"><span data-stu-id="df702-145">Update the client</span></span>
<span data-ttu-id="df702-146"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="df702-146"></span></span>

<span data-ttu-id="df702-147">EWS マネージ API を使用する場合は、新しいフォルダーまたは変更されたフォルダーの一覧を取得した後、[Folder.Load](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) メソッドを使用して新しいフォルダーまたは変更されたフォルダーのプロパティを取得し、それらのプロパティをローカル値と比較して、クライアント上のフォルダーを更新または作成します。</span><span class="sxs-lookup"><span data-stu-id="df702-147">If you’re using the EWS Managed API, after you get the list of new or changed folders, use the [Folder.Loadhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.load(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) method to get properties on the new or changed items, compare the properties to the local values, and update or create the folders on the client.</span></span> 
  
<span data-ttu-id="df702-148">EWS を使用する場合は、[GetFolder 操作](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)を使用して新しいフォルダーまたは変更されたフォルダーのプロパティを取得して、クライアント上のフォルダーを更新または作成します。</span><span class="sxs-lookup"><span data-stu-id="df702-148">If you’re using EWS, use the [GetFolder Operation](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get properties on the new or changed folders and update or create the folders on the client.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="df702-149">関連項目</span><span class="sxs-lookup"><span data-stu-id="df702-149">See also</span></span>

- [<span data-ttu-id="df702-150">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="df702-150">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)   
- [<span data-ttu-id="df702-151">Exchange で EWS を使用してアイテムを同期する</span><span class="sxs-lookup"><span data-stu-id="df702-151">How to: Synchronize items by using EWS in Exchange</span></span>](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="df702-152">Exchange の EWS での同期に関連するエラーの処理</span><span class="sxs-lookup"><span data-stu-id="df702-152">Handling synchronization-related errors in EWS in Exchange</span></span>](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

