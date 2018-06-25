---
title: Exchange での EWS の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: cf6fd871-9a65-4f34-8557-c8c71dd7ce09
description: Exchange で使用できる EWS 操作に関する情報を検索します。
ms.openlocfilehash: c56c3be746138cec251836fcb61ee3738d168869
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760366"
---
# <a name="ews-operations-in-exchange"></a><span data-ttu-id="75cb5-103">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-103">EWS operations in Exchange</span></span>

<span data-ttu-id="75cb5-104">Exchange で使用できる EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-104">Find information about the EWS operations that are available in Exchange.</span></span>
  
<span data-ttu-id="75cb5-105">Exchange Web サービス (EWS) は、Exchange ストアからの情報にアクセスできるようにする多くの操作を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-105">Exchange Web Services (EWS) provides many operations that enable you to access information from the Exchange store.</span></span> <span data-ttu-id="75cb5-106">このセクションの記事では、要求、応答、および各操作のための XML の例だけでなく、EWS の操作、エラーの応答メッセージの全体的な構造に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-106">The articles in this section provide information about the overall structure of the requests, responses, and error response messages for EWS operations, as well as XML examples for each operation.</span></span> <span data-ttu-id="75cb5-107">クライアントとサーバー間で送信されるメッセージの構造の概要を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-107">They provide an overview of the message structures that are sent between the client and the server.</span></span> <span data-ttu-id="75cb5-108">メッセージ構造体をデバッグして、EWS の要求で行うことができます詳細を確認するには、この情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-108">You can use this information to debug message structures and to find information about what you can do in an EWS request.</span></span> <span data-ttu-id="75cb5-109">詳細についてはどのような XML 構造は、 [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75cb5-109">For more information about what the XML structure represents, see - [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md).</span></span>
  
<span data-ttu-id="75cb5-110">EWS のすべての機能は、スキーマのバージョンに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-110">All EWS functionality is associated with a version of the schema.</span></span> <span data-ttu-id="75cb5-111">新しい EWS のスキーマ バージョンは、Exchange Server または Exchange Online の新しいリリースで導入されます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-111">New EWS schema versions are introduced in new releases of Exchange Server or Exchange Online.</span></span> <span data-ttu-id="75cb5-112">[RequestServerVersion](requestserverversion.md)要素には、スキーマのバージョンをサーバー バージョンにマップする**バージョン**の属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="75cb5-112">The [RequestServerVersion](requestserverversion.md) element contains a **Version** attribute that maps the server version to the schema version.</span></span> <span data-ttu-id="75cb5-113">この資料では、各操作が導入されたに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-113">This article provides information about when each operation was introduced.</span></span> <span data-ttu-id="75cb5-114">操作内の特定の機能には、サービスの新しいバージョンを必要があります。</span><span class="sxs-lookup"><span data-stu-id="75cb5-114">Specific functionality within an operation might require a later version of the service.</span></span> <span data-ttu-id="75cb5-115">バージョン管理されたスキーマは、EWS の以前のバージョンを対象に設計されたクライアントが EWS の新しいバージョンで動作するように実装されます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-115">The versioned schemas are implemented so that clients that are designed against an older version of EWS will work with a newer version of EWS.</span></span> 
  
<span data-ttu-id="75cb5-116">EWS エンドポイント、メールボックスを処理するこれらの操作対象にできます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-116">These operations can target the EWS endpoint that services your mailbox.</span></span> <span data-ttu-id="75cb5-117">Http:// 構造体に次のような URL を使用して、EWS のエンドポイントを参照する<clientaccessserver>.com/ews/exchange.asmx、<clientaccessserver>は、Exchange クライアント アクセス サーバー、メールボックスを処理します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-117">You can browse to the EWS endpoint by using a URL that is similar in structure to http://<clientaccessserver>.com/ews/exchange.asmx, where <clientaccessserver> is the Exchange Client Access server that services your mailbox.</span></span> <span data-ttu-id="75cb5-118">自動検出を使用すると、メールボックスを処理するクライアント アクセス サーバーへの URL を取得します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-118">You can use Autodiscover to get the URL to the Client Access server that services your mailbox.</span></span> <span data-ttu-id="75cb5-119">自動検出の詳細については、 [Exchange の自動検出](../exchange-web-services/autodiscover-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75cb5-119">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="75cb5-120">電子情報開示の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-120">eDiscovery operations</span></span>
<span data-ttu-id="75cb5-121"><a name="bk_eDiscovery"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-121"></span></span>

<span data-ttu-id="75cb5-122">電子的証拠開示の操作では、法的保存の検索操作を提供し、メールボックスのデータをインデックス化し、検索の検索結果で返されることはできませんを識別します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-122">The eDiscovery operations provide search operations for legal holds and identify mailbox data that cannot be indexed and returned in discovery search results.</span></span>
  
<span data-ttu-id="75cb5-123">次の表は、電子的証拠開示の操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-123">The following table lists the eDiscovery operations.</span></span>
  
|<span data-ttu-id="75cb5-124">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-124">**Operation name**</span></span>|<span data-ttu-id="75cb5-125">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-125">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-126">GetDiscoverySearchConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-126">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-127">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-127">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-128">GetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-128">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md) <br/> |<span data-ttu-id="75cb5-129">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-129">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-130">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-130">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md) <br/> |<span data-ttu-id="75cb5-131">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-131">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-132">GetNonIndexableItemStatistics 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-132">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md) <br/> |<span data-ttu-id="75cb5-133">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-133">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-134">GetSearchableMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-134">GetSearchableMailboxes operation</span></span>](getsearchablemailboxes-operation.md) <br/> |<span data-ttu-id="75cb5-135">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-135">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-136">SearchMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-136">SearchMailboxes operation</span></span>](searchmailboxes-operation.md) <br/> |<span data-ttu-id="75cb5-137">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-137">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-138">SetHoldOnMailboxes 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-138">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md) <br/> |<span data-ttu-id="75cb5-139">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-139">Exchange 2013</span></span>  <br/> |
   
