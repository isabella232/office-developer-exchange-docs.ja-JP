---
title: Exchange での EWS の電子情報開示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Exchange の EWS の電子情報開示について説明します。
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758881"
---
# <a name="ediscovery-in-ews-in-exchange"></a><span data-ttu-id="27b78-103">Exchange での EWS の電子情報開示</span><span class="sxs-lookup"><span data-stu-id="27b78-103">eDiscovery in EWS in Exchange</span></span>

<span data-ttu-id="27b78-104">Exchange の EWS の電子情報開示について説明します。</span><span class="sxs-lookup"><span data-stu-id="27b78-104">Learn about eDiscovery in EWS in Exchange.</span></span>
  
<span data-ttu-id="27b78-105">電子情報開示は、外部アプリケーションが Exchange データのクエリを実行できるようにするフェデレーション クエリ Web サービスです。</span><span class="sxs-lookup"><span data-stu-id="27b78-105">eDiscovery is a federated query web service that enables external applications to perform queries of Exchange data.</span></span>
  
<span data-ttu-id="27b78-p101">証拠開示は、主なデータの識別や保持、データの選別や確認、法廷でのデータの生成を含むいくつかのフェーズから構成されます。電子情報開示のクエリは、Exchange と SharePoint にまたがる単一の証拠開示ワークフローを提供することで、証拠開示プロセスを容易にします。</span><span class="sxs-lookup"><span data-stu-id="27b78-p101">Discovery consists of several phases, including identifying and preserving key data, culling down and reviewing the data, and producing data in court. eDiscovery queries facilitate the discovery process by providing a single discovery workflow across Exchange and SharePoint.</span></span>
  
## <a name="ediscovery-operations"></a><span data-ttu-id="27b78-108">電子情報開示の操作</span><span class="sxs-lookup"><span data-stu-id="27b78-108">eDiscovery operations</span></span>

<span data-ttu-id="27b78-109">EWS で公開されている電子情報開示機能は、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のバージョンの Exchange で導入された操作によって利用できます。</span><span class="sxs-lookup"><span data-stu-id="27b78-109">The eDiscovery functionality that is exposed by EWS is available via operations introduced in Exchange Online, Exchange Online as part of Office 365, and versions of Exchange starting with exchange15short.</span></span> 
  
<span data-ttu-id="27b78-110">**表 1. 電子情報開示のための新しい操作**</span><span class="sxs-lookup"><span data-stu-id="27b78-110">**Table 1.  New operations for eDiscovery**</span></span>

|<span data-ttu-id="27b78-111">**操作名**</span><span class="sxs-lookup"><span data-stu-id="27b78-111">**Operation name**</span></span>|<span data-ttu-id="27b78-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="27b78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27b78-113">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="27b78-113">GetDiscoverySearchConfiguration</span></span>](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-114">インプレース ホールド、保存された探索検索、探索検索が有効になっているメールボックスの構成情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="27b78-114">Gets configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span>  <br/> |
|[<span data-ttu-id="27b78-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="27b78-115">GetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-116">クエリ ベースの保持 ([SetHoldOnMailboxes 操作](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx)を使用して設定される) の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="27b78-116">Gets the status of a query-based hold, which is set by using the SetHoldOnMailboxes operation.</span></span>  <br/> |
|[<span data-ttu-id="27b78-117">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="27b78-117">GetNonIndexableItemDetails</span></span>](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-p102">インデックスを作成できないアイテムの詳細を取得します。これには、アイテム識別子、エラー コード、エラーの説明、アイテムのインデックス作成をしようとしたタイミング、ファイルに関する追加情報が含まれますが、これに限定されません。</span><span class="sxs-lookup"><span data-stu-id="27b78-p102">Retrieves details about items that cannot be indexed. This includes, but is not limited to, the item identifier, an error code, an error description, when an attempt was made to index the item, and additional information about the file.</span></span>  <br/> |
|[<span data-ttu-id="27b78-120">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="27b78-120">GetNonIndexableItemStatistics</span></span>](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-121">メールボックス内にある、インデックスを作成できないアイテムの数を取得します。</span><span class="sxs-lookup"><span data-stu-id="27b78-121">Retrieves the count of items that cannot be indexed in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="27b78-122">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="27b78-122">GetSearchableMailboxes</span></span>](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-123">クライアントが検索または電子情報開示を実行するアクセス許可を持つメールボックスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="27b78-123">Gets a list of mailboxes that the client has permission to search or perform eDiscovery on.</span></span>  <br/> |
|[<span data-ttu-id="27b78-124">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="27b78-124">SearchMailboxes</span></span>](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-125">特定のメールボックス内にある、クエリ キーワードに一致するアイテムを検索します。</span><span class="sxs-lookup"><span data-stu-id="27b78-125">Searches for items in specific mailboxes that match query keywords.</span></span>  <br/> |
|[<span data-ttu-id="27b78-126">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="27b78-126">SetHoldOnMailboxes</span></span>](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |<span data-ttu-id="27b78-127">アイテムにクエリベースの保持を設定します。</span><span class="sxs-lookup"><span data-stu-id="27b78-127">Sets a query-based hold on items.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27b78-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="27b78-128">See also</span></span>

- [<span data-ttu-id="27b78-129">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="27b78-129">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="27b78-130">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="27b78-130">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="27b78-131">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="27b78-131">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

