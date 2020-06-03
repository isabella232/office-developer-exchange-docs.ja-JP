---
title: EcpUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7cbd6076-9981-4c65-a296-5e57518671b5
description: EcpUrl 要素は、メールが有効なユーザーの Exchange コントロールパネルの URL を指定します。
ms.openlocfilehash: b761147dc5912652bca2847bd5ec0d305e0624b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461276"
---
# <a name="ecpurl-pox"></a><span data-ttu-id="24f6b-103">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-103">EcpUrl (POX)</span></span>

<span data-ttu-id="24f6b-104">**EcpUrl**要素は、メールが有効なユーザーの Exchange コントロールパネルの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="24f6b-104">The **EcpUrl** element specifies the URL of the Exchange Control Panel for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="24f6b-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="24f6b-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="24f6b-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="24f6b-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="24f6b-109">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-109">EcpUrl (POX)</span></span>](ecpurl-pox.md)
  
```XML
<EcpUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="24f6b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="24f6b-110">Attributes and elements</span></span>

<span data-ttu-id="24f6b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="24f6b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24f6b-112">属性</span><span class="sxs-lookup"><span data-stu-id="24f6b-112">Attributes</span></span>

<span data-ttu-id="24f6b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="24f6b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24f6b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="24f6b-114">Child elements</span></span>

<span data-ttu-id="24f6b-115">なし。</span><span class="sxs-lookup"><span data-stu-id="24f6b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24f6b-116">親要素</span><span class="sxs-lookup"><span data-stu-id="24f6b-116">Parent elements</span></span>

|<span data-ttu-id="24f6b-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="24f6b-117">**Element**</span></span>|<span data-ttu-id="24f6b-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="24f6b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f6b-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="24f6b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="24f6b-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="24f6b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24f6b-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="24f6b-121">Text value</span></span>

<span data-ttu-id="24f6b-122">Text 値は、ユーザーの Exchange コントロールパネルの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="24f6b-122">The text value represents the URL of the Exchange Control Panel for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24f6b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="24f6b-123">Remarks</span></span>

<span data-ttu-id="24f6b-124">**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="24f6b-124">The **EcpUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="24f6b-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="24f6b-125">See also</span></span>



[<span data-ttu-id="24f6b-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="24f6b-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

