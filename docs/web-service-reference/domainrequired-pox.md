---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: DomainRequired 要素は、ドメインが認証に必要かどうかを示します。
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461325"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="752e7-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-103">DomainRequired (POX)</span></span>

<span data-ttu-id="752e7-104">**Domainrequired**要素は、ドメインが認証に必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="752e7-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="752e7-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="752e7-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="752e7-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="752e7-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="752e7-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="752e7-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="752e7-110">Attributes and elements</span></span>

<span data-ttu-id="752e7-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="752e7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="752e7-112">属性</span><span class="sxs-lookup"><span data-stu-id="752e7-112">Attributes</span></span>

<span data-ttu-id="752e7-113">なし。</span><span class="sxs-lookup"><span data-stu-id="752e7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="752e7-114">子要素</span><span class="sxs-lookup"><span data-stu-id="752e7-114">Child elements</span></span>

<span data-ttu-id="752e7-115">なし。</span><span class="sxs-lookup"><span data-stu-id="752e7-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="752e7-116">親要素</span><span class="sxs-lookup"><span data-stu-id="752e7-116">Parent elements</span></span>

|<span data-ttu-id="752e7-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="752e7-117">**Element**</span></span>|<span data-ttu-id="752e7-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="752e7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="752e7-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="752e7-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="752e7-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="752e7-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="752e7-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="752e7-121">Text value</span></span>

<span data-ttu-id="752e7-122">Text 値は、ドメインが認証に必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="752e7-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="752e7-123">有効な値は、 **[オン**] または [**オフ**] です。</span><span class="sxs-lookup"><span data-stu-id="752e7-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="752e7-124">値が**on**の場合、以降の要求にはユーザーのアカウントのドメインが含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="752e7-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="752e7-125">注釈</span><span class="sxs-lookup"><span data-stu-id="752e7-125">Remarks</span></span>

<span data-ttu-id="752e7-126">ドメインが[POX (ログイン)](loginname-pox.md)要素で指定されていない場合、または要素が指定さ**れてい**ない場合は、認証が成功する前に、ユーザーはドメインを入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="752e7-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="752e7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="752e7-127">See also</span></span>

- [<span data-ttu-id="752e7-128">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="752e7-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

