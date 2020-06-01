---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: ServerDN 要素は、Microsoft Exchange Server 2007 を実行しているコンピューターの識別名を指定します。
ms.openlocfilehash: 16c6e7368e221b7e54c8d7d63532bb29464a7e54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461997"
---
# <a name="serverdn-pox"></a><span data-ttu-id="10a95-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-103">ServerDN (POX)</span></span>

<span data-ttu-id="10a95-104">**Serverdn**要素は、Microsoft Exchange Server 2007 を実行しているコンピューターの識別名を指定します。</span><span class="sxs-lookup"><span data-stu-id="10a95-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="10a95-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="10a95-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="10a95-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="10a95-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="10a95-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="10a95-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="10a95-110">Attributes and elements</span></span>

<span data-ttu-id="10a95-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="10a95-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10a95-112">属性</span><span class="sxs-lookup"><span data-stu-id="10a95-112">Attributes</span></span>

<span data-ttu-id="10a95-113">なし。</span><span class="sxs-lookup"><span data-stu-id="10a95-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10a95-114">子要素</span><span class="sxs-lookup"><span data-stu-id="10a95-114">Child elements</span></span>

<span data-ttu-id="10a95-115">なし。</span><span class="sxs-lookup"><span data-stu-id="10a95-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10a95-116">親要素</span><span class="sxs-lookup"><span data-stu-id="10a95-116">Parent elements</span></span>

|<span data-ttu-id="10a95-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="10a95-117">**Element**</span></span>|<span data-ttu-id="10a95-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="10a95-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10a95-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="10a95-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="10a95-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="10a95-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10a95-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="10a95-121">Text value</span></span>

<span data-ttu-id="10a95-122">Text 値は、Exchange サーバーの識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="10a95-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10a95-123">注釈</span><span class="sxs-lookup"><span data-stu-id="10a95-123">Remarks</span></span>

<span data-ttu-id="10a95-124">**Serverdn**の値は、 [Type (POX)](type-pox.md)が EXCH と等しい場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="10a95-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="10a95-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="10a95-125">See also</span></span>



[<span data-ttu-id="10a95-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="10a95-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

