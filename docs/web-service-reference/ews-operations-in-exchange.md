---
title: Exchange での EWS 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Exchange で使用可能な EWS 操作についての情報を検索します。
localization_priority: Priority
ms.openlocfilehash: 143903d9198a7e31e876adcbbb336df34ecf01fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526124"
---
# <a name="ews-operations-in-exchange"></a><span data-ttu-id="762db-103">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="762db-103">EWS operations in Exchange</span></span>

<span data-ttu-id="762db-104">Exchange で使用可能な EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="762db-104">Find information about the EWS operations that are available in Exchange.</span></span>
  
<span data-ttu-id="762db-105">Exchange Web サービス (EWS) には、Exchange ストアからの情報へのアクセスを可能にする多くの操作が用意されています。</span><span class="sxs-lookup"><span data-stu-id="762db-105">Exchange Web Services (EWS) provides many operations that enable you to access information from the Exchange store.</span></span> <span data-ttu-id="762db-106">このセクションの記事では、EWS 操作の要求、応答、エラー応答メッセージの全体的な構造、および各操作の XML 例について説明します。</span><span class="sxs-lookup"><span data-stu-id="762db-106">The articles in this section provide information about the overall structure of the requests, responses, and error response messages for EWS operations, as well as XML examples for each operation.</span></span> <span data-ttu-id="762db-107">クライアントとサーバー間で送信されるメッセージ構造の概要を説明します。</span><span class="sxs-lookup"><span data-stu-id="762db-107">They provide an overview of the message structures that are sent between the client and the server.</span></span> <span data-ttu-id="762db-108">この情報を使用して、メッセージ構造をデバッグしたり、EWS 要求で何ができるかについての情報を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="762db-108">You can use this information to debug message structures and to find information about what you can do in an EWS request.</span></span> <span data-ttu-id="762db-109">XML 構造が何を表しているかの詳細については、「 [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762db-109">For more information about what the XML structure represents, see - [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md).</span></span>
  
<span data-ttu-id="762db-110">すべての EWS 機能は、スキーマのバージョンに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="762db-110">All EWS functionality is associated with a version of the schema.</span></span> <span data-ttu-id="762db-111">新しい EWS スキーマのバージョンは、Exchange Server または Exchange Online の新しいリリースで導入されました。</span><span class="sxs-lookup"><span data-stu-id="762db-111">New EWS schema versions are introduced in new releases of Exchange Server or Exchange Online.</span></span> <span data-ttu-id="762db-112">[RequestServerVersion](requestserverversion.md)要素には、サーバーバージョンをスキーマバージョンにマップする**version**属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="762db-112">The [RequestServerVersion](requestserverversion.md) element contains a **Version** attribute that maps the server version to the schema version.</span></span> <span data-ttu-id="762db-113">この記事では、各操作がいつ導入されたかについて説明します。</span><span class="sxs-lookup"><span data-stu-id="762db-113">This article provides information about when each operation was introduced.</span></span> <span data-ttu-id="762db-114">操作内の特定の機能によっては、サービスの新しいバージョンが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="762db-114">Specific functionality within an operation might require a later version of the service.</span></span> <span data-ttu-id="762db-115">以前のバージョンの EWS に対して設計されたクライアントが、新しいバージョンの EWS で動作するように、バージョン付きのスキーマが実装されています。</span><span class="sxs-lookup"><span data-stu-id="762db-115">The versioned schemas are implemented so that clients that are designed against an older version of EWS will work with a newer version of EWS.</span></span> 
  
<span data-ttu-id="762db-116">これらの操作は、メールボックスを処理する EWS エンドポイントを対象とすることができます。</span><span class="sxs-lookup"><span data-stu-id="762db-116">These operations can target the EWS endpoint that services your mailbox.</span></span> <span data-ttu-id="762db-117">Http:///ews/exchange .asmx に似た URL を使用して、EWS エンドポイントを参照できます。 <clientaccessserver> ここで、 <clientaccessserver> はメールボックスをサービスする Exchange クライアントアクセスサーバーです。</span><span class="sxs-lookup"><span data-stu-id="762db-117">You can browse to the EWS endpoint by using a URL that is similar in structure to http://<clientaccessserver>.com/ews/exchange.asmx, where <clientaccessserver> is the Exchange Client Access server that services your mailbox.</span></span> <span data-ttu-id="762db-118">自動検出を使用して、メールボックスをサービスするクライアントアクセスサーバーへの URL を取得できます。</span><span class="sxs-lookup"><span data-stu-id="762db-118">You can use Autodiscover to get the URL to the Client Access server that services your mailbox.</span></span> <span data-ttu-id="762db-119">自動検出の詳細については、「 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762db-119">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="762db-120">電子情報開示の操作</span><span class="sxs-lookup"><span data-stu-id="762db-120">eDiscovery operations</span></span>
<span data-ttu-id="762db-121"><a name="bk_eDiscovery"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-121"><a name="bk_eDiscovery"> </a></span></span>

<span data-ttu-id="762db-122">電子情報開示操作は、法的情報保留のための検索操作を提供し、探索検索結果でインデックスが作成されずに返されるメールボックスのデータを特定します。</span><span class="sxs-lookup"><span data-stu-id="762db-122">The eDiscovery operations provide search operations for legal holds and identify mailbox data that cannot be indexed and returned in discovery search results.</span></span>
  
<span data-ttu-id="762db-123">次の表に、電子情報開示操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-123">The following table lists the eDiscovery operations.</span></span>
  
|<span data-ttu-id="762db-124">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-124">**Operation name**</span></span>|<span data-ttu-id="762db-125">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-125">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-126">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-126">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md) <br/> |<span data-ttu-id="762db-127">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-127">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-128">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="762db-128">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md) <br/> |<span data-ttu-id="762db-129">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-129">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-130">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="762db-130">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md) <br/> |<span data-ttu-id="762db-131">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-131">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-132">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="762db-132">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md) <br/> |<span data-ttu-id="762db-133">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-133">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-134">Getsearchablemailemail箱操作</span><span class="sxs-lookup"><span data-stu-id="762db-134">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md) <br/> |<span data-ttu-id="762db-135">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-135">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-136">SearchMailboxes ボックスの操作</span><span class="sxs-lookup"><span data-stu-id="762db-136">SearchMailboxes operation</span></span>](searchmailboxes-operation.md) <br/> |<span data-ttu-id="762db-137">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-137">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-138">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="762db-138">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md) <br/> |<span data-ttu-id="762db-139">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-139">Exchange 2013</span></span>  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a><span data-ttu-id="762db-140">Exchange メールボックスデータの操作</span><span class="sxs-lookup"><span data-stu-id="762db-140">Exchange mailbox data operations</span></span>
<span data-ttu-id="762db-141"><a name="bk_Exchange_mailbox_data"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-141"><a name="bk_Exchange_mailbox_data"> </a></span></span>

