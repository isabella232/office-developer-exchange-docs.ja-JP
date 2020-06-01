---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: RedirectUrl 要素には、Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。これにより、クライアントアクセスサーバーの役割がインストールされており、自動検出の設定を取得するために使用する必要があります。
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468090"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="c3285-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="c3285-104">**Redirecturl**要素には、Microsoft Exchange server 2007 を実行しているコンピューターの URL が含まれています。これにより、クライアントアクセスサーバーの役割がインストールされており、自動検出の設定を取得するために使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3285-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="c3285-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c3285-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c3285-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c3285-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c3285-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c3285-109">Attributes and elements</span></span>

<span data-ttu-id="c3285-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c3285-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c3285-111">属性</span><span class="sxs-lookup"><span data-stu-id="c3285-111">Attributes</span></span>

<span data-ttu-id="c3285-112">なし。</span><span class="sxs-lookup"><span data-stu-id="c3285-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c3285-113">子要素</span><span class="sxs-lookup"><span data-stu-id="c3285-113">Child elements</span></span>

<span data-ttu-id="c3285-114">なし。</span><span class="sxs-lookup"><span data-stu-id="c3285-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c3285-115">親要素</span><span class="sxs-lookup"><span data-stu-id="c3285-115">Parent elements</span></span>

|<span data-ttu-id="c3285-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="c3285-116">**Element**</span></span>|<span data-ttu-id="c3285-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="c3285-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c3285-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="c3285-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="c3285-119">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3285-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c3285-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c3285-120">Text value</span></span>

<span data-ttu-id="c3285-121">Text 値は、自動検出設定を取得するために使用するクライアントアクセスサーバーの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="c3285-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c3285-122">注釈</span><span class="sxs-lookup"><span data-stu-id="c3285-122">Remarks</span></span>

<span data-ttu-id="c3285-123">クライアントアプリケーションは、10回リダイレクトした後にリダイレクトを停止する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3285-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c3285-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="c3285-124">See also</span></span>



[<span data-ttu-id="c3285-125">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="c3285-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

