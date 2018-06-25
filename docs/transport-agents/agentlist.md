---
title: agentList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentList
api_type:
- schema
ms.assetid: e877b7ef-e303-4270-964d-8d116ff2a865
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 7dd9d48356932c82dbc048a85b9f02437c6366de
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759227"
---
# <a name="agentlist"></a><span data-ttu-id="84155-103">agentList</span><span class="sxs-lookup"><span data-stu-id="84155-103">agentList</span></span>
  
<span data-ttu-id="84155-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="84155-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="84155-105">**AgentList**要素には、インストールされている各エージェントの[エージェント](agent.md)の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="84155-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="84155-106">構成</span><span class="sxs-lookup"><span data-stu-id="84155-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="84155-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="84155-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="84155-108">agentList</span><span class="sxs-lookup"><span data-stu-id="84155-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="84155-109">**agentListType (複合型)**</span><span class="sxs-lookup"><span data-stu-id="84155-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="84155-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="84155-110">Attributes and elements</span></span>

<span data-ttu-id="84155-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="84155-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84155-112">属性</span><span class="sxs-lookup"><span data-stu-id="84155-112">Attributes</span></span>

<span data-ttu-id="84155-113">なし。</span><span class="sxs-lookup"><span data-stu-id="84155-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84155-114">子要素</span><span class="sxs-lookup"><span data-stu-id="84155-114">Child elements</span></span>

|<span data-ttu-id="84155-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="84155-115">**Element**</span></span>|<span data-ttu-id="84155-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="84155-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84155-117">エージェント</span><span class="sxs-lookup"><span data-stu-id="84155-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="84155-118">インストールされているエージェントの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="84155-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="84155-119">親要素</span><span class="sxs-lookup"><span data-stu-id="84155-119">Parent elements</span></span>

|<span data-ttu-id="84155-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="84155-120">**Element**</span></span>|<span data-ttu-id="84155-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="84155-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84155-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="84155-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="84155-123">エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントに関する構成情報を定義する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="84155-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="84155-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="84155-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84155-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="84155-125">Namespace</span></span>  <br/> |<span data-ttu-id="84155-126">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="84155-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="84155-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="84155-127">Schema Name</span></span>  <br/> |<span data-ttu-id="84155-128">該当なし。</span><span class="sxs-lookup"><span data-stu-id="84155-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="84155-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="84155-129">Validation File</span></span>  <br/> |<span data-ttu-id="84155-130">該当なし。</span><span class="sxs-lookup"><span data-stu-id="84155-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="84155-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="84155-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="84155-132">False。</span><span class="sxs-lookup"><span data-stu-id="84155-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84155-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="84155-133">See also</span></span>

- [<span data-ttu-id="84155-134">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="84155-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

