---
title: 種類 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Type 要素は、構成されたメールアカウントの種類を識別します。
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465101"
---
# <a name="type-pox"></a><span data-ttu-id="8e30a-103">種類 (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-103">Type (POX)</span></span>

<span data-ttu-id="8e30a-104">**Type**要素は、構成されたメールアカウントの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="8e30a-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8e30a-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8e30a-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8e30a-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8e30a-109">種類 (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8e30a-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8e30a-110">Attributes and elements</span></span>

<span data-ttu-id="8e30a-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e30a-112">属性</span><span class="sxs-lookup"><span data-stu-id="8e30a-112">Attributes</span></span>

<span data-ttu-id="8e30a-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8e30a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e30a-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8e30a-114">Child elements</span></span>

<span data-ttu-id="8e30a-115">なし。</span><span class="sxs-lookup"><span data-stu-id="8e30a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e30a-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8e30a-116">Parent elements</span></span>

|<span data-ttu-id="8e30a-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="8e30a-117">**Element**</span></span>|<span data-ttu-id="8e30a-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e30a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e30a-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8e30a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8e30a-120">クライアントを Exchange サーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8e30a-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e30a-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8e30a-121">Text value</span></span>

<span data-ttu-id="8e30a-122">Text 値は、メールアカウントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="8e30a-123">次の表に、使用可能な値を示します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="8e30a-124">**値**</span><span class="sxs-lookup"><span data-stu-id="8e30a-124">**Value**</span></span>|<span data-ttu-id="8e30a-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="8e30a-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8e30a-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="8e30a-126">EXCH</span></span>  <br/> |<span data-ttu-id="8e30a-127">サーバーへの接続に使用されるプロトコルは、Exchange RPC です。</span><span class="sxs-lookup"><span data-stu-id="8e30a-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="8e30a-128">EXHTTP</span><span class="sxs-lookup"><span data-stu-id="8e30a-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="8e30a-129">サーバーの RPC/HTTP 接続に接続するために使用されるプロトコル。</span><span class="sxs-lookup"><span data-stu-id="8e30a-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="8e30a-130">引数</span><span class="sxs-lookup"><span data-stu-id="8e30a-130">EXPR</span></span>  <br/> |<span data-ttu-id="8e30a-131">サーバーへの接続に使用されるプロトコルは、RPC プロキシサーバーを使用する Exchange RPC over HTTP です。</span><span class="sxs-lookup"><span data-stu-id="8e30a-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="8e30a-132">これは、 [AccountType (POX)](accounttype-pox.md)要素が電子メールに設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8e30a-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="8e30a-133">WEB</span><span class="sxs-lookup"><span data-stu-id="8e30a-133">WEB</span></span>  <br/> |<span data-ttu-id="8e30a-134">Web ブラウザーから電子メールにアクセスするには、[サーバー (POX)](server-pox.md)要素で指定されている URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="8e30a-135">これは、 [AccountType (POX)](accounttype-pox.md)要素が電子メールに設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="8e30a-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="8e30a-136">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="8e30a-136">Version differences</span></span>

<span data-ttu-id="8e30a-137">Office 365、Exchange Online、およびオンプレミスバージョンの Exchange は、サーバーが RPC/HTTP 接続を受け付けるように構成されており、クライアントに "ExHttpInfo" が含まれている[X ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、build 15.00.0995.014 からの値を返します。</span><span class="sxs-lookup"><span data-stu-id="8e30a-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8e30a-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="8e30a-138">See also</span></span>



[<span data-ttu-id="8e30a-139">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="8e30a-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

