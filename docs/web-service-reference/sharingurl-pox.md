---
title: SharingUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: d590188a-5aa6-46c6-ab5f-2a0dd6793109
description: SharingUrl 要素には、予定表と連絡先を組織間で共有するために使用される共有サーバーの URL が含まれています。
ms.openlocfilehash: 9c793935808dbd20d2dc0631b82ee74db3f8a19f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465255"
---
# <a name="sharingurl-pox"></a><span data-ttu-id="1f09f-103">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-103">SharingUrl (POX)</span></span>

<span data-ttu-id="1f09f-104">**Sharingurl**要素には、予定表と連絡先を組織間で共有するために使用される共有サーバーの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f09f-104">The **SharingUrl** element contains the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span> 
  
[<span data-ttu-id="1f09f-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1f09f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1f09f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1f09f-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="1f09f-109">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-109">SharingUrl (POX)</span></span>](sharingurl-pox.md)
  
```XML
<SharingUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1f09f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f09f-110">Attributes and elements</span></span>

<span data-ttu-id="1f09f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f09f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f09f-112">属性</span><span class="sxs-lookup"><span data-stu-id="1f09f-112">Attributes</span></span>

<span data-ttu-id="1f09f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1f09f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f09f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1f09f-114">Child elements</span></span>

<span data-ttu-id="1f09f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="1f09f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f09f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="1f09f-116">Parent elements</span></span>

|<span data-ttu-id="1f09f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f09f-117">**Element**</span></span>|<span data-ttu-id="1f09f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f09f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f09f-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1f09f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1f09f-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f09f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f09f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1f09f-121">Text value</span></span>

<span data-ttu-id="1f09f-122">Text 値は、予定表と連絡先を組織間で共有するために使用される共有サーバーの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="1f09f-122">The text value represents the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f09f-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1f09f-123">Remarks</span></span>

<span data-ttu-id="1f09f-124">**Sharingurl**要素は、**プロトコル**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="1f09f-124">The **SharingUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1f09f-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f09f-125">See also</span></span>



[<span data-ttu-id="1f09f-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f09f-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

