---
title: Exchange 2013 のトランスポート エージェントの名前空間
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c40788e-c182-4502-9202-206e6aaa53f8
description: Exchange 2013 用のカスタムトランスポートエージェントを作成するために使用できる .NET Framework のクラスとメンバーについて説明します。
ms.openlocfilehash: fc2d9108c910a730bb48c5be028797f0f15ad4ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461794"
---
# <a name="transport-agent-namespaces-in-exchange-2013"></a><span data-ttu-id="de80f-103">Exchange 2013 のトランスポート エージェントの名前空間</span><span class="sxs-lookup"><span data-stu-id="de80f-103">Transport agent namespaces in Exchange 2013</span></span>

<span data-ttu-id="de80f-104">Exchange 2013 用のカスタムトランスポートエージェントを作成するために使用できる .NET Framework のクラスとメンバーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="de80f-104">Learn about the .NET Framework classes and members that you can use to create custom transport agents for Exchange 2013.</span></span>
  
<span data-ttu-id="de80f-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="de80f-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="de80f-106">この記事では、Exchange Server 2013 のトランスポートエージェントの作成に使用できる参照情報を含む名前空間について説明します。</span><span class="sxs-lookup"><span data-stu-id="de80f-106">This article provides information about the namespaces that contain reference information that you can use to create transport agents for Exchange Server 2013.</span></span> <span data-ttu-id="de80f-107">さらに、トランスポート パイプラインを通過する電子メール メッセージの読み取りおよび変更をトランスポート エージェントで行うために使用できるクラスについても説明します。</span><span class="sxs-lookup"><span data-stu-id="de80f-107">It also describes the classes that your transport agents can use to read and modify email messages that pass through the transport pipeline.</span></span>
  
## <a name="transport-agent-class-library"></a><span data-ttu-id="de80f-108">トランスポート エージェントのクラス ライブラリ</span><span class="sxs-lookup"><span data-stu-id="de80f-108">Transport agent class library</span></span>

<span data-ttu-id="de80f-109">次の名前空間には、トランスポート エージェントの作成と拡張に使用できる型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-109">The following namespaces contain types that you can use to create and extend transport agents.</span></span>

<span data-ttu-id="de80f-110">**表1.NET Framework の名前空間**</span><span class="sxs-lookup"><span data-stu-id="de80f-110">**Table 1. .NET Framework namespaces**</span></span>

