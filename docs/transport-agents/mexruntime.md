---
title: mexRuntime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- mexRuntime
api_type:
- schema
ms.assetid: eabb2f12-10a7-4ce2-ae4b-9c04010c765f
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 4a34eedfc16d64cbfa67003ed23cf6eba2bb4bad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759259"
---
# <a name="mexruntime"></a><span data-ttu-id="5b56b-103">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="5b56b-103">mexRuntime</span></span>
  
<span data-ttu-id="5b56b-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5b56b-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="5b56b-105">**MexRuntime**要素には、監視エージェントの構成情報および SMTP およびインストールされているルーティング エージェントの構成情報を定義する要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b56b-105">The **mexRuntime** element contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span> 
  
- [<span data-ttu-id="5b56b-106">構成</span><span class="sxs-lookup"><span data-stu-id="5b56b-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="5b56b-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="5b56b-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<mexRuntime>
   <monitoring/>
   <agentList/>
</mexRuntime>
```

<span data-ttu-id="5b56b-108">**mexRuntimeType (複合型)**</span><span class="sxs-lookup"><span data-stu-id="5b56b-108">**mexRuntimeType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5b56b-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5b56b-109">Attributes and elements</span></span>

<span data-ttu-id="5b56b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b56b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b56b-111">属性</span><span class="sxs-lookup"><span data-stu-id="5b56b-111">Attributes</span></span>

<span data-ttu-id="5b56b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="5b56b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b56b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="5b56b-113">Child elements</span></span>

|<span data-ttu-id="5b56b-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="5b56b-114">**Element**</span></span>|<span data-ttu-id="5b56b-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b56b-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b56b-116">監視</span><span class="sxs-lookup"><span data-stu-id="5b56b-116">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="5b56b-117">トランスポートがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b56b-117">Contains configuration information that defines how and when transport monitors agents that are installed.</span></span>  <br/> |
|[<span data-ttu-id="5b56b-118">agentList</span><span class="sxs-lookup"><span data-stu-id="5b56b-118">agentList</span></span>](agentlist.md) <br/> |<span data-ttu-id="5b56b-119">インストールされている各エージェントの[エージェント](agent.md)の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b56b-119">Contains an [agent](agent.md) element for each agent that is installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b56b-120">親要素</span><span class="sxs-lookup"><span data-stu-id="5b56b-120">Parent elements</span></span>

|<span data-ttu-id="5b56b-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="5b56b-121">**Element**</span></span>|<span data-ttu-id="5b56b-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b56b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b56b-123">構成</span><span class="sxs-lookup"><span data-stu-id="5b56b-123">configuration</span></span>](configuration.md) <br/> |<span data-ttu-id="5b56b-124">エージェント構成ファイルのルート要素です。</span><span class="sxs-lookup"><span data-stu-id="5b56b-124">The root element for the agents configuration file.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="5b56b-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="5b56b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b56b-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="5b56b-126">Namespace</span></span>  <br/> |<span data-ttu-id="5b56b-127">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="5b56b-127">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="5b56b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b56b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5b56b-129">該当なし。</span><span class="sxs-lookup"><span data-stu-id="5b56b-129">Not available.</span></span>  <br/> |
|<span data-ttu-id="5b56b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b56b-130">Validation File</span></span>  <br/> |<span data-ttu-id="5b56b-131">該当なし。</span><span class="sxs-lookup"><span data-stu-id="5b56b-131">Not available.</span></span>  <br/> |
|<span data-ttu-id="5b56b-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5b56b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b56b-133">False。</span><span class="sxs-lookup"><span data-stu-id="5b56b-133">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b56b-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b56b-134">See also</span></span>

- [<span data-ttu-id="5b56b-135">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="5b56b-135">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

