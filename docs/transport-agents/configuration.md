---
title: 環境
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
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: b886851b9a0c17d58428f49281d664930d0e4070
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461563"
---
# <a name="configuration"></a><span data-ttu-id="401ea-103">環境</span><span class="sxs-lookup"><span data-stu-id="401ea-103">configuration</span></span>
  
<span data-ttu-id="401ea-104">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="401ea-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="401ea-105">**configuration** 要素は、エージェント構成ファイルのルート要素です。</span><span class="sxs-lookup"><span data-stu-id="401ea-105">The **configuration** element is the root element for the agents configuration file.</span></span> 
  
- [<span data-ttu-id="401ea-106">構成</span><span class="sxs-lookup"><span data-stu-id="401ea-106">configuration</span></span>](configuration.md) 
- [<span data-ttu-id="401ea-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="401ea-107">mexRuntime</span></span>](mexruntime.md)
  
```XML
<configuration>
      <mexRuntime/>
</configuration>
```

<span data-ttu-id="401ea-108">**configurationType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="401ea-108">**configurationType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="401ea-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="401ea-109">Attributes and elements</span></span>

<span data-ttu-id="401ea-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="401ea-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="401ea-111">属性</span><span class="sxs-lookup"><span data-stu-id="401ea-111">Attributes</span></span>

<span data-ttu-id="401ea-112">なし。</span><span class="sxs-lookup"><span data-stu-id="401ea-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="401ea-113">子要素</span><span class="sxs-lookup"><span data-stu-id="401ea-113">Child elements</span></span>

|<span data-ttu-id="401ea-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="401ea-114">**Element**</span></span>|<span data-ttu-id="401ea-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="401ea-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="401ea-116">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="401ea-116">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="401ea-117">エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントの SMTP およびルーティングに関する構成情報を定義する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="401ea-117">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="401ea-118">親要素</span><span class="sxs-lookup"><span data-stu-id="401ea-118">Parent elements</span></span>

<span data-ttu-id="401ea-119">なし。</span><span class="sxs-lookup"><span data-stu-id="401ea-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="401ea-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="401ea-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="401ea-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="401ea-121">Namespace</span></span>  <br/> |<span data-ttu-id="401ea-122">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="401ea-122">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="401ea-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="401ea-123">Schema Name</span></span>  <br/> |<span data-ttu-id="401ea-124">注意事項なし。</span><span class="sxs-lookup"><span data-stu-id="401ea-124">Not available.</span></span>  <br/> |
|<span data-ttu-id="401ea-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="401ea-125">Validation File</span></span>  <br/> |<span data-ttu-id="401ea-126">該当なし。</span><span class="sxs-lookup"><span data-stu-id="401ea-126">Not available.</span></span>  <br/> |
|<span data-ttu-id="401ea-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="401ea-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="401ea-128">不正解。</span><span class="sxs-lookup"><span data-stu-id="401ea-128">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="401ea-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="401ea-129">See also</span></span>

- [<span data-ttu-id="401ea-130">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="401ea-130">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

