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
description: RedirectAddr 要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。
ms.openlocfilehash: 6bff28001851f421b4c7429770185401f2f0a743
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529876"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="34fe6-103">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="34fe6-104">**Redirectaddr**要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="34fe6-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="34fe6-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="34fe6-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="34fe6-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="34fe6-108">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="34fe6-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="34fe6-109">Attributes and elements</span></span>

<span data-ttu-id="34fe6-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="34fe6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34fe6-111">属性</span><span class="sxs-lookup"><span data-stu-id="34fe6-111">Attributes</span></span>

<span data-ttu-id="34fe6-112">なし。</span><span class="sxs-lookup"><span data-stu-id="34fe6-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34fe6-113">子要素</span><span class="sxs-lookup"><span data-stu-id="34fe6-113">Child elements</span></span>

<span data-ttu-id="34fe6-114">なし。</span><span class="sxs-lookup"><span data-stu-id="34fe6-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34fe6-115">親要素</span><span class="sxs-lookup"><span data-stu-id="34fe6-115">Parent elements</span></span>

|<span data-ttu-id="34fe6-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="34fe6-116">**Element**</span></span>|<span data-ttu-id="34fe6-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="34fe6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34fe6-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="34fe6-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="34fe6-119">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="34fe6-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="34fe6-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="34fe6-120">Text value</span></span>

<span data-ttu-id="34fe6-121">Text 値は、以降の自動検出要求に使用される電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="34fe6-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34fe6-122">注釈</span><span class="sxs-lookup"><span data-stu-id="34fe6-122">Remarks</span></span>

<span data-ttu-id="34fe6-123">この要素が自動検出応答に存在する場合は、 **Redirectaddr**要素のテキスト値を使用して、別の要求を行います。</span><span class="sxs-lookup"><span data-stu-id="34fe6-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="34fe6-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="34fe6-124">See also</span></span>



[<span data-ttu-id="34fe6-125">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="34fe6-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

