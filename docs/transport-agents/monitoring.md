---
title: 管理
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- monitoring
api_type:
- schema
ms.assetid: 350d7b46-9260-41a7-8613-3cb8cc1b29a5
description: '最終更新日: 2015 年9月17日'
ms.openlocfilehash: 5614ac2c6428da9b6845769a9335486d3ded5754
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455829"
---
# <a name="monitoring"></a><span data-ttu-id="7eb10-103">管理</span><span class="sxs-lookup"><span data-stu-id="7eb10-103">monitoring</span></span>
  
<span data-ttu-id="7eb10-104">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="7eb10-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="7eb10-105">**monitoring** 要素には、インストールされているエージェントをフロント エンド トランスポート サービスまたはトランスポート サービスが監視する方法とタイミングを定義する構成情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="7eb10-105">The **monitoring** element contains configuration information that defines how and when the Front End transport service or the Transport service monitors agents that are installed.</span></span> 
  
- [<span data-ttu-id="7eb10-106">構成</span><span class="sxs-lookup"><span data-stu-id="7eb10-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="7eb10-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="7eb10-107">mexRuntime</span></span>](mexruntime.md)  
- [<span data-ttu-id="7eb10-108">管理</span><span class="sxs-lookup"><span data-stu-id="7eb10-108">monitoring</span></span>](monitoring.md)
  
```XML
<monitoring>
   <agentExecution/>
   <messageSnapshot/>
</monitoring>
```

<span data-ttu-id="7eb10-109">**monitoringType (complexType)**</span><span class="sxs-lookup"><span data-stu-id="7eb10-109">**monitoringType (complexType)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7eb10-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7eb10-110">Attributes and elements</span></span>

<span data-ttu-id="7eb10-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7eb10-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7eb10-112">属性</span><span class="sxs-lookup"><span data-stu-id="7eb10-112">Attributes</span></span>

<span data-ttu-id="7eb10-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7eb10-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7eb10-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7eb10-114">Child elements</span></span>

|<span data-ttu-id="7eb10-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="7eb10-115">**Element**</span></span>|<span data-ttu-id="7eb10-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb10-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb10-117">agentExecution</span><span class="sxs-lookup"><span data-stu-id="7eb10-117">agentExecution</span></span>](agentexecution.md) <br/> |<span data-ttu-id="7eb10-118">クライアント アクセス サーバーまたはメールボックス サーバーがエージェントのイベントからの復帰を待機する時間をミリ秒単位で定義します。この時間を過ぎるとイベント ログへの書き込みが行われます。</span><span class="sxs-lookup"><span data-stu-id="7eb10-118">Defines the time, in milliseconds, for the Client Access or the Mailbox server to wait for an agent to return from an event before it writes to the event log.</span></span>  <br/> |
|[<span data-ttu-id="7eb10-119">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="7eb10-119">messageSnapshot</span></span>](messagesnapshot.md) <br/> |<span data-ttu-id="7eb10-120">クライアントアクセスまたはメールボックスサーバーでパイプライントレース機能が有効になっているかどうかを指定する属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7eb10-120">Contains an attribute that specifies whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7eb10-121">親要素</span><span class="sxs-lookup"><span data-stu-id="7eb10-121">Parent elements</span></span>

|<span data-ttu-id="7eb10-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="7eb10-122">**Element**</span></span>|<span data-ttu-id="7eb10-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="7eb10-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7eb10-124">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="7eb10-124">mexRuntime</span></span>](mexruntime.md) <br/> |<span data-ttu-id="7eb10-125">エージェントの監視に関する構成情報を定義する要素と、インストールされているエージェントの SMTP およびルーティングに関する構成情報を定義する要素を格納します。</span><span class="sxs-lookup"><span data-stu-id="7eb10-125">Contains elements that define configuration information for agent monitoring and configuration information for SMTP and routing agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="7eb10-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7eb10-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7eb10-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="7eb10-127">Namespace</span></span>  <br/> |<span data-ttu-id="7eb10-128">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="7eb10-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="7eb10-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7eb10-129">Schema Name</span></span>  <br/> |<span data-ttu-id="7eb10-130">注意事項なし。</span><span class="sxs-lookup"><span data-stu-id="7eb10-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="7eb10-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7eb10-131">Validation File</span></span>  <br/> |<span data-ttu-id="7eb10-132">該当なし。</span><span class="sxs-lookup"><span data-stu-id="7eb10-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="7eb10-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7eb10-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="7eb10-134">不正解。</span><span class="sxs-lookup"><span data-stu-id="7eb10-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7eb10-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="7eb10-135">See also</span></span>

- [<span data-ttu-id="7eb10-136">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="7eb10-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