## <a name="exchange-mailbox-data-operations"></a><span data-ttu-id="75cb5-140">Exchange のメールボックス データの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-140">Exchange mailbox data operations</span></span>
<span data-ttu-id="75cb5-141"><a name="bk_Exchange_mailbox_data"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-141"></span></span>

<span data-ttu-id="75cb5-142">Exchange のメールボックス データの操作は、クライアントを処理し、あいまいな名前解決、配布リストの展開に加え、アイテム、フォルダー、および添付ファイルを整理するを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-142">The Exchange mailbox data operations enable clients to handle and organize items, folders, and attachments, as well as ambiguous name resolution and distribution list expansion.</span></span> <span data-ttu-id="75cb5-143">Exchange のメールボックス データの操作には、アイテム、フォルダー、添付ファイル、およびユーティリティの操作が含まれます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-143">Exchange mailbox data operations include item, folder, attachment, and utilities operations.</span></span>
  
<span data-ttu-id="75cb5-144">次の表は、Exchange のメールボックス データの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-144">The following table lists the Exchange mailbox data operations.</span></span>
  
|<span data-ttu-id="75cb5-145">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-145">**Operation name**</span></span>|<span data-ttu-id="75cb5-146">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-146">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-147">ArchiveItem 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-147">ArchiveItem operation</span></span>](archiveitem-operation.md) <br/> |<span data-ttu-id="75cb5-148">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-148">Exchange 2013</span></span>  <br/> |
|<span data-ttu-id="75cb5-149">
  [CreateItem 操作](createitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-149">[CreateItem operation](createitem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-150">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-150">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-151">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-151">[CopyItem operation](copyitem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-152">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-152">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-153">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-153">DeleteItem operation</span></span>](deleteitem-operation.md) <br/> |<span data-ttu-id="75cb5-154">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-154">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-155">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-155">[FindItem operation](finditem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-156">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-156">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-157">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-157">[GetItem operation](getitem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-158">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-158">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-159">MarkAllItemsAsRead 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-159">MarkAllItemsAsRead operation</span></span>](markallitemsasread-operation.md) <br/> |<span data-ttu-id="75cb5-160">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-160">Exchange 2013</span></span>  <br/> |
|<span data-ttu-id="75cb5-161">
  [MoveItem 操作](moveitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-161">[MoveItem operation](moveitem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-162">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-162">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-163">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-163">[SendItem operation](senditem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-164">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-164">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-165">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-165">[UpdateItem operation](updateitem-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-166">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-166">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="75cb5-167">次の表は、Exchange メールボックスのデータ フォルダーの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-167">The following table lists the Exchange mailbox data folder operations.</span></span>
  
|<span data-ttu-id="75cb5-168">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-168">**Operation name**</span></span>|<span data-ttu-id="75cb5-169">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-169">**Introduced in**</span></span>|
|:-----|:-----|
|<span data-ttu-id="75cb5-170">
  [CreateFolder 操作](createfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-170">[CreateFolder operation](createfolder-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-171">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-171">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-172">CreateFolderPath 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-172">CreateFolderPath operation</span></span>](createfolderpath-operation.md) <br/> |<span data-ttu-id="75cb5-173">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-173">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-174">CreateManagedFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-174">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md) <br/> |<span data-ttu-id="75cb5-175">Exchange 2007。</span><span class="sxs-lookup"><span data-stu-id="75cb5-175">Exchange 2007.</span></span> <span data-ttu-id="75cb5-176">この機能はバージョンの Exchange が Exchange 2010 で始まる deemphasized されています。</span><span class="sxs-lookup"><span data-stu-id="75cb5-176">This functionality has been deemphasized in versions of Exchange starting with Exchange 2010.</span></span> <span data-ttu-id="75cb5-177">メッセージング レコード管理用のタグを保存し、ポリシーを使用して移行する方法の詳細については、[管理対象フォルダーからの移行](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.141%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75cb5-177">For more information about how to migrate to using retention tags and policies for messaging records management, see [Migrate from Managed Folders](http://technet.microsoft.com/en-us/library/dd298032%28v=exchg.141%29.aspx).</span></span>  <br/> |
|[<span data-ttu-id="75cb5-178">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-178">CopyFolder operation</span></span>](copyfolder-operation.md) <br/> |<span data-ttu-id="75cb5-179">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-179">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-180">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-180">DeleteFolder operation</span></span>](deletefolder-operation.md) <br/> |<span data-ttu-id="75cb5-181">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-181">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-182">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-182">EmptyFolder operation</span></span>](emptyfolder-operation.md) <br/> |<span data-ttu-id="75cb5-183">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-183">Exchange 2010</span></span>  <br/> |
|<span data-ttu-id="75cb5-184">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-184">[FindFolder operation](findfolder-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-185">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-185">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-186">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-186">[GetFolder operation](getfolder-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-187">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-187">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-188">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-188">MoveFolder operation</span></span>](movefolder-operation.md) <br/> |<span data-ttu-id="75cb5-189">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-189">Exchange 2007</span></span>  <br/> |
|<span data-ttu-id="75cb5-190">
  [UpdateFolder 操作](updatefolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-190">[UpdateFolder operation](updatefolder-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-191">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-191">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="75cb5-192">次の表は、Exchange メールボックスのデータの添付ファイルの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-192">The following table lists the Exchange mailbox data attachment operations.</span></span>
  
|<span data-ttu-id="75cb5-193">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-193">**Operation name**</span></span>|<span data-ttu-id="75cb5-194">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-194">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-195">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-195">CreateAttachment operation</span></span>](createattachment-operation.md) <br/> |<span data-ttu-id="75cb5-196">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-196">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-197">GetAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-197">GetAttachment operation</span></span>](getattachment-operation.md) <br/> |<span data-ttu-id="75cb5-198">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-198">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-199">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-199">DeleteAttachment operation</span></span>](deleteattachment-operation.md) <br/> |<span data-ttu-id="75cb5-200">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-200">Exchange 2007</span></span>  <br/> |
   
<span data-ttu-id="75cb5-201">次の表に、Exchange メールボックスのアラームの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-201">The following table lists the Exchange mailbox reminder operations.</span></span>
  
|<span data-ttu-id="75cb5-202">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-202">**Operation name**</span></span>|<span data-ttu-id="75cb5-203">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-203">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-204">GetReminders 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-204">GetReminders operation</span></span>](getreminders-operation.md) <br/> |<span data-ttu-id="75cb5-205">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-205">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-206">PerformReminderAction 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-206">PerformReminderAction operation</span></span>](performreminderaction-operation.md) <br/> |<span data-ttu-id="75cb5-207">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-207">Exchange 2013</span></span>  <br/> |
   
<span data-ttu-id="75cb5-208">次の表に、Exchange メールボックス データの対話操作を示します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-208">The following table lists the Exchange mailbox data conversation operations.</span></span>
  
|<span data-ttu-id="75cb5-209">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-209">**Operation name**</span></span>|<span data-ttu-id="75cb5-210">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-210">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-211">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-211">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md) <br/> |<span data-ttu-id="75cb5-212">Exchange 2010 Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="75cb5-212">Exchange 2010 Service Pack 1 (SP1)</span></span>  <br/> |
|<span data-ttu-id="75cb5-213">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-213">[FindConversation operation](findconversation-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-214">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-214">Exchange 2010 SP1</span></span>  <br/> |
|<span data-ttu-id="75cb5-215">
  [GetConversationItems 操作](getconversationitems-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75cb5-215">[GetConversationItems operation](getconversationitems-operation.md)</span></span> <br/> |<span data-ttu-id="75cb5-216">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-216">Exchange 2013</span></span>  <br/> |
   
<span data-ttu-id="75cb5-217">次の表は、Exchange のメールボックス データ ユーティリティの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-217">The following table lists the Exchange mailbox data utilities operations.</span></span>
  
|<span data-ttu-id="75cb5-218">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-218">**Operation name**</span></span>|<span data-ttu-id="75cb5-219">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-219">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-220">ConvertId 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-220">ConvertId operation</span></span>](convertid-operation.md) <br/> |<span data-ttu-id="75cb5-221">Exchange 2007 Service Pack 1</span><span class="sxs-lookup"><span data-stu-id="75cb5-221">Exchange 2007 Service Pack 1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-222">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-222">ExpandDL operation</span></span>](expanddl-operation.md) <br/> |<span data-ttu-id="75cb5-223">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-223">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-224">GetUserPhoto 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-224">GetUserPhoto operation</span></span>](getuserphoto-operation.md) <br/> |<span data-ttu-id="75cb5-225">Exchange 2013。</span><span class="sxs-lookup"><span data-stu-id="75cb5-225">Exchange 2013.</span></span> <span data-ttu-id="75cb5-226">この操作では、残りの部分と SOAP の実装の両方があります。</span><span class="sxs-lookup"><span data-stu-id="75cb5-226">This operation has both a REST and a SOAP implementation.</span></span>  <br/> |
|[<span data-ttu-id="75cb5-227">MarkAsJunk の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-227">MarkAsJunk operation</span></span>](markasjunk-operation.md) <br/> |<span data-ttu-id="75cb5-228">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-228">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-229">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-229">ResolveNames operation</span></span>](resolvenames-operation.md) <br/> |<span data-ttu-id="75cb5-230">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-230">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-231">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-231">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md) <br/> |<span data-ttu-id="75cb5-232">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-232">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="availability-operations"></a><span data-ttu-id="75cb5-233">可用性の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-233">Availability operations</span></span>
<span data-ttu-id="75cb5-234"><a name="bk_Availability"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-234"></span></span>

