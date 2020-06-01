---
title: EcpUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: EcpUrl 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーの予定表の発行設定にアクセスするために使用できる URL を生成できる url の一部を指定します。
ms.openlocfilehash: 98cac9132c1ba6e368be6337fbf3b522a02cb47a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458006"
---
# <a name="ecpurl-publish-pox"></a><span data-ttu-id="d1221-103">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-103">EcpUrl-publish (POX)</span></span>

<span data-ttu-id="d1221-104">**EcpUrl**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの予定表の発行設定にアクセスするために使用できる url を生成できる url の一部を指定します。</span><span class="sxs-lookup"><span data-stu-id="d1221-104">The **EcpUrl-publish** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="d1221-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d1221-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d1221-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d1221-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d1221-109">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-109">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d1221-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d1221-110">Attributes and elements</span></span>

<span data-ttu-id="d1221-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d1221-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1221-112">属性</span><span class="sxs-lookup"><span data-stu-id="d1221-112">Attributes</span></span>

<span data-ttu-id="d1221-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d1221-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1221-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d1221-114">Child elements</span></span>

<span data-ttu-id="d1221-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d1221-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1221-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d1221-116">Parent elements</span></span>

|<span data-ttu-id="d1221-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d1221-117">**Element**</span></span>|<span data-ttu-id="d1221-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1221-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1221-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="d1221-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d1221-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d1221-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1221-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d1221-121">Text value</span></span>

<span data-ttu-id="d1221-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーの予定表の発行設定にアクセスするために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="d1221-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d1221-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d1221-123">Remarks</span></span>

<span data-ttu-id="d1221-124">**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="d1221-124">The **EcpUrl-publish** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d1221-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1221-125">See also</span></span>



[<span data-ttu-id="d1221-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="d1221-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

