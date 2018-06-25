---
title: サーバー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0ce51644-7f3a-408c-a398-814439b658dc
description: サーバー要素は、メール サーバーの名前を指定します。
ms.openlocfilehash: fafd6684d0857bd8b7e1bac0aae0ed162a6a938a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833369"
---
# <a name="server-pox"></a><span data-ttu-id="f4a43-103">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-103">Server (POX)</span></span>

<span data-ttu-id="f4a43-104">**サーバー**要素は、メール サーバーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4a43-104">The **Server** element specifies the name of the mail server.</span></span> 
  
[<span data-ttu-id="f4a43-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="f4a43-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f4a43-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f4a43-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f4a43-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f4a43-109">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-109">Server (POX)</span></span>](server-pox.md)
  
```xml
<Server/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f4a43-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f4a43-110">Attributes and elements</span></span>

<span data-ttu-id="f4a43-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4a43-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4a43-112">属性</span><span class="sxs-lookup"><span data-stu-id="f4a43-112">Attributes</span></span>

<span data-ttu-id="f4a43-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f4a43-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4a43-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f4a43-114">Child elements</span></span>

<span data-ttu-id="f4a43-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f4a43-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4a43-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f4a43-116">Parent elements</span></span>

|<span data-ttu-id="f4a43-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4a43-117">**Element**</span></span>|<span data-ttu-id="f4a43-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4a43-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4a43-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f4a43-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f4a43-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4a43-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4a43-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f4a43-121">Text value</span></span>

<span data-ttu-id="f4a43-122">テキスト値は、サーバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f4a43-122">The text value identifies the server.</span></span> <span data-ttu-id="f4a43-123">POP3、SMTP、IMAP、または NNTP などのプロトコル、ホスト名または IP アドレスのいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f4a43-123">For protocols such as POP3, SMTP, IMAP, or NNTP, this value will be either a host name or an IP address.</span></span> <span data-ttu-id="f4a43-124">WEB DAV などのプロトコルの URL になります。</span><span class="sxs-lookup"><span data-stu-id="f4a43-124">For protocols such as DAV or WEB, this will be a URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f4a43-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4a43-125">See also</span></span>



[<span data-ttu-id="f4a43-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f4a43-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