<span data-ttu-id="75cb5-235">予定表と空き時間情報より最新の状態で、豊富なセキュリティで保護された空き時間情報を提供することで経験を共有する、可用性の操作が向上します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-235">The availability operations improve the calendar and free/busy sharing experience by providing more secure, up-to-date, and rich free/busy information.</span></span> <span data-ttu-id="75cb5-236">空き時間情報データは、会議をスケジュールすることの重要なコンポーネントです。</span><span class="sxs-lookup"><span data-stu-id="75cb5-236">Free/busy data is a critical component of scheduling meetings.</span></span> <span data-ttu-id="75cb5-237">可用性の操作では、効果的なスケジュールに関する信頼性の高い基盤を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-237">The availability operations provide a reliable foundation for effective scheduling.</span></span> 
  
<span data-ttu-id="75cb5-238">次の表は、可用性の操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-238">The following table lists the availability operations.</span></span>
  
|<span data-ttu-id="75cb5-239">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-239">**Operation name**</span></span>|<span data-ttu-id="75cb5-240">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-240">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-241">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-241">GetUserAvailability operation</span></span>](getuseravailability-operation.md) <br/> |<span data-ttu-id="75cb5-242">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-242">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-243">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-243">GetRoomLists operation</span></span>](getroomlists-operation.md) <br/> |<span data-ttu-id="75cb5-244">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-244">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-245">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-245">GetRooms operation</span></span>](getrooms-operation.md) <br/> |<span data-ttu-id="75cb5-246">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-246">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-247">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-247">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) <br/> |<span data-ttu-id="75cb5-248">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-248">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-249">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-249">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md) <br/> |<span data-ttu-id="75cb5-250">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-250">Exchange 2007</span></span>  <br/> |
   
