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
description: Action 要素では、ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760441"
---
# <a name="action-pox"></a><span data-ttu-id="a434f-103">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="a434f-103">Action (POX)</span></span>

<span data-ttu-id="a434f-104">**Action**要素では、ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a434f-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="a434f-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="a434f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="a434f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="a434f-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="a434f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a434f-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="a434f-108">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="a434f-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a434f-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a434f-109">Attributes and elements</span></span>

<span data-ttu-id="a434f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a434f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a434f-111">属性</span><span class="sxs-lookup"><span data-stu-id="a434f-111">Attributes</span></span>

<span data-ttu-id="a434f-112">なし。</span><span class="sxs-lookup"><span data-stu-id="a434f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a434f-113">子要素</span><span class="sxs-lookup"><span data-stu-id="a434f-113">Child elements</span></span>

<span data-ttu-id="a434f-114">なし。</span><span class="sxs-lookup"><span data-stu-id="a434f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a434f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="a434f-115">Parent elements</span></span>

|<span data-ttu-id="a434f-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="a434f-116">**Element**</span></span>|<span data-ttu-id="a434f-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="a434f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a434f-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a434f-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="a434f-119">ユーザーのアカウントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="a434f-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a434f-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a434f-120">Text value</span></span>

<span data-ttu-id="a434f-121">テキスト値は、別の自動検出要求がユーザーの構成情報を取得する必要があるかどうかを表します。</span><span class="sxs-lookup"><span data-stu-id="a434f-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="a434f-122">次の表は、可能な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="a434f-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="a434f-123">**値**</span><span class="sxs-lookup"><span data-stu-id="a434f-123">**Value**</span></span>|<span data-ttu-id="a434f-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="a434f-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a434f-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="a434f-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="a434f-126">この値を指定する場合、 [RedirectUrl (POX)](redirecturl-pox.md)要素はそれ以降の自動検出の要求で使用するクライアント アクセス サーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="a434f-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="a434f-127">クライアント アプリケーションでは、10 リダイレクト後のリダイレクトを停止する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a434f-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="a434f-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="a434f-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="a434f-129">この値を指定する場合、 [RedirectAddr (POX)](redirectaddr-pox.md)要素は後続の自動検出要求に使用する電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="a434f-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="a434f-130">settings</span><span class="sxs-lookup"><span data-stu-id="a434f-130">settings</span></span>  <br/> |<span data-ttu-id="a434f-131">この値を指定する場合、自動検出の応答には、アカウントを構成するために使用する設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a434f-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="a434f-132">[プロトコル (POX)](protocol-pox.md)要素にほとんどの設定が存在します。</span><span class="sxs-lookup"><span data-stu-id="a434f-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a434f-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="a434f-133">See also</span></span>

- [<span data-ttu-id="a434f-134">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a434f-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

