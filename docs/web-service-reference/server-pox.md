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
description: Server 要素は、メールサーバーの名前を指定します。
ms.openlocfilehash: 6b29b153bc75b8836bfa113e126d122d620c2984
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462011"
---
# <a name="server-pox"></a><span data-ttu-id="cba19-103">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-103">Server (POX)</span></span>

<span data-ttu-id="cba19-104">**Server**要素は、メールサーバーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="cba19-104">The **Server** element specifies the name of the mail server.</span></span> 
  
[<span data-ttu-id="cba19-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="cba19-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="cba19-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="cba19-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="cba19-109">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-109">Server (POX)</span></span>](server-pox.md)
  
```xml
<Server/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cba19-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cba19-110">Attributes and elements</span></span>

<span data-ttu-id="cba19-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cba19-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cba19-112">属性</span><span class="sxs-lookup"><span data-stu-id="cba19-112">Attributes</span></span>

<span data-ttu-id="cba19-113">なし。</span><span class="sxs-lookup"><span data-stu-id="cba19-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cba19-114">子要素</span><span class="sxs-lookup"><span data-stu-id="cba19-114">Child elements</span></span>

<span data-ttu-id="cba19-115">なし。</span><span class="sxs-lookup"><span data-stu-id="cba19-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cba19-116">親要素</span><span class="sxs-lookup"><span data-stu-id="cba19-116">Parent elements</span></span>

|<span data-ttu-id="cba19-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="cba19-117">**Element**</span></span>|<span data-ttu-id="cba19-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="cba19-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cba19-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="cba19-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cba19-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cba19-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cba19-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cba19-121">Text value</span></span>

<span data-ttu-id="cba19-122">テキスト値は、サーバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="cba19-122">The text value identifies the server.</span></span> <span data-ttu-id="cba19-123">POP3、SMTP、IMAP、NNTP などのプロトコルの場合、この値はホスト名または IP アドレスのいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="cba19-123">For protocols such as POP3, SMTP, IMAP, or NNTP, this value will be either a host name or an IP address.</span></span> <span data-ttu-id="cba19-124">DAV や WEB などのプロトコルの場合は、URL になります。</span><span class="sxs-lookup"><span data-stu-id="cba19-124">For protocols such as DAV or WEB, this will be a URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="cba19-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="cba19-125">See also</span></span>



[<span data-ttu-id="cba19-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="cba19-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