## <a name="bulk-transfer-operations"></a><span data-ttu-id="75cb5-251">一括転送操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-251">Bulk transfer operations</span></span>
<span data-ttu-id="75cb5-252"><a name="bk_bulk_transfer"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-252"></span></span>

<span data-ttu-id="75cb5-253">一括転送操作は、メールボックスとの間にクライアントがストリームの項目を有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-253">The bulk transfer operations enable clients to stream items into and out of a mailbox.</span></span> 
  
<span data-ttu-id="75cb5-254">次の表は、バルク転送の操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-254">The following table lists the bulk transfer operations.</span></span>
  
|<span data-ttu-id="75cb5-255">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-255">**Operation name**</span></span>|<span data-ttu-id="75cb5-256">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-256">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-257">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-257">UploadItems operation</span></span>](uploaditems-operation.md) <br/> |<span data-ttu-id="75cb5-258">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-258">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-259">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-259">ExportItems operation</span></span>](exportitems-operation.md) <br/> |<span data-ttu-id="75cb5-260">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-260">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="delegate-management-operations"></a><span data-ttu-id="75cb5-261">管理作業を委任します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-261">Delegate management operations</span></span>
<span data-ttu-id="75cb5-262"><a name="bk_delegate_management"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-262"></span></span>

<span data-ttu-id="75cb5-263">代理人の管理操作は、追加、取得、更新、クライアントを有効にし、自分のメールボックスからデリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-263">The delegate management operations enable clients to add, get, update, and remove delegates from their mailboxes.</span></span> 
  
<span data-ttu-id="75cb5-264">次の表に、代理人の管理操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-264">The following table lists the delegate management operations.</span></span>
  
|<span data-ttu-id="75cb5-265">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-265">**Operation name**</span></span>|<span data-ttu-id="75cb5-266">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-266">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-267">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-267">AddDelegate operation</span></span>](adddelegate-operation.md) <br/> |<span data-ttu-id="75cb5-268">Exchange 2007 Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="75cb5-268">Exchange 2007 Service Pack 1 (SP1)</span></span>  <br/> |
|[<span data-ttu-id="75cb5-269">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-269">GetDelegate operation</span></span>](getdelegate-operation.md) <br/> |<span data-ttu-id="75cb5-270">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-270">Exchange 2007 SP1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-271">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-271">UpdateDelegate operation</span></span>](updatedelegate-operation.md) <br/> |<span data-ttu-id="75cb5-272">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-272">Exchange 2007 SP1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-273">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-273">RemoveDelegate operation</span></span>](removedelegate-operation.md) <br/> |<span data-ttu-id="75cb5-274">Exchange 2007 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-274">Exchange 2007 SP1</span></span>  <br/> |
   
## <a name="inbox-rules-operations"></a><span data-ttu-id="75cb5-275">受信トレイ ルールの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-275">Inbox rules operations</span></span>
<span data-ttu-id="75cb5-276"><a name="bk_inbox_rules"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-276"></span></span>

<span data-ttu-id="75cb5-277">受信トレイ ルールの操作は、クライアントが受信トレイ ルールを取得し、サーバー上のメッセージの更新を有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-277">The Inbox rules operations enable clients to get Inbox rules and update them for messages on the server.</span></span> <span data-ttu-id="75cb5-278">受信トレイ ルールは、条件およびクライアントが自動的に整理、分類、およびフォルダーにメッセージが配信されると同時に、メッセージの機能を有効にするに関連付けられているアクションのセットです。</span><span class="sxs-lookup"><span data-stu-id="75cb5-278">Inbox rules are sets of conditions and associated actions that enable clients to automatically organize, categorize, and act on messages as the messages are delivered to a folder.</span></span> 
  
<span data-ttu-id="75cb5-279">次の表に、受信トレイ ルールの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-279">The following table lists the Inbox rules operations.</span></span>
  
|<span data-ttu-id="75cb5-280">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-280">**Operation name**</span></span>|<span data-ttu-id="75cb5-281">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-281">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-282">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-282">GetInboxRules operation</span></span>](getinboxrules-operation.md) <br/> |<span data-ttu-id="75cb5-283">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-283">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-284">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-284">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md) <br/> |<span data-ttu-id="75cb5-285">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-285">Exchange 2010 SP1</span></span>  <br/> |
   