<span data-ttu-id="762db-142">Exchange メールボックスデータ操作を使用すると、クライアントはアイテム、フォルダー、および添付ファイルを処理および整理し、あいまいな名前解決と配布リストの展開を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="762db-142">The Exchange mailbox data operations enable clients to handle and organize items, folders, and attachments, as well as ambiguous name resolution and distribution list expansion.</span></span> <span data-ttu-id="762db-143">Exchange メールボックスのデータ操作には、アイテム、フォルダー、添付ファイル、およびユーティリティの操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="762db-143">Exchange mailbox data operations include item, folder, attachment, and utilities operations.</span></span>
  
<span data-ttu-id="762db-144">次の表に、Exchange メールボックスのデータ操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-144">The following table lists the Exchange mailbox data operations.</span></span>
  
|<span data-ttu-id="762db-145">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-145">**Operation name**</span></span>|<span data-ttu-id="762db-146">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-146">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-147">アーカイブアイテムの操作</span><span class="sxs-lookup"><span data-stu-id="762db-147">ArchiveItem operation</span></span>](archiveitem-operation.md) <br/> |<span data-ttu-id="762db-148">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-148">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-149">CreateItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-149">CreateItem operation</span></span>](createitem-operation.md) <br/> |<span data-ttu-id="762db-150">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-150">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-151">CopyItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-151">CopyItem operation</span></span>](copyitem-operation.md) <br/> |<span data-ttu-id="762db-152">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-152">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-153">DeleteItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-153">DeleteItem operation</span></span>](deleteitem-operation.md) <br/> |<span data-ttu-id="762db-154">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-154">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-155">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-155">FindItem operation</span></span>](finditem-operation.md) <br/> |<span data-ttu-id="762db-156">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-156">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-157">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-157">GetItem operation</span></span>](getitem-operation.md) <br/> |<span data-ttu-id="762db-158">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-158">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-159">MarkAllItemsAsRead 操作</span><span class="sxs-lookup"><span data-stu-id="762db-159">MarkAllItemsAsRead operation</span></span>](markallitemsasread-operation.md) <br/> |<span data-ttu-id="762db-160">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-160">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-161">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-161">MoveItem operation</span></span>](moveitem-operation.md) <br/> |<span data-ttu-id="762db-162">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-162">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-163">SendItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-163">SendItem operation</span></span>](senditem-operation.md) <br/> |<span data-ttu-id="762db-164">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-164">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-165">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="762db-165">UpdateItem operation</span></span>](updateitem-operation.md) <br/> |<span data-ttu-id="762db-166">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-166">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="762db-167">次の表に、Exchange メールボックスデータフォルダーの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-167">The following table lists the Exchange mailbox data folder operations.</span></span>
  