|<span data-ttu-id="de80f-111">**名前空間**</span><span class="sxs-lookup"><span data-stu-id="de80f-111">**Namespace**</span></span>|<span data-ttu-id="de80f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="de80f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de80f-113">Microsoft のデータ交換</span><span class="sxs-lookup"><span data-stu-id="de80f-113">Microsoft.Exchange.Data</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.aspx) <br/> |<span data-ttu-id="de80f-114">データと構成の例外を指定する型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-114">Contains types that specify data and configuration exceptions.</span></span>  <br/> |
|[<span data-ttu-id="de80f-115">Microsoft. データ共有</span><span class="sxs-lookup"><span data-stu-id="de80f-115">Microsoft.Exchange.Data.Common</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Common.aspx) <br/> |<span data-ttu-id="de80f-116">ローカライズとエラー処理をサポートする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-116">Contains types that support localization and error handling.</span></span>  <br/> |
|[<span data-ttu-id="de80f-117">ContentTypes を行います。</span><span class="sxs-lookup"><span data-stu-id="de80f-117">Microsoft.Exchange.Data.ContentTypes.iCalendar</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.aspx) <br/> |<span data-ttu-id="de80f-118">iCalendar データの読み取りと書き込みを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-118">Contains types that enable you to read and write iCalendar data.</span></span>  <br/> |
|[<span data-ttu-id="de80f-119">ContentTypes (. Tnef)</span><span class="sxs-lookup"><span data-stu-id="de80f-119">Microsoft.Exchange.Data.ContentTypes.Tnef</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.aspx) <br/> |<span data-ttu-id="de80f-120">TNEF データの読み取りと書き込みを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-120">Contains types that enable you to read and write TNEF data.</span></span>  <br/> |
|[<span data-ttu-id="de80f-121">ContentTypes (. vCard)</span><span class="sxs-lookup"><span data-stu-id="de80f-121">Microsoft.Exchange.Data.ContentTypes.vCard</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.vCard.aspx) <br/> |<span data-ttu-id="de80f-122">vCard データの読み取りと書き込みを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-122">Contains types that enable you to read and write vCard data.</span></span>  <br/> |
|[<span data-ttu-id="de80f-123">Microsoft によるデータのグローバリゼーション</span><span class="sxs-lookup"><span data-stu-id="de80f-123">Microsoft.Exchange.Data.Globalization</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Globalization.aspx) <br/> |<span data-ttu-id="de80f-124">ローカライズされたコンテンツを生成するカルチャと文字セットの操作を可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-124">Contains types that enable you to work with cultures and character sets to produce localized content.</span></span>  <br/> |
|[<span data-ttu-id="de80f-125">Microsoft. データの Mime</span><span class="sxs-lookup"><span data-stu-id="de80f-125">Microsoft.Exchange.Data.Mime</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.aspx) <br/> |<span data-ttu-id="de80f-126">MIME データの読み取りと書き込みを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-126">Contains types that enable you to read and write MIME data.</span></span>  <br/> |
|[<span data-ttu-id="de80f-127">(データの場合)</span><span class="sxs-lookup"><span data-stu-id="de80f-127">Microsoft.Exchange.Data.Mime.Encoders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.aspx) <br/> |<span data-ttu-id="de80f-128">MIME データのエンコードとデコードを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-128">Contains types that enable you to encode and decode MIME data.</span></span>  <br/> |
|[<span data-ttu-id="de80f-129">Microsoft のデータ変換器</span><span class="sxs-lookup"><span data-stu-id="de80f-129">Microsoft.Exchange.Data.TextConverters</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.aspx) <br/> |<span data-ttu-id="de80f-130">各種のテキスト形式によるデータの読み書きと、それらの形式間での変換を可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-130">Contains types that enable you to read and write data with different text formats, and convert data to and from those formats.</span></span>  <br/> |
|[<span data-ttu-id="de80f-131">Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="de80f-131">Microsoft.Exchange.Data.Transport</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.aspx) <br/> |<span data-ttu-id="de80f-132">トランスポート パイプラインに関するルーティング情報、ホスト情報、およびドメイン情報へのアクセスを可能にする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-132">Contains types that enable you to access routing, host, and domain information about the transport pipeline.</span></span>  <br/> |
|[<span data-ttu-id="de80f-133">その後、配送。</span><span class="sxs-lookup"><span data-stu-id="de80f-133">Microsoft.Exchange.Data.Transport.Delivery</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.aspx) <br/> |<span data-ttu-id="de80f-134">Exchange 2013 配信エージェントの拡張機能をサポートする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-134">Contains types that support the extension of Exchange 2013 delivery agents.</span></span>  <br/> |
|[<span data-ttu-id="de80f-135">その後、電子メール</span><span class="sxs-lookup"><span data-stu-id="de80f-135">Microsoft.Exchange.Data.Transport.Email</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.aspx) <br/> |<span data-ttu-id="de80f-136">電子メール メッセージの読み取り、書き込み、および変更をサポートする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-136">Contains types that support creating, reading, writing, and modifying email messages.</span></span>  <br/> |
|[<span data-ttu-id="de80f-137">Microsoft Exchange Server のルーティング</span><span class="sxs-lookup"><span data-stu-id="de80f-137">Microsoft.Exchange.Data.Transport.Routing</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.aspx) <br/> |<span data-ttu-id="de80f-138">Exchange 2013 トランスポートルーティングの動作の拡張をサポートする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-138">Contains types that support the extension of the Exchange 2013 transport routing behavior.</span></span>  <br/> |
|[<span data-ttu-id="de80f-139">その後、Smtp (トランスポート)</span><span class="sxs-lookup"><span data-stu-id="de80f-139">Microsoft.Exchange.Data.Transport.Smtp</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.aspx) <br/> |<span data-ttu-id="de80f-140">Exchange 2013 トランスポート SMTP の動作の拡張をサポートする型が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de80f-140">Contains types that support the extension of the Exchange 2013 transport SMTP behavior.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de80f-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="de80f-141">See also</span></span>

- [<span data-ttu-id="de80f-142">Exchange のトランスポート エージェント</span><span class="sxs-lookup"><span data-stu-id="de80f-142">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)   
- [<span data-ttu-id="de80f-143">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="de80f-143">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md) 
- <span data-ttu-id="de80f-144">
  [Exchange 用 EWS リファレンス](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="de80f-144">[Server API reference for Exchange](https://msdn.microsoft.com/library/6eddd052-f59f-45b4-b846-7e53d4d7eb16%28Office.15%29.aspx)</span></span>
- [<span data-ttu-id="de80f-145">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="de80f-145">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)
    