## <a name="mail-app-management-operations"></a><span data-ttu-id="75cb5-286">メール アプリケーションの管理</span><span class="sxs-lookup"><span data-stu-id="75cb5-286">Mail app management operations</span></span>
<span data-ttu-id="75cb5-287"><a name="bk_mail_apps"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-287"></span></span>

<span data-ttu-id="75cb5-288">メール アプリケーションの管理操作を使用すると、Outlook のメール アプリケーションを管理できます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-288">The mail app management operations enable you to manage mail apps for Outlook.</span></span> <span data-ttu-id="75cb5-289">インストール、アンインストール、無効にするには、これらの操作を使用して Outlook Web App および Outlook 2013 で使用可能なメール ・ アプリケーションに関する情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-289">You can use these operations to install, uninstall, disable, and get information about mail apps that are available for Outlook Web App and Outlook 2013.</span></span>
  
<span data-ttu-id="75cb5-290">メール アプリケーションの管理操作を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-290">The following table lists the mail app management operations.</span></span>
  
|<span data-ttu-id="75cb5-291">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-291">**Operation name**</span></span>|<span data-ttu-id="75cb5-292">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-292">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-293">DisableApp 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-293">DisableApp operation</span></span>](disableapp-operation.md) <br/> |<span data-ttu-id="75cb5-294">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-294">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-295">GetAppManifests 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-295">GetAppManifests operation</span></span>](getappmanifests-operation.md) <br/> |<span data-ttu-id="75cb5-296">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-296">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-297">GetAppMarketplaceUrl 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-297">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md) <br/> |<span data-ttu-id="75cb5-298">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-298">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-299">GetClientAccessToken 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-299">GetClientAccessToken operation</span></span>](getclientaccesstoken-operation.md) <br/> |<span data-ttu-id="75cb5-300">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-300">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-301">InstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-301">InstallApp operation</span></span>](installapp-operation.md) <br/> |<span data-ttu-id="75cb5-302">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-302">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-303">UninstallApp 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-303">UninstallApp operation</span></span>](uninstallapp-operation.md) <br/> |<span data-ttu-id="75cb5-304">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-304">Exchange 2013</span></span>  <br/> |
   
## <a name="mail-tips-operation"></a><span data-ttu-id="75cb5-305">メール ヒントの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-305">Mail tips operation</span></span>
<span data-ttu-id="75cb5-306"><a name="bk_mail_tips"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-306"></span></span>

<span data-ttu-id="75cb5-307">メール ヒントの操作は、作成者がメッセージを作成するときに受信者のメールボックスのサーバーから情報を要求するクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-307">The mail tips operation enables clients to request information from the server about recipient mailboxes when an author is composing a message.</span></span> <span data-ttu-id="75cb5-308">次の表に、メール ヒントの操作を示します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-308">The following table lists the mail tips operation.</span></span>
  
|<span data-ttu-id="75cb5-309">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-309">**Operation name**</span></span>|<span data-ttu-id="75cb5-310">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-310">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-311">GetMailTips 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-311">GetMailTips operation</span></span>](getmailtips-operation.md) <br/> |<span data-ttu-id="75cb5-312">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-312">Exchange 2010</span></span>  <br/> |
   
## <a name="message-tracking-operations"></a><span data-ttu-id="75cb5-313">メッセージ追跡の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-313">Message tracking operations</span></span>
<span data-ttu-id="75cb5-314"><a name="bk_message_tracking"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-314"></span></span>

<span data-ttu-id="75cb5-315">メッセージ追跡操作は、指定条件を満たすメッセージを検索して、メッセージ ・ トラッキング ・ レポート内の各メッセージについての詳細な追跡情報を取得するクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-315">The message tracking operations enable clients to find messages that meet specified criteria and to get detailed tracking information about each message in a message tracking report.</span></span> 
  
<span data-ttu-id="75cb5-316">次の表は、メッセージの操作を追跡します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-316">The following table lists the message tracking operations.</span></span>
  
|<span data-ttu-id="75cb5-317">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-317">**Operation name**</span></span>|<span data-ttu-id="75cb5-318">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-318">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-319">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-319">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md) <br/> |<span data-ttu-id="75cb5-320">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-320">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-321">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-321">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md) <br/> |<span data-ttu-id="75cb5-322">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-322">Exchange 2010</span></span>  <br/> |
   
## <a name="notification-operations"></a><span data-ttu-id="75cb5-323">通知の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-323">Notification operations</span></span>
<span data-ttu-id="75cb5-324"><a name="bk_notification"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-324"></span></span>

<span data-ttu-id="75cb5-325">通知の操作は、指定されたメールボックス アイテムおよびフォルダーに関連付けられているイベントのクライアント アプリケーションを通知します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-325">The notification operations notify the client application of events that are associated with items and folders a specified mailbox.</span></span> <span data-ttu-id="75cb5-326">プッシュ、プル ベース、またはストリーム ベースのサブスクリプション モデルができます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-326">The subscription model can be push-based, pull-based, or streaming-based.</span></span> 
  
<span data-ttu-id="75cb5-327">次の表は、通知の操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-327">The following table lists the notification operations.</span></span>
  
|<span data-ttu-id="75cb5-328">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-328">**Operation name**</span></span>|<span data-ttu-id="75cb5-329">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-329">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-330">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-330">GetEvents operation</span></span>](getevents-operation.md) <br/> |<span data-ttu-id="75cb5-331">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-331">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-332">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-332">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) <br/> |<span data-ttu-id="75cb5-333">Exchange 2010 SP1</span><span class="sxs-lookup"><span data-stu-id="75cb5-333">Exchange 2010 SP1</span></span>  <br/> |
|[<span data-ttu-id="75cb5-334">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-334">Subscribe operation</span></span>](subscribe-operation.md) <br/> |<span data-ttu-id="75cb5-335">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-335">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-336">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-336">Unsubscribe operation</span></span>](unsubscribe-operation.md) <br/> |<span data-ttu-id="75cb5-337">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-337">Exchange 2007</span></span>  <br/> |
   
