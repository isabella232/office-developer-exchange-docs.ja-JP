---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: RedirectAddr 要素は、後の自動検出要求に使用する電子メール アドレスを指定します。
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833020"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="6b18d-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="6b18d-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="6b18d-104">**RedirectAddr**要素は、後の自動検出要求に使用する電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b18d-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="6b18d-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="6b18d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6b18d-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="6b18d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6b18d-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="6b18d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6b18d-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="6b18d-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6b18d-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b18d-109">Attributes and elements</span></span>

<span data-ttu-id="6b18d-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b18d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b18d-111">属性</span><span class="sxs-lookup"><span data-stu-id="6b18d-111">Attributes</span></span>

<span data-ttu-id="6b18d-112">なし。</span><span class="sxs-lookup"><span data-stu-id="6b18d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b18d-113">子要素</span><span class="sxs-lookup"><span data-stu-id="6b18d-113">Child elements</span></span>

<span data-ttu-id="6b18d-114">なし。</span><span class="sxs-lookup"><span data-stu-id="6b18d-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b18d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6b18d-115">Parent elements</span></span>

|<span data-ttu-id="6b18d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b18d-116">**Element**</span></span>|<span data-ttu-id="6b18d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b18d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b18d-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="6b18d-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="6b18d-119">ユーザーのアカウントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b18d-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b18d-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b18d-120">Text value</span></span>

<span data-ttu-id="6b18d-121">テキスト値は、後続の自動検出要求に使用する電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="6b18d-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b18d-122">備考</span><span class="sxs-lookup"><span data-stu-id="6b18d-122">Remarks</span></span>

<span data-ttu-id="6b18d-123">自動検出応答でこの要素がある場合は、 **RedirectAddr**要素のテキスト値を使用して、別の要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="6b18d-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6b18d-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b18d-124">See also</span></span>



[<span data-ttu-id="6b18d-125">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b18d-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

