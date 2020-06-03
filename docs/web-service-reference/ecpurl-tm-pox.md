---
title: EcpUrl-tm (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: EcpUrl-tm 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーが現在メンバーであるすべてのサイトメールボックスのリストにアクセスするために使用できる URL を生成するために使用できる URL の一部を指定します。
ms.openlocfilehash: 8d4c787e2eeae5300cd0496f199ea71baace98ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463546"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="f4249-103">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="f4249-104">**EcpUrl-tm**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーが現在メンバーであるすべてのサイトメールボックスのリストにアクセスするために使用できる url を生成するために使用できる url の一部を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4249-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="f4249-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f4249-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f4249-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f4249-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="f4249-109">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f4249-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f4249-110">Attributes and elements</span></span>

<span data-ttu-id="f4249-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4249-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4249-112">属性</span><span class="sxs-lookup"><span data-stu-id="f4249-112">Attributes</span></span>

<span data-ttu-id="f4249-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f4249-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4249-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f4249-114">Child elements</span></span>

<span data-ttu-id="f4249-115">なし。</span><span class="sxs-lookup"><span data-stu-id="f4249-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4249-116">親要素</span><span class="sxs-lookup"><span data-stu-id="f4249-116">Parent elements</span></span>

|<span data-ttu-id="f4249-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4249-117">**Element**</span></span>|<span data-ttu-id="f4249-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4249-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4249-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="f4249-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="f4249-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f4249-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4249-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f4249-121">Text value</span></span>

<span data-ttu-id="f4249-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーのサイトメールボックスのリストにアクセスするために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="f4249-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f4249-123">注釈</span><span class="sxs-lookup"><span data-stu-id="f4249-123">Remarks</span></span>

<span data-ttu-id="f4249-124">**EcpUrl-tm**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="f4249-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f4249-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4249-125">See also</span></span>



[<span data-ttu-id="f4249-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="f4249-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