## <a name="persona-operations"></a><span data-ttu-id="75cb5-338">ペルソナの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-338">Persona operations</span></span>
<span data-ttu-id="75cb5-339"><a name="bk_personas"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-339"></span></span>

<span data-ttu-id="75cb5-340">ペルソナの操作は、検索し、リンクされた取引先担当者に関する情報を取得するためのインターフェイスを提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-340">The persona operations provide an interface to find and get information about a linked contact.</span></span> <span data-ttu-id="75cb5-341">次の表は、ペルソナの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-341">The following table lists the persona operations.</span></span>
  
|<span data-ttu-id="75cb5-342">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-342">**Operation name**</span></span>|<span data-ttu-id="75cb5-343">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-343">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-344">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-344">FindPeople operation</span></span>](findpeople-operation.md) <br/> |<span data-ttu-id="75cb5-345">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-345">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-346">GetPersona 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-346">GetPersona operation</span></span>](getpersona-operation.md) <br/> |<span data-ttu-id="75cb5-347">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-347">Exchange 2013</span></span>  <br/> |
   
## <a name="retention-policy-operation"></a><span data-ttu-id="75cb5-348">保持ポリシーの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-348">Retention policy operation</span></span>
<span data-ttu-id="75cb5-349"><a name="bk_retention_policy"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-349"></span></span>

<span data-ttu-id="75cb5-350">保持ポリシーの操作には、ユーザーのアイテム保持ポリシーにリンクされているすべての保持タグの一覧が用意されています。</span><span class="sxs-lookup"><span data-stu-id="75cb5-350">The retention policy operation provides a list of all the retention tags that are linked to a user's retention policy.</span></span> 
  
<span data-ttu-id="75cb5-351">次の表に、保持ポリシーの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-351">The following table lists the retention policy operation.</span></span>
  
|<span data-ttu-id="75cb5-352">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-352">**Operation name**</span></span>|<span data-ttu-id="75cb5-353">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-353">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-354">GetUserRetentionPolicyTags 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-354">GetUserRetentionPolicyTags operation</span></span>](getuserretentionpolicytags-operation.md) <br/> |<span data-ttu-id="75cb5-355">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-355">Exchange 2013</span></span>  <br/> |
   
## <a name="service-configuration-operation"></a><span data-ttu-id="75cb5-356">サービス構成の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-356">Service configuration operation</span></span>
<span data-ttu-id="75cb5-357"><a name="bk_service_config"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-357"></span></span>

<span data-ttu-id="75cb5-358">サービスの構成操作は、ユニファイド メッセージング、保護の規則、ポリシーのヒントは、メール ヒントおよびサービスの構成情報を取得するクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-358">The service configuration operation enables clients to get configuration information for the Unified Messaging, Protection Rules, Policy Tips, and Mail Tips services.</span></span> 
  
<span data-ttu-id="75cb5-359">サービス構成の操作を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-359">The following table lists the service configuration operation.</span></span>
  
