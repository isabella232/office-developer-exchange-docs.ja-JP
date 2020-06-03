---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: EcpUrl-aggr 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーの電子メール集計設定にアクセスするために使用できる URL を生成できる url の部分を指定します。
ms.openlocfilehash: 26e855900154fb965eae9ba90a373b88e85c2ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457285"
---
# <a name="ecpurl-aggr-pox"></a><span data-ttu-id="91c44-103">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-103">EcpUrl-aggr (POX)</span></span>

<span data-ttu-id="91c44-104">**EcpUrl-aggr**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メール集計設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="91c44-104">The **EcpUrl-aggr** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="91c44-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="91c44-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="91c44-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="91c44-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="91c44-109">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-109">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="91c44-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="91c44-110">Attributes and elements</span></span>

<span data-ttu-id="91c44-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="91c44-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91c44-112">属性</span><span class="sxs-lookup"><span data-stu-id="91c44-112">Attributes</span></span>

<span data-ttu-id="91c44-113">なし。</span><span class="sxs-lookup"><span data-stu-id="91c44-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91c44-114">子要素</span><span class="sxs-lookup"><span data-stu-id="91c44-114">Child elements</span></span>

<span data-ttu-id="91c44-115">なし。</span><span class="sxs-lookup"><span data-stu-id="91c44-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91c44-116">親要素</span><span class="sxs-lookup"><span data-stu-id="91c44-116">Parent elements</span></span>

|<span data-ttu-id="91c44-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="91c44-117">**Element**</span></span>|<span data-ttu-id="91c44-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="91c44-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91c44-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="91c44-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="91c44-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="91c44-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91c44-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="91c44-121">Text value</span></span>

<span data-ttu-id="91c44-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーの電子メール集計の設定にアクセスするために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="91c44-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91c44-123">注釈</span><span class="sxs-lookup"><span data-stu-id="91c44-123">Remarks</span></span>

<span data-ttu-id="91c44-124">**EcpUrl-aggr**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="91c44-124">The **EcpUrl-aggr** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="91c44-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="91c44-125">See also</span></span>



[<span data-ttu-id="91c44-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="91c44-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

