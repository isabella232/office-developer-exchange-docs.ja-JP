---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: EmwsUrl 要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530671"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="2a40f-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="2a40f-104">**Emwsurl**要素は、メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a40f-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="2a40f-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="2a40f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="2a40f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="2a40f-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="2a40f-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2a40f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a40f-110">Attributes and elements</span></span>

<span data-ttu-id="2a40f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a40f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a40f-112">属性</span><span class="sxs-lookup"><span data-stu-id="2a40f-112">Attributes</span></span>

<span data-ttu-id="2a40f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2a40f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a40f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2a40f-114">Child elements</span></span>

<span data-ttu-id="2a40f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2a40f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a40f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2a40f-116">Parent elements</span></span>

|<span data-ttu-id="2a40f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a40f-117">**Element**</span></span>|<span data-ttu-id="2a40f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a40f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a40f-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="2a40f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="2a40f-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a40f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a40f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2a40f-121">Text value</span></span>

<span data-ttu-id="2a40f-122">Text 値は、ユーザーの EWS エンドポイントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="2a40f-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="2a40f-123">[Ewsurl (POX)](ewsurl-pox.md)要素と同じです。</span><span class="sxs-lookup"><span data-stu-id="2a40f-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2a40f-124">注釈</span><span class="sxs-lookup"><span data-stu-id="2a40f-124">Remarks</span></span>

<span data-ttu-id="2a40f-125">**Emwsurl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="2a40f-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2a40f-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a40f-126">See also</span></span>

- [<span data-ttu-id="2a40f-127">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a40f-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