|<span data-ttu-id="762db-168">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-168">**Operation name**</span></span>|<span data-ttu-id="762db-169">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-169">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-170">CreateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-170">CreateFolder operation</span></span>](createfolder-operation.md) <br/> |<span data-ttu-id="762db-171">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-171">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-172">CreateFolderPath 操作</span><span class="sxs-lookup"><span data-stu-id="762db-172">CreateFolderPath operation</span></span>](createfolderpath-operation.md) <br/> |<span data-ttu-id="762db-173">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-173">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-174">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-174">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md) <br/> |<span data-ttu-id="762db-175">Exchange 2007。</span><span class="sxs-lookup"><span data-stu-id="762db-175">Exchange 2007.</span></span> <span data-ttu-id="762db-176">Exchange 2010 以降のバージョンの Exchange では、この機能は強調されていません。</span><span class="sxs-lookup"><span data-stu-id="762db-176">This functionality has been deemphasized in versions of Exchange starting with Exchange 2010.</span></span> <span data-ttu-id="762db-177">メッセージングレコード管理用の保持タグおよびポリシーを使用するように移行する方法の詳細については、「[管理フォルダーからの移行](https://technet.microsoft.com/library/dd298032%28v=exchg.141%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762db-177">For more information about how to migrate to using retention tags and policies for messaging records management, see [Migrate from Managed Folders](https://technet.microsoft.com/library/dd298032%28v=exchg.141%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="762db-178">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-178">CopyFolder operation</span></span>](copyfolder-operation.md) <br/> |<span data-ttu-id="762db-179">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-179">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-180">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-180">DeleteFolder operation</span></span>](deletefolder-operation.md) <br/> |<span data-ttu-id="762db-181">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-181">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-182">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-182">EmptyFolder operation</span></span>](emptyfolder-operation.md) <br/> |<span data-ttu-id="762db-183">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-183">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-184">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-184">FindFolder operation</span></span>](findfolder-operation.md) <br/> |<span data-ttu-id="762db-185">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-185">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-186">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-186">GetFolder operation</span></span>](getfolder-operation.md) <br/> |<span data-ttu-id="762db-187">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-187">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-188">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-188">MoveFolder operation</span></span>](movefolder-operation.md) <br/> |<span data-ttu-id="762db-189">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-189">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-190">UpdateFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-190">UpdateFolder operation</span></span>](updatefolder-operation.md) <br/> |<span data-ttu-id="762db-191">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-191">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="762db-192">次の表に、Exchange メールボックスデータ添付操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-192">The following table lists the Exchange mailbox data attachment operations.</span></span>
  
|<span data-ttu-id="762db-193">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-193">**Operation name**</span></span>|<span data-ttu-id="762db-194">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-194">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-195">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="762db-195">CreateAttachment operation</span></span>](createattachment-operation.md) <br/> |<span data-ttu-id="762db-196">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-196">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-197">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="762db-197">GetAttachment operation</span></span>](getattachment-operation.md) <br/> |<span data-ttu-id="762db-198">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-198">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-199">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="762db-199">DeleteAttachment operation</span></span>](deleteattachment-operation.md) <br/> |<span data-ttu-id="762db-200">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-200">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="762db-201">次の表に、Exchange メールボックスのアラーム操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-201">The following table lists the Exchange mailbox reminder operations.</span></span>
  
|<span data-ttu-id="762db-202">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-202">**Operation name**</span></span>|<span data-ttu-id="762db-203">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-203">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-204">GetReminders 操作</span><span class="sxs-lookup"><span data-stu-id="762db-204">GetReminders operation</span></span>](getreminders-operation.md) <br/> |<span data-ttu-id="762db-205">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-205">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-206">PerformReminderAction 操作</span><span class="sxs-lookup"><span data-stu-id="762db-206">PerformReminderAction operation</span></span>](performreminderaction-operation.md) <br/> |<span data-ttu-id="762db-207">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-207">Exchange 2013</span></span>  <br/> |
   
<span data-ttu-id="762db-208">次の表に、Exchange メールボックスデータの会話操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-208">The following table lists the Exchange mailbox data conversation operations.</span></span>
  
|<span data-ttu-id="762db-209">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-209">**Operation name**</span></span>|<span data-ttu-id="762db-210">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-210">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-211">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="762db-211">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md) <br/> |<span data-ttu-id="762db-212">Exchange 2010 Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="762db-212">Exchange 2010 Service Pack 1 (SP1)</span></span>  <br/> |
|[<span data-ttu-id="762db-213">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="762db-213">FindConversation operation</span></span>](findconversation-operation.md) <br/> |<span data-ttu-id="762db-214">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-214">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-215">GetConversationItems 操作</span><span class="sxs-lookup"><span data-stu-id="762db-215">GetConversationItems operation</span></span>](getconversationitems-operation.md) <br/> |<span data-ttu-id="762db-216">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-216">Exchange 2013</span></span>  <br/> |
   
<span data-ttu-id="762db-217">次の表に、Exchange メールボックスデータユーティリティの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-217">The following table lists the Exchange mailbox data utilities operations.</span></span>
  
|<span data-ttu-id="762db-218">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-218">**Operation name**</span></span>|<span data-ttu-id="762db-219">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-219">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-220">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="762db-220">ConvertId operation</span></span>](convertid-operation.md) <br/> |<span data-ttu-id="762db-221">Exchange 2007 Service Pack 1</span><span class="sxs-lookup"><span data-stu-id="762db-221">Exchange 2007 Service Pack 1</span></span>  <br/> |
|[<span data-ttu-id="762db-222">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="762db-222">ExpandDL operation</span></span>](expanddl-operation.md) <br/> |<span data-ttu-id="762db-223">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-223">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-224">GetUserPhoto 操作</span><span class="sxs-lookup"><span data-stu-id="762db-224">GetUserPhoto operation</span></span>](getuserphoto-operation.md) <br/> |<span data-ttu-id="762db-225">Exchange 2013。</span><span class="sxs-lookup"><span data-stu-id="762db-225">Exchange 2013.</span></span> <span data-ttu-id="762db-226">この操作には、REST と SOAP の実装の両方があります。</span><span class="sxs-lookup"><span data-stu-id="762db-226">This operation has both a REST and a SOAP implementation.</span></span>  <br/> |
|[<span data-ttu-id="762db-227">MarkAsJunk 操作</span><span class="sxs-lookup"><span data-stu-id="762db-227">MarkAsJunk operation</span></span>](markasjunk-operation.md) <br/> |<span data-ttu-id="762db-228">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-228">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-229">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="762db-229">ResolveNames operation</span></span>](resolvenames-operation.md) <br/> |<span data-ttu-id="762db-230">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-230">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-231">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="762db-231">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md) <br/> |<span data-ttu-id="762db-232">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-232">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="availability-operations"></a><span data-ttu-id="762db-233">可用性の操作</span><span class="sxs-lookup"><span data-stu-id="762db-233">Availability operations</span></span>
<span data-ttu-id="762db-234"><a name="bk_Availability"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-234"><a name="bk_Availability"> </a></span></span>

<span data-ttu-id="762db-235">可用性の操作により、より安全で最新の、または豊富な空き時間情報が提供され、予定表と空き時間情報の共有の機能が向上します。</span><span class="sxs-lookup"><span data-stu-id="762db-235">The availability operations improve the calendar and free/busy sharing experience by providing more secure, up-to-date, and rich free/busy information.</span></span> <span data-ttu-id="762db-236">空き時間情報データは、会議をスケジュールするための重要なコンポーネントです。</span><span class="sxs-lookup"><span data-stu-id="762db-236">Free/busy data is a critical component of scheduling meetings.</span></span> <span data-ttu-id="762db-237">可用性運用は、効果的なスケジュール設定のための信頼できる基盤を提供します。</span><span class="sxs-lookup"><span data-stu-id="762db-237">The availability operations provide a reliable foundation for effective scheduling.</span></span> 
  
