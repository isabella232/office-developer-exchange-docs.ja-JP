---
title: Exchange のトランスポート エージェント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Exchange 2013 のトランスポートエージェントに関する情報を参照してください。
ms.openlocfilehash: 62fb259672c47242a57b939deb4887e1e5519e2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461759"
---
# <a name="transport-agents-in-exchange"></a><span data-ttu-id="01dd7-103">Exchange のトランスポート エージェント</span><span class="sxs-lookup"><span data-stu-id="01dd7-103">Transport agents in Exchange</span></span>
  
<span data-ttu-id="01dd7-104">Exchange 2013 には、Exchange トランスポート動作の拡張をサポートし、コンテンツタイプの読み取り、書き込み、および変換を可能にするクラスのライブラリが用意されています。</span><span class="sxs-lookup"><span data-stu-id="01dd7-104">Exchange 2013 provides a library of classes that support the extension of the Exchange transport behavior and enable the reading, writing, and converting of content types.</span></span> <span data-ttu-id="01dd7-105">これらのクラスを使用すると、トランスポート パイプライン内でメッセージの読み取り、書き込み、および処理を行う Exchange トランスポート アプリケーションを作成できます。</span><span class="sxs-lookup"><span data-stu-id="01dd7-105">You can use these classes to create Exchange transport applications that read, write, and process messages in the transport pipeline.</span></span>
  
## <a name="what-you-need-to-know-about-transport-agents"></a><span data-ttu-id="01dd7-106">トランスポート エージェントについて知っておくべき事項</span><span class="sxs-lookup"><span data-stu-id="01dd7-106">What you need to know about transport agents</span></span>

|<span data-ttu-id="01dd7-107">ご参考までに</span><span class="sxs-lookup"><span data-stu-id="01dd7-107">If you're wondering about…</span></span>|<span data-ttu-id="01dd7-108">説明</span><span class="sxs-lookup"><span data-stu-id="01dd7-108">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="01dd7-109">可用性</span><span class="sxs-lookup"><span data-stu-id="01dd7-109">Availability</span></span>  <br/> |<span data-ttu-id="01dd7-110">トランスポートエージェントは、Exchange 2007 以降のバージョンの Exchange で使用できます。</span><span class="sxs-lookup"><span data-stu-id="01dd7-110">Transport agents are available in versions of Exchange starting with Exchange 2007.</span></span> <span data-ttu-id="01dd7-111">トランスポートエージェントは、Office 365 または Exchange Online ではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01dd7-111">Transport agents are not supported in Office 365 or Exchange Online.</span></span>  <br/> |
|<span data-ttu-id="01dd7-112">リモート使用</span><span class="sxs-lookup"><span data-stu-id="01dd7-112">Remote usage</span></span>  <br/> |<span data-ttu-id="01dd7-113">トランスポート エージェントは Exchange サーバー上で実行し、リモート使用をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="01dd7-113">Transport agents run on the Exchange server and do not support remote usage.</span></span>  <br/> |
|<span data-ttu-id="01dd7-114">サポートされている言語</span><span class="sxs-lookup"><span data-stu-id="01dd7-114">Languages supported</span></span>  <br/> |<span data-ttu-id="01dd7-115">トランスポート エージェントには、任意の .NET Framework 言語を使用できます。</span><span class="sxs-lookup"><span data-stu-id="01dd7-115">You can use any .NET Framework language to work with transport agents.</span></span>  <br/> |
|<span data-ttu-id="01dd7-116">利用可能なテスト ツールとデバッグ ツール</span><span class="sxs-lookup"><span data-stu-id="01dd7-116">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="01dd7-117">トランスポート エージェントのデバッグには、Visual Studio 2012 以降の Visual Studio の各バージョンを使用してください。</span><span class="sxs-lookup"><span data-stu-id="01dd7-117">Use versions of Visual Studio starting with Visual Studio 2012 to debug transport agents.</span></span>  <br/> |
|<span data-ttu-id="01dd7-118">展開の方法</span><span class="sxs-lookup"><span data-stu-id="01dd7-118">Deployment methods</span></span>  <br/> |<span data-ttu-id="01dd7-119">トランスポート エージェント アプリケーションは、[Exchange 管理シェル](../management/exchange-management-shell.md) スクリプトを使用してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="01dd7-119">You can install transport agent applications by using an [Exchange Management Shell](../management/exchange-management-shell.md) script.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="01dd7-120">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="01dd7-120">In this section</span></span>

- [<span data-ttu-id="01dd7-121">Exchange 2013 の新規および更新されたトランスポート エージェント API</span><span class="sxs-lookup"><span data-stu-id="01dd7-121">New and updated transport agent APIs in Exchange 2013</span></span>](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [<span data-ttu-id="01dd7-122">Exchange 2013 のトランスポート エージェントのコード サンプル</span><span class="sxs-lookup"><span data-stu-id="01dd7-122">Transport agent code samples for Exchange 2013</span></span>](transport-agent-code-samples-for-exchange-2013.md)
    
- [<span data-ttu-id="01dd7-123">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="01dd7-123">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
    
- [<span data-ttu-id="01dd7-124">Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更</span><span class="sxs-lookup"><span data-stu-id="01dd7-124">Reading and modifying messages in the Exchange 2013 transport pipeline</span></span>](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [<span data-ttu-id="01dd7-125">Exchange 2013 のトランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="01dd7-125">Creating transport agents for Exchange 2013</span></span>](creating-transport-agents-for-exchange-2013.md)
    
- [<span data-ttu-id="01dd7-126">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="01dd7-126">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="01dd7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="01dd7-127">See also</span></span>

- [<span data-ttu-id="01dd7-128">Exchange Online と Exchange の開発</span><span class="sxs-lookup"><span data-stu-id="01dd7-128">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)    
- [<span data-ttu-id="01dd7-129">Exchange の EWS マネージ API、EWS、Web サービスについて探究してみましょう</span><span class="sxs-lookup"><span data-stu-id="01dd7-129">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [<span data-ttu-id="01dd7-130">Exchange のバックアップと復元</span><span class="sxs-lookup"><span data-stu-id="01dd7-130">Backup and restore for Exchange</span></span>](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