|<span data-ttu-id="75cb5-360">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-360">**Operation name**</span></span>|<span data-ttu-id="75cb5-361">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-361">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-362">GetServiceConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-362">GetServiceConfiguration operation</span></span>](getserviceconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-363">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-363">Exchange 2010</span></span>  <br/> |
   
## <a name="sharing-operations"></a><span data-ttu-id="75cb5-364">操作の共有</span><span class="sxs-lookup"><span data-stu-id="75cb5-364">Sharing operations</span></span>
<span data-ttu-id="75cb5-365"><a name="bk_sharing"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-365"></span></span>

<span data-ttu-id="75cb5-366">共有の操作は、予定表データ、連絡先データを共有するクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-366">The sharing operations enable clients to share calendar data and contacts data.</span></span> 
  
<span data-ttu-id="75cb5-367">次の表は、共有の操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-367">The following table lists the sharing operations.</span></span>
  
|<span data-ttu-id="75cb5-368">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-368">**Operation name**</span></span>|<span data-ttu-id="75cb5-369">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-369">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-370">Createitem メソッド (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="75cb5-370">CreateItem (AcceptSharingInvitation)</span></span>](createitem-acceptsharinginvitation.md) <br/> |<span data-ttu-id="75cb5-371">Exchange 2010。</span><span class="sxs-lookup"><span data-stu-id="75cb5-371">Exchange 2010.</span></span> <span data-ttu-id="75cb5-372">**CreateItem**操作は、EWS のすべてのバージョンに該当する場合は、 **AcceptSharingInvitation**応答オブジェクトは EWS バージョンの Exchange が Exchange 2010 を起動します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-372">Although the **CreateItem** operation is applicable to all versions of EWS, the **AcceptSharingInvitation** response object is only applicable to EWS in versions of Exchange starting with Exchange 2010.</span></span>  <br/> |
|[<span data-ttu-id="75cb5-373">GetSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-373">GetSharingFolder operation</span></span>](getsharingfolder-operation.md) <br/> |<span data-ttu-id="75cb5-374">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-374">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-375">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-375">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md) <br/> |<span data-ttu-id="75cb5-376">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-376">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-377">RefreshSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-377">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md) <br/> |<span data-ttu-id="75cb5-378">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-378">Exchange 2010</span></span>  <br/> |
   
## <a name="synchronization-operations"></a><span data-ttu-id="75cb5-379">同期操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-379">Synchronization operations</span></span>
<span data-ttu-id="75cb5-380"><a name="bk_synchronization"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-380"></span></span>

<span data-ttu-id="75cb5-381">同期操作は、ユーザーのフォルダーおよびアイテムのキャッシュされたコピーの一方向同期を提供します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-381">The synchronization operations provide a one-way synchronized cached copy of a user's folders and items.</span></span> 
  
<span data-ttu-id="75cb5-382">次の表は、同期操作を示します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-382">The following table lists the synchronization operations.</span></span>
  
|<span data-ttu-id="75cb5-383">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-383">**Operation name**</span></span>|<span data-ttu-id="75cb5-384">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-384">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-385">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-385">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md) <br/> |<span data-ttu-id="75cb5-386">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-386">Exchange 2007</span></span>  <br/> |
|[<span data-ttu-id="75cb5-387">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-387">SyncFolderItems operation</span></span>](syncfolderitems-operation.md) <br/> |<span data-ttu-id="75cb5-388">Exchange 2007</span><span class="sxs-lookup"><span data-stu-id="75cb5-388">Exchange 2007</span></span>  <br/> |
   
## <a name="time-zone-operation"></a><span data-ttu-id="75cb5-389">タイム ゾーンの処理</span><span class="sxs-lookup"><span data-stu-id="75cb5-389">Time zone operation</span></span>
<span data-ttu-id="75cb5-390"><a name="bk_timezone"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-390"></span></span>

<span data-ttu-id="75cb5-391">タイム ゾーンの操作は、サーバーでサポートされているタイム ゾーン定義の一覧を取得するクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-391">The time zone operation enables clients to get a list of time zone definitions that are supported by the server.</span></span> 
  
<span data-ttu-id="75cb5-392">次の表に、タイム ゾーンの処理をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-392">The following table lists the time zone operation.</span></span>
  
|<span data-ttu-id="75cb5-393">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-393">**Operation name**</span></span>|<span data-ttu-id="75cb5-394">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-394">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-395">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-395">GetServerTimeZones operation</span></span>](getservertimezones-operation.md) <br/> |<span data-ttu-id="75cb5-396">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-396">Exchange 2010</span></span>  <br/> |
   
## <a name="unified-messaging-operations"></a><span data-ttu-id="75cb5-397">ユニファイド メッセージングの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-397">Unified Messaging operations</span></span>
<span data-ttu-id="75cb5-398"><a name="bk_um"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-398"></span></span>

<span data-ttu-id="75cb5-399">ユニファイド メッセージング操作は、ユニファイド メッセージングのプロパティについての情報を読み取ると、電話でボイス メール メッセージを再生するのにはクライアントを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-399">The Unified Messaging operations enable clients to read information about Unified Messaging properties and to play voice mail messages over the phone.</span></span> 
  
<span data-ttu-id="75cb5-400">次の表に、ユニファイド メッセージングの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-400">The following table lists the Unified Messaging operations.</span></span>
  
|<span data-ttu-id="75cb5-401">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-401">**Operation name**</span></span>|<span data-ttu-id="75cb5-402">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-402">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-403">DisconnectPhoneCall 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-403">DisconnectPhoneCall operation</span></span>](disconnectphonecall-operation.md) <br/> |<span data-ttu-id="75cb5-404">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-404">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-405">GetPhoneCallInformation 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-405">GetPhoneCallInformation operation</span></span>](getphonecallinformation-operation.md) <br/> |<span data-ttu-id="75cb5-406">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-406">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-407">PlayOnPhone 操作 (EWS)</span><span class="sxs-lookup"><span data-stu-id="75cb5-407">PlayOnPhone operation (EWS)</span></span>](playonphone-operation-ews.md) <br/> |<span data-ttu-id="75cb5-408">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-408">Exchange 2010</span></span>  <br/> |
   
<span data-ttu-id="75cb5-409">[GetServiceConfiguration 操作](getserviceconfiguration-operation.md)を使用すると、メールボックスのユニファイド メッセージングの構成情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="75cb5-409">Use the [GetServiceConfiguration operation](getserviceconfiguration-operation.md) to get the Unified Messaging configuration information for a mailbox.</span></span> <span data-ttu-id="75cb5-410">ユニファイド メッセージングの web サービスを Exchange 2007 ユニファイド メッセージング アプリケーションを使用します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-410">Use the Unified Messaging web service for Unified Messaging applications that target Exchange 2007.</span></span> <span data-ttu-id="75cb5-411">詳細については、 [exchange ユニファイド メッセージングの web サービス参照](unified-messaging-web-service-reference-for-exchange.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75cb5-411">For more information, see [Unified Messaging web service reference for Exchange](unified-messaging-web-service-reference-for-exchange.md).</span></span>
  
## <a name="unified-contact-store-operations"></a><span data-ttu-id="75cb5-412">統合連絡先ストアの操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-412">Unified Contact Store operations</span></span>
<span data-ttu-id="75cb5-413"><a name="bk_ucs"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-413"></span></span>