<span data-ttu-id="762db-238">次の表に、可用性の操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-238">The following table lists the availability operations.</span></span>
  
|<span data-ttu-id="762db-239">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-239">**Operation name**</span></span>|<span data-ttu-id="762db-240">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-240">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-241">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="762db-241">GetUserAvailability operation</span></span>](getuseravailability-operation.md) <br/> |<span data-ttu-id="762db-242">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-242">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-243">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="762db-243">GetRoomLists operation</span></span>](getroomlists-operation.md) <br/> |<span data-ttu-id="762db-244">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-244">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-245">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="762db-245">GetRooms operation</span></span>](getrooms-operation.md) <br/> |<span data-ttu-id="762db-246">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-246">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-247">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="762db-247">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) <br/> |<span data-ttu-id="762db-248">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-248">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-249">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="762db-249">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md) <br/> |<span data-ttu-id="762db-250">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-250">Exchange 2007</span></span>  <br/> |
   
## <a name="bulk-transfer-operations"></a><span data-ttu-id="762db-251">一括転送操作</span><span class="sxs-lookup"><span data-stu-id="762db-251">Bulk transfer operations</span></span>
<span data-ttu-id="762db-252"><a name="bk_bulk_transfer"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-252"><a name="bk_bulk_transfer"> </a></span></span>

<span data-ttu-id="762db-253">一括転送操作を使用すると、クライアントはメールボックスのアイテムをストリームすることができます。</span><span class="sxs-lookup"><span data-stu-id="762db-253">The bulk transfer operations enable clients to stream items into and out of a mailbox.</span></span> 
  
<span data-ttu-id="762db-254">次の表に一括転送操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-254">The following table lists the bulk transfer operations.</span></span>
  
|<span data-ttu-id="762db-255">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-255">**Operation name**</span></span>|<span data-ttu-id="762db-256">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-256">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-257">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="762db-257">UploadItems operation</span></span>](uploaditems-operation.md) <br/> |<span data-ttu-id="762db-258">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-258">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-259">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="762db-259">ExportItems operation</span></span>](exportitems-operation.md) <br/> |<span data-ttu-id="762db-260">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-260">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="delegate-management-operations"></a><span data-ttu-id="762db-261">管理操作を委任する</span><span class="sxs-lookup"><span data-stu-id="762db-261">Delegate management operations</span></span>
<span data-ttu-id="762db-262"><a name="bk_delegate_management"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-262"><a name="bk_delegate_management"> </a></span></span>

<span data-ttu-id="762db-263">代理人管理操作を使用すると、クライアントはメールボックスの代理人の追加、取得、更新、削除を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="762db-263">The delegate management operations enable clients to add, get, update, and remove delegates from their mailboxes.</span></span> 
  
<span data-ttu-id="762db-264">次の表に、代理人の管理操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-264">The following table lists the delegate management operations.</span></span>
  
|<span data-ttu-id="762db-265">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-265">**Operation name**</span></span>|<span data-ttu-id="762db-266">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-266">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-267">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="762db-267">AddDelegate operation</span></span>](adddelegate-operation.md) <br/> |<span data-ttu-id="762db-268">Exchange 2007 Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="762db-268">Exchange 2007 Service Pack 1 (SP1)</span></span>  <br/> |
|[<span data-ttu-id="762db-269">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="762db-269">GetDelegate operation</span></span>](getdelegate-operation.md) <br/> |<span data-ttu-id="762db-270">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-270">Exchange 2007 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-271">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="762db-271">UpdateDelegate operation</span></span>](updatedelegate-operation.md) <br/> |<span data-ttu-id="762db-272">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-272">Exchange 2007 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-273">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="762db-273">RemoveDelegate operation</span></span>](removedelegate-operation.md) <br/> |<span data-ttu-id="762db-274">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-274">Exchange 2007 SP1</span></span>  <br/> |
   
## <a name="inbox-rules-operations"></a><span data-ttu-id="762db-275">受信トレイルールの操作</span><span class="sxs-lookup"><span data-stu-id="762db-275">Inbox rules operations</span></span>
<span data-ttu-id="762db-276"><a name="bk_inbox_rules"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-276"><a name="bk_inbox_rules"> </a></span></span>

<span data-ttu-id="762db-277">受信トレイルールの操作を使用すると、クライアントは受信トレイルールを取得して、サーバー上のメッセージに対して更新することができます。</span><span class="sxs-lookup"><span data-stu-id="762db-277">The Inbox rules operations enable clients to get Inbox rules and update them for messages on the server.</span></span> <span data-ttu-id="762db-278">受信トレイルールは、メッセージがフォルダーに配信されるときに、クライアントがメッセージを自動的に整理、分類、および処理できるようにする一連の条件と関連付けられたアクションです。</span><span class="sxs-lookup"><span data-stu-id="762db-278">Inbox rules are sets of conditions and associated actions that enable clients to automatically organize, categorize, and act on messages as the messages are delivered to a folder.</span></span> 
  
<span data-ttu-id="762db-279">次の表に、受信トレイルールの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-279">The following table lists the Inbox rules operations.</span></span>
  
