---
title: Exchange の Web サービス クライアントを開発する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 899ba15b-336d-4f9b-8563-318c61e43713
description: Exchange 用の EWS と Web サービス クライアントのアプリケーションの開発に役立つ情報を紹介します。
ms.openlocfilehash: 2b8b032124e45dda7c83932d519ffb87bcdb5514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758875"
---
# <a name="develop-web-service-clients-for-exchange"></a><span data-ttu-id="f0c44-103">Exchange の Web サービス クライアントを開発する</span><span class="sxs-lookup"><span data-stu-id="f0c44-103">Develop web service clients for Exchange</span></span>

<span data-ttu-id="f0c44-104">Exchange 用の EWS と Web サービス クライアントのアプリケーションの開発に役立つ情報を紹介します。</span><span class="sxs-lookup"><span data-stu-id="f0c44-104">Find information to help you develop EWS and web service client applications for Exchange.</span></span>
  
<span data-ttu-id="f0c44-105">このセクションの記事では、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange 用の Exchange クライアント アプリケーションにおいて、EWS と Web サービスを使用する方法について説明し、特定のタスクを実行する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="f0c44-105">The articles in this section explain how to use EWS and web services in your Exchange client applications for Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange 2013, and provide examples that show you how to perform specific tasks.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="f0c44-106">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="f0c44-106">In this section</span></span>

- [<span data-ttu-id="f0c44-107">Exchange での EWS のアーカイブ</span><span class="sxs-lookup"><span data-stu-id="f0c44-107">Archiving in EWS in Exchange</span></span>](archiving-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-108">Exchange の添付物と EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-108">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-109">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="f0c44-109">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-110">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-110">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-111">Exchange の配布グループと EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-111">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-112">Exchange での EWS の電子情報開示</span><span class="sxs-lookup"><span data-stu-id="f0c44-112">eDiscovery in EWS in Exchange</span></span>](ediscovery-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-113">Exchange の電子メールと EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-113">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-114">Exchange の EWS のフォルダーとアイテム</span><span class="sxs-lookup"><span data-stu-id="f0c44-114">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-115">Exchange の識別子</span><span class="sxs-lookup"><span data-stu-id="f0c44-115">Identifiers in Exchange</span></span>](ews-identifiers-in-exchange.md)
    
- [<span data-ttu-id="f0c44-116">Exchange の偽装と EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-116">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-117">Exchange での受信トレイの管理と EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-117">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-118">Notification subscriptions, mailbox events, and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="f0c44-118">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-119">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="f0c44-119">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-120">Exchange の EWS の永続的なアプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="f0c44-120">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-121">Exchange における EWS のプロパティと拡張プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0c44-121">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-122">Exchange の EWS でのプロパティ セットと応答の図形</span><span class="sxs-lookup"><span data-stu-id="f0c44-122">Property sets and response shapes in EWS in Exchange</span></span>](property-sets-and-response-shapes-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-123">Exchange での EWS を使用したパブリック フォルダー アクセス</span><span class="sxs-lookup"><span data-stu-id="f0c44-123">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-124">Exchange の検索と EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-124">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-125">Exchange のメールボックス同期と EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-125">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-126">Exchange のタイム ゾーンと EWS</span><span class="sxs-lookup"><span data-stu-id="f0c44-126">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f0c44-127">Exchange の EWS アプリケーションのトラブルシューティングに使用するツールとリソース</span><span class="sxs-lookup"><span data-stu-id="f0c44-127">Tools and resources for troubleshooting EWS applications for Exchange</span></span>](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    
- [<span data-ttu-id="f0c44-128">EWS または EWS マネージ API の呼び出しの結果の確認</span><span class="sxs-lookup"><span data-stu-id="f0c44-128">Verifying the results of an EWS or EWS Managed API call</span></span>](verifying-the-results-of-an-ews-or-ews-managed-api-call.md)
    
## <a name="see-also"></a><span data-ttu-id="f0c44-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0c44-129">See also</span></span>

- [<span data-ttu-id="f0c44-130">Exchange、EWS の管理 API、EWS、および web サービスを探索します。</span><span class="sxs-lookup"><span data-stu-id="f0c44-130">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)     
- [<span data-ttu-id="f0c44-131">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="f0c44-131">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="f0c44-132">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="f0c44-132">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)  
- [<span data-ttu-id="f0c44-133">Exchange web サービスの参照</span><span class="sxs-lookup"><span data-stu-id="f0c44-133">Web services reference for Exchange</span></span>](../web-service-reference/web-services-reference-for-exchange.md)
    

