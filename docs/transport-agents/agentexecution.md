---
title: agentExecution
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agentExecution
api_type:
- schema
ms.assetid: 600c4690-941c-45af-a906-5528748d09cd
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 5848d52a68c8c3f747614015e49becb34bc4cfd8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759225"
---
# <a name="agentexecution"></a><span data-ttu-id="f92c9-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="f92c9-103">agentExecution</span></span>
  
<span data-ttu-id="f92c9-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f92c9-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="f92c9-105">**AgentExecution**要素は、エージェントがイベント ログに書き込む前にイベントを終了するまで待機するか、クライアント アクセス、メールボックス サーバーをミリ秒単位で時間を定義します。</span><span class="sxs-lookup"><span data-stu-id="f92c9-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="f92c9-106">構成</span><span class="sxs-lookup"><span data-stu-id="f92c9-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="f92c9-107">監視</span><span class="sxs-lookup"><span data-stu-id="f92c9-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="f92c9-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="f92c9-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="f92c9-109">**agentExecutionType (複合型)**</span><span class="sxs-lookup"><span data-stu-id="f92c9-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f92c9-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f92c9-110">Attributes and elements</span></span>

<span data-ttu-id="f92c9-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f92c9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f92c9-112">属性</span><span class="sxs-lookup"><span data-stu-id="f92c9-112">Attributes</span></span>

|<span data-ttu-id="f92c9-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="f92c9-113">**Attribute**</span></span>|<span data-ttu-id="f92c9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f92c9-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f92c9-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="f92c9-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="f92c9-p101">エージェントのイベントからの復帰をサーバーが待機する時間をミリ秒単位で指定する正の整数値。この時間を過ぎるとイベント ログに警告が書き込まれます。この値が小さすぎると、パフォーマンスが低下することがあります。この属性の推奨値は、5 分間に相当する 300,000 です。</span><span class="sxs-lookup"><span data-stu-id="f92c9-p101">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log. Performance can decrease if this value is too small. The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f92c9-119">子要素</span><span class="sxs-lookup"><span data-stu-id="f92c9-119">Child elements</span></span>

<span data-ttu-id="f92c9-120">なし。</span><span class="sxs-lookup"><span data-stu-id="f92c9-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f92c9-121">親要素</span><span class="sxs-lookup"><span data-stu-id="f92c9-121">Parent elements</span></span>

|<span data-ttu-id="f92c9-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="f92c9-122">**Element**</span></span>|<span data-ttu-id="f92c9-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="f92c9-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f92c9-124">監視</span><span class="sxs-lookup"><span data-stu-id="f92c9-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="f92c9-125">インストールされているエージェントをフロント エンド トランスポート サービスまたはトランスポート サービスが監視する方法とタイミングを定義する構成情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="f92c9-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="f92c9-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="f92c9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f92c9-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="f92c9-127">Namespace</span></span>  <br/> |<span data-ttu-id="f92c9-128">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="f92c9-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="f92c9-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f92c9-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f92c9-130">該当なし。</span><span class="sxs-lookup"><span data-stu-id="f92c9-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="f92c9-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f92c9-131">Validation File</span></span>  <br/> |<span data-ttu-id="f92c9-132">該当なし。</span><span class="sxs-lookup"><span data-stu-id="f92c9-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="f92c9-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f92c9-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f92c9-134">False。</span><span class="sxs-lookup"><span data-stu-id="f92c9-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f92c9-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="f92c9-135">See also</span></span>

- [<span data-ttu-id="f92c9-136">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="f92c9-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