|<span data-ttu-id="762db-280">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-280">**Operation name**</span></span>|<span data-ttu-id="762db-281">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-281">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-282">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="762db-282">GetInboxRules operation</span></span>](getinboxrules-operation.md) <br/> |<span data-ttu-id="762db-283">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-283">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-284">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="762db-284">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md) <br/> |<span data-ttu-id="762db-285">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-285">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="mail-app-management-operations"></a><span data-ttu-id="762db-286">メールアプリの管理操作</span><span class="sxs-lookup"><span data-stu-id="762db-286">Mail app management operations</span></span>
<span data-ttu-id="762db-287"><a name="bk_mail_apps"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-287"><a name="bk_mail_apps"> </a></span></span>

<span data-ttu-id="762db-288">メールアプリの管理操作により、Outlook 用メールアプリを管理できます。</span><span class="sxs-lookup"><span data-stu-id="762db-288">The mail app management operations enable you to manage mail apps for Outlook.</span></span> <span data-ttu-id="762db-289">これらの操作は、Outlook Web App および Outlook 2013 で利用可能なメールアプリに関する情報をインストール、アンインストール、無効化、および取得するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="762db-289">You can use these operations to install, uninstall, disable, and get information about mail apps that are available for Outlook Web App and Outlook 2013.</span></span>
  
<span data-ttu-id="762db-290">次の表に、メールアプリの管理操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-290">The following table lists the mail app management operations.</span></span>
  
|<span data-ttu-id="762db-291">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-291">**Operation name**</span></span>|<span data-ttu-id="762db-292">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-292">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-293">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="762db-293">DisableApp operation</span></span>](disableapp-operation.md) <br/> |<span data-ttu-id="762db-294">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-294">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-295">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="762db-295">GetAppManifests operation</span></span>](getappmanifests-operation.md) <br/> |<span data-ttu-id="762db-296">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-296">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-297">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="762db-297">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md) <br/> |<span data-ttu-id="762db-298">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-298">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-299">GetClientAccessToken 操作</span><span class="sxs-lookup"><span data-stu-id="762db-299">GetClientAccessToken operation</span></span>](getclientaccesstoken-operation.md) <br/> |<span data-ttu-id="762db-300">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-300">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-301">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="762db-301">InstallApp operation</span></span>](installapp-operation.md) <br/> |<span data-ttu-id="762db-302">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-302">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-303">アン Installapp 操作</span><span class="sxs-lookup"><span data-stu-id="762db-303">UninstallApp operation</span></span>](uninstallapp-operation.md) <br/> |<span data-ttu-id="762db-304">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-304">Exchange 2013</span></span>  <br/> |
   
## <a name="mail-tips-operation"></a><span data-ttu-id="762db-305">メールヒントの操作</span><span class="sxs-lookup"><span data-stu-id="762db-305">Mail tips operation</span></span>
<span data-ttu-id="762db-306"><a name="bk_mail_tips"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-306"><a name="bk_mail_tips"> </a></span></span>

<span data-ttu-id="762db-307">メールヒント操作を使用すると、作成者がメッセージを作成している場合に、受信者のメールボックスに関する情報をクライアントがサーバーから要求できるようになります。</span><span class="sxs-lookup"><span data-stu-id="762db-307">The mail tips operation enables clients to request information from the server about recipient mailboxes when an author is composing a message.</span></span> <span data-ttu-id="762db-308">次の表に、メールヒント操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-308">The following table lists the mail tips operation.</span></span>
  
|<span data-ttu-id="762db-309">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-309">**Operation name**</span></span>|<span data-ttu-id="762db-310">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-310">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-311">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="762db-311">GetMailTips operation</span></span>](getmailtips-operation.md) <br/> |<span data-ttu-id="762db-312">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-312">Exchange 2010</span></span>  <br/> |
   
## <a name="message-tracking-operations"></a><span data-ttu-id="762db-313">メッセージ追跡操作</span><span class="sxs-lookup"><span data-stu-id="762db-313">Message tracking operations</span></span>
<span data-ttu-id="762db-314"><a name="bk_message_tracking"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-314"><a name="bk_message_tracking"> </a></span></span>

<span data-ttu-id="762db-315">メッセージ追跡操作を使用すると、クライアントは、指定された条件に一致するメッセージを検索し、メッセージ追跡レポート内の各メッセージに関する詳細な追跡情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="762db-315">The message tracking operations enable clients to find messages that meet specified criteria and to get detailed tracking information about each message in a message tracking report.</span></span> 
  
<span data-ttu-id="762db-316">次の表に、メッセージ追跡操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-316">The following table lists the message tracking operations.</span></span>
  
|<span data-ttu-id="762db-317">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-317">**Operation name**</span></span>|<span data-ttu-id="762db-318">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-318">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-319">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="762db-319">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md) <br/> |<span data-ttu-id="762db-320">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-320">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-321">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="762db-321">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) <br/> |<span data-ttu-id="762db-322">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-322">Exchange 2010</span></span>  <br/> |
   
## <a name="notification-operations"></a><span data-ttu-id="762db-323">通知の操作   </span><span class="sxs-lookup"><span data-stu-id="762db-323">Notification operations</span></span>
<span data-ttu-id="762db-324"><a name="bk_notification"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-324"><a name="bk_notification"> </a></span></span>

<span data-ttu-id="762db-325">通知操作は、指定されたメールボックスのアイテムとフォルダーに関連付けられているイベントをクライアントアプリケーションに通知します。</span><span class="sxs-lookup"><span data-stu-id="762db-325">The notification operations notify the client application of events that are associated with items and folders a specified mailbox.</span></span> <span data-ttu-id="762db-326">サブスクリプションモデルは、プッシュベース、プルベース、またはストリーミングベースにすることができます。</span><span class="sxs-lookup"><span data-stu-id="762db-326">The subscription model can be push-based, pull-based, or streaming-based.</span></span> 
  
<span data-ttu-id="762db-327">次の表に、通知操作の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-327">The following table lists the notification operations.</span></span>
  
