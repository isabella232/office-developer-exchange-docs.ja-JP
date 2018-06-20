---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: DeploymentId 要素は、Microsoft Exchange Server 2007 のフォレストを一意に識別します。
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760011"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="7cd6b-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="7cd6b-103">DeploymentId (POX)</span></span>

<span data-ttu-id="7cd6b-104">**DeploymentId**要素は、Microsoft Exchange Server 2007 のフォレストを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="7cd6b-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="7cd6b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="7cd6b-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="7cd6b-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="7cd6b-107">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="7cd6b-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="7cd6b-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="7cd6b-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7cd6b-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7cd6b-109">Attributes and elements</span></span>

<span data-ttu-id="7cd6b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cd6b-111">属性</span><span class="sxs-lookup"><span data-stu-id="7cd6b-111">Attributes</span></span>

<span data-ttu-id="7cd6b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cd6b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="7cd6b-113">Child elements</span></span>

<span data-ttu-id="7cd6b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7cd6b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7cd6b-115">Parent elements</span></span>

|<span data-ttu-id="7cd6b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7cd6b-116">**Element**</span></span>|<span data-ttu-id="7cd6b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7cd6b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cd6b-118">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="7cd6b-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="7cd6b-119">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cd6b-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7cd6b-120">Text value</span></span>

<span data-ttu-id="7cd6b-121">テキスト値は、Exchange 2007 フォレストでは、GUID の形式を一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cd6b-122">備考</span><span class="sxs-lookup"><span data-stu-id="7cd6b-122">Remarks</span></span>

<span data-ttu-id="7cd6b-123">アンインストールし、Exchange 2007 を再インストールし、同じサーバー名を使用すると、 **DeploymentId**の値を変更します。</span><span class="sxs-lookup"><span data-stu-id="7cd6b-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7cd6b-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="7cd6b-124">See also</span></span>

- [<span data-ttu-id="7cd6b-125">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7cd6b-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

