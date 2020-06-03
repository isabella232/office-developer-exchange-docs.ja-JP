---
title: アクション (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Action 要素は、ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。
ms.openlocfilehash: f6d542b908948d09020b850b60ca1bdb025dd342
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529694"
---
# <a name="action-pox"></a><span data-ttu-id="150a9-103">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-103">Action (POX)</span></span>

<span data-ttu-id="150a9-104">**Action**要素は、ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="150a9-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="150a9-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="150a9-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="150a9-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="150a9-108">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="150a9-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="150a9-109">Attributes and elements</span></span>

<span data-ttu-id="150a9-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="150a9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="150a9-111">属性</span><span class="sxs-lookup"><span data-stu-id="150a9-111">Attributes</span></span>

<span data-ttu-id="150a9-112">なし。</span><span class="sxs-lookup"><span data-stu-id="150a9-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="150a9-113">子要素</span><span class="sxs-lookup"><span data-stu-id="150a9-113">Child elements</span></span>

<span data-ttu-id="150a9-114">なし。</span><span class="sxs-lookup"><span data-stu-id="150a9-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="150a9-115">親要素</span><span class="sxs-lookup"><span data-stu-id="150a9-115">Parent elements</span></span>

|<span data-ttu-id="150a9-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="150a9-116">**Element**</span></span>|<span data-ttu-id="150a9-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="150a9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="150a9-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="150a9-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="150a9-119">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="150a9-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="150a9-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="150a9-120">Text value</span></span>

<span data-ttu-id="150a9-121">Text 値は、ユーザーの構成情報を取得するために別の自動検出要求が必要かどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="150a9-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="150a9-122">次の表に、使用可能な値を示します。</span><span class="sxs-lookup"><span data-stu-id="150a9-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="150a9-123">**値**</span><span class="sxs-lookup"><span data-stu-id="150a9-123">**Value**</span></span>|<span data-ttu-id="150a9-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="150a9-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="150a9-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="150a9-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="150a9-126">この値が指定されている場合、 [Redirecturl (POX)](redirecturl-pox.md)要素は、以降の自動検出要求で使用されるクライアントアクセスサーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="150a9-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="150a9-127">クライアントアプリケーションは、10回リダイレクトした後にリダイレクトを停止する必要があります。</span><span class="sxs-lookup"><span data-stu-id="150a9-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="150a9-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="150a9-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="150a9-129">この値が指定されている場合、 [Redirectaddr (POX)](redirectaddr-pox.md)要素は、以降の自動検出要求に使用する電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="150a9-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="150a9-130">設定</span><span class="sxs-lookup"><span data-stu-id="150a9-130">settings</span></span>  <br/> |<span data-ttu-id="150a9-131">この値が指定されている場合、自動検出応答には、アカウントの構成に使用される設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="150a9-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="150a9-132">ほとんどの設定は[Protocol (POX)](protocol-pox.md)要素にあります。</span><span class="sxs-lookup"><span data-stu-id="150a9-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="150a9-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="150a9-133">See also</span></span>

- [<span data-ttu-id="150a9-134">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="150a9-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