|<span data-ttu-id="762db-328">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-328">**Operation name**</span></span>|<span data-ttu-id="762db-329">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-329">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-330">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="762db-330">GetEvents operation</span></span>](getevents-operation.md) <br/> |<span data-ttu-id="762db-331">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-331">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-332">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="762db-332">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) <br/> |<span data-ttu-id="762db-333">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="762db-333">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="762db-334">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="762db-334">Subscribe operation</span></span>](subscribe-operation.md) <br/> |<span data-ttu-id="762db-335">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-335">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-336">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="762db-336">Unsubscribe operation</span></span>](unsubscribe-operation.md) <br/> |<span data-ttu-id="762db-337">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-337">Exchange 2007</span></span>  <br/> |
   
## <a name="persona-operations"></a><span data-ttu-id="762db-338">Persona 操作</span><span class="sxs-lookup"><span data-stu-id="762db-338">Persona operations</span></span>
<span data-ttu-id="762db-339"><a name="bk_personas"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-339"><a name="bk_personas"> </a></span></span>

<span data-ttu-id="762db-340">ペルソナ操作は、リンクされた連絡先に関する情報を検索して取得するためのインターフェイスを提供します。</span><span class="sxs-lookup"><span data-stu-id="762db-340">The persona operations provide an interface to find and get information about a linked contact.</span></span> <span data-ttu-id="762db-341">次の表に、ペルソナ操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-341">The following table lists the persona operations.</span></span>
  
|<span data-ttu-id="762db-342">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-342">**Operation name**</span></span>|<span data-ttu-id="762db-343">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-343">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-344">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="762db-344">FindPeople operation</span></span>](findpeople-operation.md) <br/> |<span data-ttu-id="762db-345">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-345">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-346">GetPersona 操作</span><span class="sxs-lookup"><span data-stu-id="762db-346">GetPersona operation</span></span>](getpersona-operation.md) <br/> |<span data-ttu-id="762db-347">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-347">Exchange 2013</span></span>  <br/> |
   
## <a name="retention-policy-operation"></a><span data-ttu-id="762db-348">アイテム保持ポリシーの操作</span><span class="sxs-lookup"><span data-stu-id="762db-348">Retention policy operation</span></span>
<span data-ttu-id="762db-349"><a name="bk_retention_policy"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-349"><a name="bk_retention_policy"> </a></span></span>

<span data-ttu-id="762db-350">[アイテム保持ポリシー] 操作には、ユーザーのアイテム保持ポリシーにリンクされているすべての保持タグの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="762db-350">The retention policy operation provides a list of all the retention tags that are linked to a user's retention policy.</span></span> 
  
<span data-ttu-id="762db-351">次の表に、アイテム保持ポリシーの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-351">The following table lists the retention policy operation.</span></span>
  
|<span data-ttu-id="762db-352">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-352">**Operation name**</span></span>|<span data-ttu-id="762db-353">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-353">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-354">GetUserRetentionPolicyTags 操作</span><span class="sxs-lookup"><span data-stu-id="762db-354">GetUserRetentionPolicyTags operation</span></span>](getuserretentionpolicytags-operation.md) <br/> |<span data-ttu-id="762db-355">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-355">Exchange 2013</span></span>  <br/> |
   
## <a name="service-configuration-operation"></a><span data-ttu-id="762db-356">サービス構成操作</span><span class="sxs-lookup"><span data-stu-id="762db-356">Service configuration operation</span></span>
<span data-ttu-id="762db-357"><a name="bk_service_config"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-357"><a name="bk_service_config"> </a></span></span>

<span data-ttu-id="762db-358">サービス構成操作により、クライアントは、ユニファイドメッセージング、保護ルール、ポリシーヒント、およびメールヒントサービスの構成情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="762db-358">The service configuration operation enables clients to get configuration information for the Unified Messaging, Protection Rules, Policy Tips, and Mail Tips services.</span></span> 
  
<span data-ttu-id="762db-359">次の表に、サービスの構成操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-359">The following table lists the service configuration operation.</span></span>
  
|<span data-ttu-id="762db-360">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-360">**Operation name**</span></span>|<span data-ttu-id="762db-361">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-361">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-362">GetServiceConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-362">GetServiceConfiguration operation</span></span>](getserviceconfiguration-operation.md) <br/> |<span data-ttu-id="762db-363">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-363">Exchange 2010</span></span>  <br/> |
   
## <a name="sharing-operations"></a><span data-ttu-id="762db-364">共有操作</span><span class="sxs-lookup"><span data-stu-id="762db-364">Sharing operations</span></span>
<span data-ttu-id="762db-365"><a name="bk_sharing"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-365"><a name="bk_sharing"> </a></span></span>

<span data-ttu-id="762db-366">共有の操作により、クライアントは予定表データと連絡先データを共有できます。</span><span class="sxs-lookup"><span data-stu-id="762db-366">The sharing operations enable clients to share calendar data and contacts data.</span></span> 
  
<span data-ttu-id="762db-367">次の表に、共有操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-367">The following table lists the sharing operations.</span></span>
  
