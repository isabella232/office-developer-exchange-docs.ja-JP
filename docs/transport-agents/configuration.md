---
title: 構成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- configuration
api_type:
- schema
ms.assetid: 6fc04e4d-657a-4999-9431-186ccb7832b5
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 342e52e879534b6a130d286d358138c6095e4563
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759229"
---
# <a name="configuration"></a><span data-ttu-id="3a4c4-103">configuration</span><span class="sxs-lookup"><span data-stu-id="3a4c4-103">configuration</span></span>
  
<span data-ttu-id="3a4c4-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3a4c4-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="3a4c4-105">**構成**要素は、エージェント構成ファイルのルート要素です。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="3a4c4-106">構成</span><span class="sxs-lookup"><span data-stu-id="3a4c4-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="3a4c4-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="3a4c4-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="3a4c4-108">**configurationType (複合型)**</span><span class="sxs-lookup"><span data-stu-id="3a4c4-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3a4c4-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a4c4-109">Attributes and elements</span></span>

<span data-ttu-id="3a4c4-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a4c4-111">属性</span><span class="sxs-lookup"><span data-stu-id="3a4c4-111">Attributes</span></span>

<span data-ttu-id="3a4c4-112">なし。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a4c4-113">子要素</span><span class="sxs-lookup"><span data-stu-id="3a4c4-113">Child elements</span></span>

|<span data-ttu-id="3a4c4-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a4c4-114">**Element**</span></span>|<span data-ttu-id="3a4c4-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a4c4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a4c4-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="3a4c4-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="3a4c4-117">エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントの SMTP およびルーティングに関する構成情報を定義する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a4c4-118">親要素</span><span class="sxs-lookup"><span data-stu-id="3a4c4-118">Parent elements</span></span>

<span data-ttu-id="3a4c4-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a4c4-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="3a4c4-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a4c4-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="3a4c4-121">Namespace</span></span>  <br/> |<span data-ttu-id="3a4c4-122">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="3a4c4-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a4c4-123">Schema Name</span></span>  <br/> |<span data-ttu-id="3a4c4-124">該当なし。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="3a4c4-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a4c4-125">Validation File</span></span>  <br/> |<span data-ttu-id="3a4c4-126">該当なし。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="3a4c4-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3a4c4-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a4c4-128">False。</span><span class="sxs-lookup"><span data-stu-id="3a4c4-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a4c4-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a4c4-129">See also</span></span>

- [<span data-ttu-id="3a4c4-130">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="3a4c4-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

