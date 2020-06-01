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
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: 99e4e24c3bca77c7e7d5f2c59bb21cee1317fed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44446393"
---
# <a name="agentlist"></a><span data-ttu-id="c7a0b-103">agentList</span><span class="sxs-lookup"><span data-stu-id="c7a0b-103">agentList</span></span>
  
<span data-ttu-id="c7a0b-104">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c7a0b-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="c7a0b-105">**agentList** 要素には、インストールされた各エージェントに [agent](agent.md) 要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-105">The **agentList** element contains an [agent](agent.md) element for each installed agent.</span></span> 
  
- [<span data-ttu-id="c7a0b-106">構成</span><span class="sxs-lookup"><span data-stu-id="c7a0b-106">configuration</span></span>](configuration.md)
- [<span data-ttu-id="c7a0b-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="c7a0b-107">mexRuntime</span></span>](mexruntime.md)
- [<span data-ttu-id="c7a0b-108">agentList</span><span class="sxs-lookup"><span data-stu-id="c7a0b-108">agentList</span></span>](agentlist.md)
  
```XML
<agentList>
      <agent/>
</agentList>
```

<span data-ttu-id="c7a0b-109">**agentListType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="c7a0b-109">**agentListType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c7a0b-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c7a0b-110">Attributes and elements</span></span>

<span data-ttu-id="c7a0b-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7a0b-112">属性</span><span class="sxs-lookup"><span data-stu-id="c7a0b-112">Attributes</span></span>

<span data-ttu-id="c7a0b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7a0b-114">子要素</span><span class="sxs-lookup"><span data-stu-id="c7a0b-114">Child elements</span></span>

|<span data-ttu-id="c7a0b-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="c7a0b-115">**Element**</span></span>|<span data-ttu-id="c7a0b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7a0b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7a0b-117">agent</span><span class="sxs-lookup"><span data-stu-id="c7a0b-117">agent</span></span>](agent.md) <br/> |<span data-ttu-id="c7a0b-118">インストールされているエージェントの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-118">Contains configuration information about an installed agent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7a0b-119">親要素</span><span class="sxs-lookup"><span data-stu-id="c7a0b-119">Parent elements</span></span>

|<span data-ttu-id="c7a0b-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="c7a0b-120">**Element**</span></span>|<span data-ttu-id="c7a0b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="c7a0b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7a0b-122">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="c7a0b-122">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="c7a0b-123">エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントに関する構成情報を定義する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-123">Contains elements that define configuration information for agent monitoring and configuration information about installed agents.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c7a0b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c7a0b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7a0b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7a0b-125">Namespace</span></span>  <br/> |<span data-ttu-id="c7a0b-126">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-126">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="c7a0b-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c7a0b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c7a0b-128">注意事項なし。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-128">Not available.</span></span>  <br/> |
|<span data-ttu-id="c7a0b-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c7a0b-129">Validation File</span></span>  <br/> |<span data-ttu-id="c7a0b-130">該当なし。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="c7a0b-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c7a0b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7a0b-132">不正解。</span><span class="sxs-lookup"><span data-stu-id="c7a0b-132">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7a0b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="c7a0b-133">See also</span></span>

- [<span data-ttu-id="c7a0b-134">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="c7a0b-134">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