<span data-ttu-id="75cb5-414">統合連絡先ストアでは、Office 製品間で一貫性のある取引先担当者の経験を提供し、同じ連絡先ストアを使用するサードパーティ製のアプリケーションの統合ポイントとして機能します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-414">The Unified Contact Store provides a consistent contact experience across Office products and acts as an integration point for third-party applications to use the same contact store.</span></span> <span data-ttu-id="75cb5-415">格納、管理、および連絡先情報にアクセスおよび Lync 2013 の Exchange、Outlook、Outlook Web App では、統合連絡先ストアへのアクセスを実装するその他のアプリケーション間でグローバルに使用できるようにするには、ユーザーやアプリケーションを有効にします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-415">It enables users and applications to store, manage, and access contact information and make it available globally among Lync, Exchange 2013, Outlook, Outlook Web App, and any other application that implements access to the Unified Contact Store.</span></span> <span data-ttu-id="75cb5-416">Exchange は、統合連絡先ストアで利用するコンテンツのストアです。</span><span class="sxs-lookup"><span data-stu-id="75cb5-416">Exchange is the content store for the Unified Contact Store experience.</span></span>
  
<span data-ttu-id="75cb5-417">次の表は、統合連絡先ストアの操作をします。</span><span class="sxs-lookup"><span data-stu-id="75cb5-417">The following table lists the Unified Contact Store operations.</span></span>
  
|<span data-ttu-id="75cb5-418">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-418">**Operation name**</span></span>|<span data-ttu-id="75cb5-419">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-419">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-420">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-420">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md) <br/> |<span data-ttu-id="75cb5-421">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-421">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-422">AddImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-422">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md) <br/> |<span data-ttu-id="75cb5-423">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-423">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-424">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-424">AddImGroup operation</span></span>](addimgroup-operation.md) <br/> |<span data-ttu-id="75cb5-425">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-425">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-426">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-426">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md) <br/> |<span data-ttu-id="75cb5-427">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-427">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-428">AddDistributionGroupToImList 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-428">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md) <br/> |<span data-ttu-id="75cb5-429">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-429">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-430">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-430">GetImItemList operation</span></span>](getimitemlist-operation.md) <br/> |<span data-ttu-id="75cb5-431">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-431">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-432">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-432">GetImItems operation</span></span>](getimitems-operation.md) <br/> |<span data-ttu-id="75cb5-433">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-433">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-434">RemoveContactFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-434">RemoveContactFromImList operation</span></span>](removecontactfromimlist-operation.md) <br/> |<span data-ttu-id="75cb5-435">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-435">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-436">RemoveImContactFromGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-436">RemoveImContactFromGroup operation</span></span>](removeimcontactfromgroup-operation.md) <br/> |<span data-ttu-id="75cb5-437">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-437">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-438">RemoveDistributionGroupFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-438">RemoveDistributionGroupFromImList operation</span></span>](removedistributiongroupfromimlist-operation.md) <br/> |<span data-ttu-id="75cb5-439">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-439">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-440">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-440">RemoveImGroup operation</span></span>](removeimgroup-operation.md) <br/> |<span data-ttu-id="75cb5-441">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-441">Exchange 2013</span></span>  <br/> |
|[<span data-ttu-id="75cb5-442">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-442">SetImGroup operation</span></span>](setimgroup-operation.md) <br/> |<span data-ttu-id="75cb5-443">Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75cb5-443">Exchange 2013</span></span>  <br/> |
   
## <a name="user-configuration-operations"></a><span data-ttu-id="75cb5-444">ユーザーの構成の操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-444">User configuration operations</span></span>
<span data-ttu-id="75cb5-445"><a name="bk_user_config"> </a></span><span class="sxs-lookup"><span data-stu-id="75cb5-445"></span></span>

<span data-ttu-id="75cb5-446">ユーザーの構成操作は、作成、削除、取得するには、クライアントを有効にして、ユーザー構成情報を更新します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-446">The user configuration operations enable clients to create, delete, get, and update user configuration information.</span></span> 
  
<span data-ttu-id="75cb5-447">次の表は、ユーザーの構成操作を示します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-447">The following table lists the user configuration operations.</span></span>
  
|<span data-ttu-id="75cb5-448">**操作名**</span><span class="sxs-lookup"><span data-stu-id="75cb5-448">**Operation name**</span></span>|<span data-ttu-id="75cb5-449">**導入されました。**</span><span class="sxs-lookup"><span data-stu-id="75cb5-449">**Introduced in**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75cb5-450">CreateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-450">CreateUserConfiguration operation</span></span>](createuserconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-451">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-451">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-452">DeleteUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-452">DeleteUserConfiguration operation</span></span>](deleteuserconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-453">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-453">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-454">GetUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-454">GetUserConfiguration operation</span></span>](getuserconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-455">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-455">Exchange 2010</span></span>  <br/> |
|[<span data-ttu-id="75cb5-456">UpdateUserConfiguration 操作</span><span class="sxs-lookup"><span data-stu-id="75cb5-456">UpdateUserConfiguration operation</span></span>](updateuserconfiguration-operation.md) <br/> |<span data-ttu-id="75cb5-457">Exchange 2010</span><span class="sxs-lookup"><span data-stu-id="75cb5-457">Exchange 2010</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75cb5-458">関連項目</span><span class="sxs-lookup"><span data-stu-id="75cb5-458">See also</span></span>

- [<span data-ttu-id="75cb5-459">Exchange、EWS の管理 API、EWS、および web サービスを探索します。</span><span class="sxs-lookup"><span data-stu-id="75cb5-459">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="75cb5-460">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="75cb5-460">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="75cb5-461">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="75cb5-461">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

