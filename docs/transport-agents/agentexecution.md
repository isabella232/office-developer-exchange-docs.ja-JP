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
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: 457257e59fb37659daf2f91b0fa5dfced5c48c03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44446491"
---
# <a name="agentexecution"></a><span data-ttu-id="4297f-103">agentExecution</span><span class="sxs-lookup"><span data-stu-id="4297f-103">agentExecution</span></span>
  
<span data-ttu-id="4297f-104">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="4297f-104">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="4297f-105">**agentExecution** 要素では、クライアント アクセス サーバーまたはメールボックス サーバーがエージェントのイベントからの復帰を待機する時間をミリ秒単位で定義します。この時間を過ぎるとイベント ログへの書き込みが行われます。</span><span class="sxs-lookup"><span data-stu-id="4297f-105">The **agentExecution** element defines the time, in milliseconds, for the Client Access or Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span> 
  
- [<span data-ttu-id="4297f-106">構成</span><span class="sxs-lookup"><span data-stu-id="4297f-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="4297f-107">管理</span><span class="sxs-lookup"><span data-stu-id="4297f-107">monitoring</span></span>](monitoring.md)
- [<span data-ttu-id="4297f-108">agentExecution</span><span class="sxs-lookup"><span data-stu-id="4297f-108">agentExecution</span></span>](agentexecution.md)
  
```XML
<agentExecution timeLimitInMilliseconds="" />
```

<span data-ttu-id="4297f-109">**agentExecutionType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="4297f-109">**agentExecutionType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4297f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4297f-110">Attributes and elements</span></span>

<span data-ttu-id="4297f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4297f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4297f-112">属性</span><span class="sxs-lookup"><span data-stu-id="4297f-112">Attributes</span></span>

|<span data-ttu-id="4297f-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="4297f-113">**Attribute**</span></span>|<span data-ttu-id="4297f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4297f-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4297f-115">**timeLimitInMilliseconds**</span><span class="sxs-lookup"><span data-stu-id="4297f-115">**timeLimitInMilliseconds**</span></span> <br/> |<span data-ttu-id="4297f-p101">エージェントのイベントからの復帰をサーバーが待機する時間をミリ秒単位で指定する正の整数値。この時間を過ぎるとイベント ログに警告が書き込まれます。この値が小さすぎると、パフォーマンスが低下することがあります。この属性の推奨値は、5 分間に相当する 300,000 です。</span><span class="sxs-lookup"><span data-stu-id="4297f-p101">A positive integer value that specifies the time, in milliseconds, for the server to wait for an agent to return from an event before it writes a warning to the event log. Performance can decrease if this value is too small. The suggested value for this attribute is 300,000, which equates to 5 minutes.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4297f-119">子要素</span><span class="sxs-lookup"><span data-stu-id="4297f-119">Child elements</span></span>

<span data-ttu-id="4297f-120">なし。</span><span class="sxs-lookup"><span data-stu-id="4297f-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4297f-121">親要素</span><span class="sxs-lookup"><span data-stu-id="4297f-121">Parent elements</span></span>

|<span data-ttu-id="4297f-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="4297f-122">**Element**</span></span>|<span data-ttu-id="4297f-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="4297f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4297f-124">管理</span><span class="sxs-lookup"><span data-stu-id="4297f-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="4297f-125">インストールされているエージェントをフロント エンド トランスポート サービスまたはトランスポート サービスが監視する方法とタイミングを定義する構成情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="4297f-125">Contains configuration information that defines how and when the Front End Transport service or the Transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4297f-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4297f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4297f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="4297f-127">Namespace</span></span>  <br/> |<span data-ttu-id="4297f-128">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="4297f-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="4297f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4297f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="4297f-130">注意事項なし。</span><span class="sxs-lookup"><span data-stu-id="4297f-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="4297f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4297f-131">Validation File</span></span>  <br/> |<span data-ttu-id="4297f-132">該当なし。</span><span class="sxs-lookup"><span data-stu-id="4297f-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="4297f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4297f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="4297f-134">不正解。</span><span class="sxs-lookup"><span data-stu-id="4297f-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4297f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="4297f-135">See also</span></span>

- [<span data-ttu-id="4297f-136">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="4297f-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

