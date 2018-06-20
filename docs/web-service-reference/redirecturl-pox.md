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
description: RedirectUrl 要素には、クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833027"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="1affd-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1affd-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="1affd-104">**RedirectUrl**要素には、クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Microsoft Exchange Server 2007 を実行しているコンピューターの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1affd-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="1affd-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="1affd-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1affd-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1affd-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1affd-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1affd-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1affd-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1affd-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1affd-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1affd-109">Attributes and elements</span></span>

<span data-ttu-id="1affd-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1affd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1affd-111">属性</span><span class="sxs-lookup"><span data-stu-id="1affd-111">Attributes</span></span>

<span data-ttu-id="1affd-112">なし。</span><span class="sxs-lookup"><span data-stu-id="1affd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1affd-113">子要素</span><span class="sxs-lookup"><span data-stu-id="1affd-113">Child elements</span></span>

<span data-ttu-id="1affd-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1affd-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1affd-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1affd-115">Parent elements</span></span>

|<span data-ttu-id="1affd-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1affd-116">**Element**</span></span>|<span data-ttu-id="1affd-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1affd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1affd-118">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1affd-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="1affd-119">ユーザーのアカウントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="1affd-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1affd-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1affd-120">Text value</span></span>

<span data-ttu-id="1affd-121">テキスト値は、自動検出の設定を取得するために使用する必要がありますクライアント アクセス サーバーの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="1affd-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1affd-122">備考</span><span class="sxs-lookup"><span data-stu-id="1affd-122">Remarks</span></span>

<span data-ttu-id="1affd-123">クライアント アプリケーションでは、10 リダイレクト後のリダイレクトを停止する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1affd-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1affd-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="1affd-124">See also</span></span>



[<span data-ttu-id="1affd-125">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1affd-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

