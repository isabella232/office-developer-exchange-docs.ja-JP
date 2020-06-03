---
title: 応答 (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 002b72f2-f94d-467c-8e6c-b3818f7e51dc
description: '適用対象:'
ms.openlocfilehash: 30f6a5c2c6e3034fde8849ab1fced3519029b1f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448976"
---
# <a name="response-pox"></a><span data-ttu-id="118ee-103">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-103">Response (POX)</span></span>


  
<span data-ttu-id="118ee-104">**Response**要素には、自動検出サービスからの応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="118ee-104">The **Response** element contains the response from the Autodiscover service.</span></span> 
  
[<span data-ttu-id="118ee-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="118ee-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-106">Response (POX)</span></span>](response-pox.md)
  
```xml
<Response>
   <User/>
   <Account/>
</Response>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="118ee-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="118ee-107">Attributes and elements</span></span>

<span data-ttu-id="118ee-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="118ee-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="118ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="118ee-109">Attributes</span></span>

<span data-ttu-id="118ee-110">なし。</span><span class="sxs-lookup"><span data-stu-id="118ee-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="118ee-111">子要素</span><span class="sxs-lookup"><span data-stu-id="118ee-111">Child elements</span></span>

|<span data-ttu-id="118ee-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="118ee-112">**Element**</span></span>|<span data-ttu-id="118ee-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="118ee-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="118ee-114">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-114">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="118ee-115">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="118ee-115">Provides user-specific information.</span></span> <span data-ttu-id="118ee-116">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="118ee-116">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="118ee-117">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-117">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="118ee-118">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="118ee-118">Specifies account settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="118ee-119">親要素</span><span class="sxs-lookup"><span data-stu-id="118ee-119">Parent elements</span></span>

|<span data-ttu-id="118ee-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="118ee-120">**Element**</span></span>|<span data-ttu-id="118ee-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="118ee-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="118ee-122">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="118ee-122">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="118ee-123">自動検出応答のルート要素。</span><span class="sxs-lookup"><span data-stu-id="118ee-123">The root element in an Autodiscover response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="118ee-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="118ee-124">See also</span></span>



[<span data-ttu-id="118ee-125">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="118ee-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

