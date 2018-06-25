---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: EmwsUrl 要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760270"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="8c017-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="8c017-104">**EmwsUrl**要素は、メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c017-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="8c017-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="8c017-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="8c017-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="8c017-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="8c017-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="8c017-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8c017-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8c017-110">Attributes and elements</span></span>

<span data-ttu-id="8c017-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8c017-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c017-112">属性</span><span class="sxs-lookup"><span data-stu-id="8c017-112">Attributes</span></span>

<span data-ttu-id="8c017-113">なし。</span><span class="sxs-lookup"><span data-stu-id="8c017-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c017-114">子要素</span><span class="sxs-lookup"><span data-stu-id="8c017-114">Child elements</span></span>

<span data-ttu-id="8c017-115">なし。</span><span class="sxs-lookup"><span data-stu-id="8c017-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8c017-116">親要素</span><span class="sxs-lookup"><span data-stu-id="8c017-116">Parent elements</span></span>

|<span data-ttu-id="8c017-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="8c017-117">**Element**</span></span>|<span data-ttu-id="8c017-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="8c017-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c017-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="8c017-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8c017-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8c017-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8c017-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8c017-121">Text value</span></span>

<span data-ttu-id="8c017-122">テキスト値は、ユーザーの EWS のエンドポイントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="8c017-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="8c017-123">[EwsUrl (POX)](ewsurl-pox.md)の要素と同じであります。</span><span class="sxs-lookup"><span data-stu-id="8c017-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8c017-124">備考</span><span class="sxs-lookup"><span data-stu-id="8c017-124">Remarks</span></span>

<span data-ttu-id="8c017-125">**EmwsUrl**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="8c017-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8c017-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="8c017-126">See also</span></span>

- [<span data-ttu-id="8c017-127">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8c017-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