|<span data-ttu-id="762db-368">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-368">**Operation name**</span></span>|<span data-ttu-id="762db-369">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-369">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-370">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="762db-370">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md) <br/> |<span data-ttu-id="762db-371">Exchange 2010。</span><span class="sxs-lookup"><span data-stu-id="762db-371">Exchange 2010.</span></span> <span data-ttu-id="762db-372">**CreateItem**操作は、すべてのバージョンの EWS に適用できますが、 **acceptsharinginvitation**応答オブジェクトは、exchange 2010 以降のバージョンの exchange の ews にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="762db-372">Although the **CreateItem** operation is applicable to all versions of EWS, the **AcceptSharingInvitation** response object is only applicable to EWS in versions of Exchange starting with Exchange 2010.</span></span>  <br/> |
|[<span data-ttu-id="762db-373">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-373">GetSharingFolder operation</span></span>](getsharingfolder-operation.md) <br/> |<span data-ttu-id="762db-374">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-374">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-375">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="762db-375">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md) <br/> |<span data-ttu-id="762db-376">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-376">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-377">RefreshSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="762db-377">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md) <br/> |<span data-ttu-id="762db-378">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-378">Exchange 2010</span></span>  <br/> |
   
## <a name="synchronization-operations"></a><span data-ttu-id="762db-379">同期操作</span><span class="sxs-lookup"><span data-stu-id="762db-379">Synchronization operations</span></span>
<span data-ttu-id="762db-380"><a name="bk_synchronization"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-380"><a name="bk_synchronization"> </a></span></span>

<span data-ttu-id="762db-381">同期操作では、ユーザーのフォルダーとアイテムの一段階の同期キャッシュコピーが提供されます。</span><span class="sxs-lookup"><span data-stu-id="762db-381">The synchronization operations provide a one-way synchronized cached copy of a user's folders and items.</span></span> 
  
<span data-ttu-id="762db-382">次の表に、同期操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-382">The following table lists the synchronization operations.</span></span>
  
|<span data-ttu-id="762db-383">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-383">**Operation name**</span></span>|<span data-ttu-id="762db-384">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-384">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-385">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="762db-385">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md) <br/> |<span data-ttu-id="762db-386">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-386">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="762db-387">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="762db-387">SyncFolderItems operation</span></span>](syncfolderitems-operation.md) <br/> |<span data-ttu-id="762db-388">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="762db-388">Exchange 2007</span></span>  <br/> |
   
## <a name="time-zone-operation"></a><span data-ttu-id="762db-389">タイムゾーンの操作</span><span class="sxs-lookup"><span data-stu-id="762db-389">Time zone operation</span></span>
<span data-ttu-id="762db-390"><a name="bk_timezone"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-390"><a name="bk_timezone"> </a></span></span>

<span data-ttu-id="762db-391">タイムゾーン操作を使用すると、クライアントはサーバーでサポートされているタイムゾーン定義の一覧を取得できます。</span><span class="sxs-lookup"><span data-stu-id="762db-391">The time zone operation enables clients to get a list of time zone definitions that are supported by the server.</span></span> 
  
<span data-ttu-id="762db-392">次の表に、タイムゾーン操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-392">The following table lists the time zone operation.</span></span>
  
|<span data-ttu-id="762db-393">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-393">**Operation name**</span></span>|<span data-ttu-id="762db-394">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-394">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-395">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="762db-395">GetServerTimeZones operation</span></span>](getservertimezones-operation.md) <br/> |<span data-ttu-id="762db-396">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-396">Exchange 2010</span></span>  <br/> |
   
## <a name="unified-messaging-operations"></a><span data-ttu-id="762db-397">ユニファイドメッセージングの操作</span><span class="sxs-lookup"><span data-stu-id="762db-397">Unified Messaging operations</span></span>
<span data-ttu-id="762db-398"><a name="bk_um"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-398"><a name="bk_um"> </a></span></span>

<span data-ttu-id="762db-399">ユニファイドメッセージングの操作により、クライアントは、ユニファイドメッセージングのプロパティに関する情報を読み取って、電話でボイスメールメッセージを再生することができます。</span><span class="sxs-lookup"><span data-stu-id="762db-399">The Unified Messaging operations enable clients to read information about Unified Messaging properties and to play voice mail messages over the phone.</span></span> 
  
<span data-ttu-id="762db-400">次の表に、ユニファイドメッセージングの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-400">The following table lists the Unified Messaging operations.</span></span>
  
|<span data-ttu-id="762db-401">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-401">**Operation name**</span></span>|<span data-ttu-id="762db-402">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-402">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-403">切断電話操作</span><span class="sxs-lookup"><span data-stu-id="762db-403">DisconnectPhoneCall operation</span></span>](disconnectphonecall-operation.md) <br/> |<span data-ttu-id="762db-404">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-404">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-405">GetPhoneCallInformation 操作</span><span class="sxs-lookup"><span data-stu-id="762db-405">GetPhoneCallInformation operation</span></span>](getphonecallinformation-operation.md) <br/> |<span data-ttu-id="762db-406">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-406">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-407">PlayOnPhone 操作 (EWS)</span><span class="sxs-lookup"><span data-stu-id="762db-407">PlayOnPhone operation (EWS)</span></span>](playonphone-operation-ews.md) <br/> |<span data-ttu-id="762db-408">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-408">Exchange 2010</span></span>  <br/> |
   
<span data-ttu-id="762db-409">[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)を使用して、メールボックスのユニファイドメッセージング構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="762db-409">Use the [GetServiceConfiguration operation](getserviceconfiguration-operation.md) to get the Unified Messaging configuration information for a mailbox.</span></span> <span data-ttu-id="762db-410">ユニファイドメッセージング web サービスは、Exchange 2007 を対象としたユニファイドメッセージングアプリケーションに対して使用します。</span><span class="sxs-lookup"><span data-stu-id="762db-410">Use the Unified Messaging web service for Unified Messaging applications that target Exchange 2007.</span></span> <span data-ttu-id="762db-411">詳細については、「[ユニファイドメッセージング web サービスリファレンス (Exchange](unified-messaging-web-service-reference-for-exchange.md))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="762db-411">For more information, see [Unified Messaging web service reference for Exchange](unified-messaging-web-service-reference-for-exchange.md).</span></span>
  
