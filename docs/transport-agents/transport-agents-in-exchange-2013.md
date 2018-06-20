---
title: Exchange のトランスポート エージェント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Exchange 2013 のトランスポート エージェントについての情報を検索します。
ms.openlocfilehash: 1a28ae79e2a7e338ddd6cb1f6961dd14a980b56e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759261"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="3109a-103">Exchange のトランスポート エージェント</span><span class="sxs-lookup"><span data-stu-id="3109a-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="3109a-104">Exchange 2013 は、書き込み、およびコンテンツの種類の変換に、Exchange トランスポートの動作の拡張機能をサポートし、読み取りを有効にするクラスのライブラリを提供します。</span><span class="sxs-lookup"><span data-stu-id="3109a-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="3109a-105">これらのクラスを使用すると、読み取り、書き込み、およびトランスポート パイプラインでメッセージを処理する Exchange トランスポートのアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="3109a-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="3109a-106">トランスポート エージェントについて知っておくべき事項</span><span class="sxs-lookup"><span data-stu-id="3109a-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="3109a-107">についてわからない場合.</span><span class="sxs-lookup"><span data-stu-id="3109a-107">If you're wondering about…</span></span>|<span data-ttu-id="3109a-108">説明</span><span class="sxs-lookup"><span data-stu-id="3109a-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="3109a-109">可用性</span><span class="sxs-lookup"><span data-stu-id="3109a-109">Availability</span></span>  <br/> |<span data-ttu-id="3109a-110">トランスポート エージェントは、Exchange が Exchange 2007 以降のバージョンで使用できます。</span><span class="sxs-lookup"><span data-stu-id="3109a-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="3109a-111">Office 365 または Exchange Online では、トランスポート エージェントはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3109a-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="3109a-112">リモート使用</span><span class="sxs-lookup"><span data-stu-id="3109a-112">Remote usage</span></span>  <br/> |<span data-ttu-id="3109a-113">トランスポート エージェントは Exchange サーバー上で実行し、リモート使用をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="3109a-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="3109a-114">サポートされている言語</span><span class="sxs-lookup"><span data-stu-id="3109a-114">Languages supported</span></span>  <br/> |<span data-ttu-id="3109a-115">トランスポート エージェントには、任意の .NET Framework 言語を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3109a-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="3109a-116">利用可能なテスト ツールとデバッグ ツール</span><span class="sxs-lookup"><span data-stu-id="3109a-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="3109a-117">トランスポート エージェントのデバッグには、Visual Studio 2012 以降の Visual Studio の各バージョンを使用してください。</span><span class="sxs-lookup"><span data-stu-id="3109a-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="3109a-118">展開の方法</span><span class="sxs-lookup"><span data-stu-id="3109a-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="3109a-119">トランスポート エージェントのアプリケーションをインストールするには、 [Exchange 管理シェル](../management/exchange-management-shell.md)スクリプトを使用します。</span><span class="sxs-lookup"><span data-stu-id="3109a-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="3109a-120">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="3109a-120">In this section</span></span>

- [<span data-ttu-id="3109a-121">新規および更新されたトランスポート エージェントでは、Exchange 2013 の Api</span><span class="sxs-lookup"><span data-stu-id="3109a-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="3109a-122">Exchange 2013 のエージェントのコード サンプルを転送します。</span><span class="sxs-lookup"><span data-stu-id="3109a-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="3109a-123">トランスポート エージェントの概念には、Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="3109a-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="3109a-124">読み取りおよび Exchange 2013 のトランスポート パイプライン内のメッセージを変更します。</span><span class="sxs-lookup"><span data-stu-id="3109a-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="3109a-125">Exchange 2013 のトランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="3109a-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="3109a-126">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="3109a-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="3109a-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="3109a-127">See also</span></span>

- [<span data-ttu-id="3109a-128">オンラインの Exchange および Exchange の開発</span><span class="sxs-lookup"><span data-stu-id="3109a-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="3109a-129">Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ</span><span class="sxs-lookup"><span data-stu-id="3109a-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="3109a-130">Exchange のバックアップ/リストア</span><span class="sxs-lookup"><span data-stu-id="3109a-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

