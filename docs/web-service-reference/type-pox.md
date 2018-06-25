---
title: (POX) の種類
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: 型要素は、構成済みのメール アカウントの種類を識別します。
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839759"
---
# <a name="type-pox"></a><span data-ttu-id="3d728-103">(POX) の種類</span><span class="sxs-lookup"><span data-stu-id="3d728-103">Type (POX)</span></span>

<span data-ttu-id="3d728-104">**型**要素は、構成済みのメール アカウントの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="3d728-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="3d728-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="3d728-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="3d728-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="3d728-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="3d728-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="3d728-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="3d728-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="3d728-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="3d728-109">(POX) の種類</span><span class="sxs-lookup"><span data-stu-id="3d728-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3d728-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3d728-110">Attributes and elements</span></span>

<span data-ttu-id="3d728-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3d728-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d728-112">属性</span><span class="sxs-lookup"><span data-stu-id="3d728-112">Attributes</span></span>

<span data-ttu-id="3d728-113">なし。</span><span class="sxs-lookup"><span data-stu-id="3d728-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d728-114">子要素</span><span class="sxs-lookup"><span data-stu-id="3d728-114">Child elements</span></span>

<span data-ttu-id="3d728-115">なし。</span><span class="sxs-lookup"><span data-stu-id="3d728-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d728-116">親要素</span><span class="sxs-lookup"><span data-stu-id="3d728-116">Parent elements</span></span>

|<span data-ttu-id="3d728-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="3d728-117">**Element**</span></span>|<span data-ttu-id="3d728-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d728-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d728-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="3d728-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="3d728-120">クライアントを Exchange サーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3d728-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3d728-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3d728-121">Text value</span></span>

<span data-ttu-id="3d728-122">テキスト値は、メール アカウントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="3d728-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="3d728-123">次の表は、可能な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="3d728-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="3d728-124">**値**</span><span class="sxs-lookup"><span data-stu-id="3d728-124">**Value**</span></span>|<span data-ttu-id="3d728-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="3d728-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3d728-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="3d728-126">EXCH</span></span>  <br/> |<span data-ttu-id="3d728-127">サーバーへの接続に使用されるプロトコルは、Exchange RPC です。</span><span class="sxs-lookup"><span data-stu-id="3d728-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="3d728-128">EXHTTP</span><span class="sxs-lookup"><span data-stu-id="3d728-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="3d728-129">サーバーの RPC/HTTP 接続への接続に使用されるプロトコルです。</span><span class="sxs-lookup"><span data-stu-id="3d728-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="3d728-130">EXPR</span><span class="sxs-lookup"><span data-stu-id="3d728-130">EXPR</span></span>  <br/> |<span data-ttu-id="3d728-131">サーバーへの接続に使用されるプロトコルでは、Exchange RPC over HTTP を RPC プロキシ サーバーを使用しています。</span><span class="sxs-lookup"><span data-stu-id="3d728-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="3d728-132">これは、 [AccountType (POX)](accounttype-pox.md)要素は、電子メールに設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3d728-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="3d728-133">WEB</span><span class="sxs-lookup"><span data-stu-id="3d728-133">WEB</span></span>  <br/> |<span data-ttu-id="3d728-134">電子メールは、[サーバー (POX)](server-pox.md)要素で指定されている URL を使用して Web ブラウザーからアクセスします。</span><span class="sxs-lookup"><span data-stu-id="3d728-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="3d728-135">これは、 [AccountType (POX)](accounttype-pox.md)要素は、電子メールに設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="3d728-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="3d728-136">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="3d728-136">Version differences</span></span>

<span data-ttu-id="3d728-137">Office 365、Exchange Online では、および設置型バージョンの Exchange が始まるビルド 15.00.0995.014 の戻り値が"EXHTTP"のサーバーが RPC または HTTP 接続を受け付けるように構成し、クライアントには、 [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれて 場合にのみです"ExHttpInfo"が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3d728-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3d728-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="3d728-138">See also</span></span>



[<span data-ttu-id="3d728-139">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3d728-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

