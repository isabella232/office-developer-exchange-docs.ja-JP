---
title: SSL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a7e2bdcd-a2f7-45a4-adcd-a03fe7fd4d9b
description: SSL の要素は、セキュリティで保護されたログオンする必要があるかどうかを指定します。
ms.openlocfilehash: 9a51c715032cb2af846e764d28698c5697670d98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833537"
---
# <a name="ssl-pox"></a><span data-ttu-id="1e7ab-103">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-103">SSL (POX)</span></span>

<span data-ttu-id="1e7ab-104">**SSL**の要素は、セキュリティで保護されたログオンする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-104">The **SSL** element specifies whether secure logon is required.</span></span> 
  
[<span data-ttu-id="1e7ab-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="1e7ab-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1e7ab-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1e7ab-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1e7ab-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="1e7ab-109">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-109">SSL (POX)</span></span>](ssl-pox.md)
  
```xml
<SSL>on or off</SSL>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1e7ab-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1e7ab-110">Attributes and elements</span></span>

<span data-ttu-id="1e7ab-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e7ab-112">属性</span><span class="sxs-lookup"><span data-stu-id="1e7ab-112">Attributes</span></span>

<span data-ttu-id="1e7ab-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e7ab-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1e7ab-114">Child elements</span></span>

<span data-ttu-id="1e7ab-115">なし。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e7ab-116">親要素</span><span class="sxs-lookup"><span data-stu-id="1e7ab-116">Parent elements</span></span>

|<span data-ttu-id="1e7ab-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="1e7ab-117">**Element**</span></span>|<span data-ttu-id="1e7ab-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e7ab-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e7ab-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1e7ab-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1e7ab-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e7ab-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1e7ab-121">Text value</span></span>

<span data-ttu-id="1e7ab-122">テキスト値は、セキュリティで保護されたログオンする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-122">The text value specifies whether secure logon is required.</span></span> <span data-ttu-id="1e7ab-123">指定しない場合、既定値は**on**に設定します。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-123">If unspecified, the default value is set to **on**.</span></span> <span data-ttu-id="1e7ab-124">使用可能な値は、**オン**と**オフを**します。</span><span class="sxs-lookup"><span data-stu-id="1e7ab-124">The possible values are **on** and **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1e7ab-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="1e7ab-125">See also</span></span>



[<span data-ttu-id="1e7ab-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1e7ab-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