## <a name="unified-contact-store-operations"></a><span data-ttu-id="762db-412">統合連絡先ストアの操作</span><span class="sxs-lookup"><span data-stu-id="762db-412">Unified Contact Store operations</span></span>
<span data-ttu-id="762db-413"><a name="bk_ucs"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-413"><a name="bk_ucs"> </a></span></span>

<span data-ttu-id="762db-414">統合連絡先ストアは、Office 製品間で一貫した連絡先環境を提供し、サードパーティアプリケーションが同じ連絡先ストアを使用するための統合ポイントとして機能します。</span><span class="sxs-lookup"><span data-stu-id="762db-414">The Unified Contact Store provides a consistent contact experience across Office products and acts as an integration point for third-party applications to use the same contact store.</span></span> <span data-ttu-id="762db-415">これにより、ユーザーとアプリケーションは、連絡先情報を格納、管理、およびアクセスして、Lync、Exchange 2013、Outlook、Outlook Web App、および統合連絡先ストアへのアクセスを実装するその他のアプリケーション間でグローバルに利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="762db-415">It enables users and applications to store, manage, and access contact information and make it available globally among Lync, Exchange 2013, Outlook, Outlook Web App, and any other application that implements access to the Unified Contact Store.</span></span> <span data-ttu-id="762db-416">Exchange は、統合連絡先ストアの機能のコンテンツストアです。</span><span class="sxs-lookup"><span data-stu-id="762db-416">Exchange is the content store for the Unified Contact Store experience.</span></span>
  
<span data-ttu-id="762db-417">次の表に、統合連絡先ストアの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-417">The following table lists the Unified Contact Store operations.</span></span>
  
|<span data-ttu-id="762db-418">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-418">**Operation name**</span></span>|<span data-ttu-id="762db-419">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-419">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-420">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-420">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md) <br/> |<span data-ttu-id="762db-421">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-421">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-422">AddImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-422">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md) <br/> |<span data-ttu-id="762db-423">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-423">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-424">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-424">AddImGroup operation</span></span>](addimgroup-operation.md) <br/> |<span data-ttu-id="762db-425">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-425">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-426">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-426">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md) <br/> |<span data-ttu-id="762db-427">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-427">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-428">Adddeploy Grouptoimlist 操作</span><span class="sxs-lookup"><span data-stu-id="762db-428">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md) <br/> |<span data-ttu-id="762db-429">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-429">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-430">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="762db-430">GetImItemList operation</span></span>](getimitemlist-operation.md) <br/> |<span data-ttu-id="762db-431">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-431">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-432">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="762db-432">GetImItems operation</span></span>](getimitems-operation.md) <br/> |<span data-ttu-id="762db-433">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-433">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-434">RemoveContactFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="762db-434">RemoveContactFromImList operation</span></span>](removecontactfromimlist-operation.md) <br/> |<span data-ttu-id="762db-435">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-435">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-436">RemoveImContactFromGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-436">RemoveImContactFromGroup operation</span></span>](removeimcontactfromgroup-operation.md) <br/> |<span data-ttu-id="762db-437">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-437">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-438">RemoveDistributionGroupFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="762db-438">RemoveDistributionGroupFromImList operation</span></span>](removedistributiongroupfromimlist-operation.md) <br/> |<span data-ttu-id="762db-439">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-439">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-440">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-440">RemoveImGroup operation</span></span>](removeimgroup-operation.md) <br/> |<span data-ttu-id="762db-441">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-441">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="762db-442">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="762db-442">SetImGroup operation</span></span>](setimgroup-operation.md) <br/> |<span data-ttu-id="762db-443">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="762db-443">Exchange 2013</span></span>  <br/> |
   
## <a name="user-configuration-operations"></a><span data-ttu-id="762db-444">ユーザー構成操作</span><span class="sxs-lookup"><span data-stu-id="762db-444">User configuration operations</span></span>
<span data-ttu-id="762db-445"><a name="bk_user_config"> </a></span><span class="sxs-lookup"><span data-stu-id="762db-445"><a name="bk_user_config"> </a></span></span>

<span data-ttu-id="762db-446">ユーザー構成操作は、クライアントがユーザー構成情報を作成、削除、取得、更新できるようにします。</span><span class="sxs-lookup"><span data-stu-id="762db-446">The user configuration operations enable clients to create, delete, get, and update user configuration information.</span></span> 
  
<span data-ttu-id="762db-447">次の表に、ユーザーの構成操作を示します。</span><span class="sxs-lookup"><span data-stu-id="762db-447">The following table lists the user configuration operations.</span></span>
  
|<span data-ttu-id="762db-448">**操作名**</span><span class="sxs-lookup"><span data-stu-id="762db-448">**Operation name**</span></span>|<span data-ttu-id="762db-449">**導入バージョン**</span><span class="sxs-lookup"><span data-stu-id="762db-449">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="762db-450">CreateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-450">CreateUserConfiguration operation</span></span>](createuserconfiguration-operation.md) <br/> |<span data-ttu-id="762db-451">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-451">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-452">DeleteUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-452">DeleteUserConfiguration operation</span></span>](deleteuserconfiguration-operation.md) <br/> |<span data-ttu-id="762db-453">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-453">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-454">GetUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-454">GetUserConfiguration operation</span></span>](getuserconfiguration-operation.md) <br/> |<span data-ttu-id="762db-455">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-455">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="762db-456">UpdateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="762db-456">UpdateUserConfiguration operation</span></span>](updateuserconfiguration-operation.md) <br/> |<span data-ttu-id="762db-457">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="762db-457">Exchange 2010</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="762db-458">関連項目</span><span class="sxs-lookup"><span data-stu-id="762db-458">See also</span></span>

- [<span data-ttu-id="762db-459">Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ</span><span class="sxs-lookup"><span data-stu-id="762db-459">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="762db-460">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="762db-460">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="762db-461">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="762db-461">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

