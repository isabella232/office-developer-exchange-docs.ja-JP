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
description: DeploymentId 要素は、Microsoft Exchange Server 2007 フォレストを一意に識別します。
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467922"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="577d8-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-103">DeploymentId (POX)</span></span>

<span data-ttu-id="577d8-104">**DeploymentId**要素は、Microsoft Exchange Server 2007 フォレストを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="577d8-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="577d8-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="577d8-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="577d8-107">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="577d8-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="577d8-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="577d8-109">Attributes and elements</span></span>

<span data-ttu-id="577d8-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="577d8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="577d8-111">属性</span><span class="sxs-lookup"><span data-stu-id="577d8-111">Attributes</span></span>

<span data-ttu-id="577d8-112">なし。</span><span class="sxs-lookup"><span data-stu-id="577d8-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="577d8-113">子要素</span><span class="sxs-lookup"><span data-stu-id="577d8-113">Child elements</span></span>

<span data-ttu-id="577d8-114">なし。</span><span class="sxs-lookup"><span data-stu-id="577d8-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="577d8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="577d8-115">Parent elements</span></span>

|<span data-ttu-id="577d8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="577d8-116">**Element**</span></span>|<span data-ttu-id="577d8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="577d8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="577d8-118">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="577d8-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="577d8-119">ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="577d8-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="577d8-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="577d8-120">Text value</span></span>

<span data-ttu-id="577d8-121">Text 値は、Exchange 2007 フォレストを GUID 形式で一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="577d8-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="577d8-122">注釈</span><span class="sxs-lookup"><span data-stu-id="577d8-122">Remarks</span></span>

<span data-ttu-id="577d8-123">Exchange 2007 をアンインストールしてから再インストールし、同じサーバー名を使用すると、 **DeploymentId**値が変更されます。</span><span class="sxs-lookup"><span data-stu-id="577d8-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="577d8-124">関連項目</span><span class="sxs-lookup"><span data-stu-id="577d8-124">See also</span></span>

- [<span data-ttu-id="577d8-125">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="577d8-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

