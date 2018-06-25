---
title: messageSnapshot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- messageSnapshot
api_type:
- schema
ms.assetid: f157e44c-b950-463f-b086-31d5da94b7ff
description: '最終更新日: 2015 年 9 月 17 日'
ms.openlocfilehash: 4b814def8eef8fb452d2e754c5f6787d644055f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759256"
---
# <a name="messagesnapshot"></a><span data-ttu-id="464e2-103">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="464e2-103">messageSnapshot</span></span>

<span data-ttu-id="464e2-104">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="464e2-104">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="464e2-105">**MessageSnapshot**要素には、クライアント アクセスまたはメールボックス サーバーの役割がインストールされている Exchange サーバーのパイプライン トレース機能が有効になっているかどうかを指定する属性が含まれています。</span><span class="sxs-lookup"><span data-stu-id="464e2-105">The **messageSnapshot** element contains an attribute that specifies whether the pipeline tracing feature is enabled for the Exchange server that has the Client Access or the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="464e2-106">構成</span><span class="sxs-lookup"><span data-stu-id="464e2-106">configuration</span></span>](configuration.md)  
- [<span data-ttu-id="464e2-107">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="464e2-107">mexRuntime</span></span>](mexruntime.md) 
- [<span data-ttu-id="464e2-108">監視</span><span class="sxs-lookup"><span data-stu-id="464e2-108">monitoring</span></span>](monitoring.md) 
- [<span data-ttu-id="464e2-109">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="464e2-109">messageSnapshot</span></span>](messagesnapshot.md)
  
```XML
<messageSnapshot enabled="" />
```

<span data-ttu-id="464e2-110">**messageSnapshotType (ブール値)**</span><span class="sxs-lookup"><span data-stu-id="464e2-110">**messageSnapshotType (Boolean)**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="464e2-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="464e2-111">Attributes and elements</span></span>

<span data-ttu-id="464e2-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="464e2-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="464e2-113">属性</span><span class="sxs-lookup"><span data-stu-id="464e2-113">Attributes</span></span>

|<span data-ttu-id="464e2-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="464e2-114">**Attribute**</span></span>|<span data-ttu-id="464e2-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="464e2-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="464e2-116">**有効になっています。**</span><span class="sxs-lookup"><span data-stu-id="464e2-116">**enabled**</span></span> <br/> |<span data-ttu-id="464e2-117">クライアント アクセスまたはメールボックス サーバーのパイプライン トレース機能が有効になっているかどうかを示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="464e2-117">A Boolean value that indicates whether the pipeline tracing feature is enabled for the Client Access or the Mailbox server.</span></span> <span data-ttu-id="464e2-118">値が**true**の場合、パイプライン トレースが有効になっています。それ以外の場合、値は**false**または、要素が存在しません。</span><span class="sxs-lookup"><span data-stu-id="464e2-118">The value is **true** if pipeline tracing is enabled; otherwise, the value is **false** or the element is not present.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="464e2-119">子要素</span><span class="sxs-lookup"><span data-stu-id="464e2-119">Child elements</span></span>

<span data-ttu-id="464e2-120">なし。</span><span class="sxs-lookup"><span data-stu-id="464e2-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="464e2-121">親要素</span><span class="sxs-lookup"><span data-stu-id="464e2-121">Parent elements</span></span>

|<span data-ttu-id="464e2-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="464e2-122">**Element**</span></span>|<span data-ttu-id="464e2-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="464e2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="464e2-124">監視</span><span class="sxs-lookup"><span data-stu-id="464e2-124">monitoring</span></span>](monitoring.md) <br/> |<span data-ttu-id="464e2-125">トランスポート サービスがインストールされているエージェントを監視する方法とタイミングを定義する構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="464e2-125">Contains configuration information that defines how and when the transport service monitors agents that are installed.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="464e2-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="464e2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="464e2-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="464e2-127">Namespace</span></span>  <br/> |<span data-ttu-id="464e2-128">このファイルには名前空間が定義されていません。</span><span class="sxs-lookup"><span data-stu-id="464e2-128">This file does not define a namespace.</span></span>  <br/> |
|<span data-ttu-id="464e2-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="464e2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="464e2-130">該当なし。</span><span class="sxs-lookup"><span data-stu-id="464e2-130">Not available.</span></span>  <br/> |
|<span data-ttu-id="464e2-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="464e2-131">Validation File</span></span>  <br/> |<span data-ttu-id="464e2-132">該当なし。</span><span class="sxs-lookup"><span data-stu-id="464e2-132">Not available.</span></span>  <br/> |
|<span data-ttu-id="464e2-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="464e2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="464e2-134">False。</span><span class="sxs-lookup"><span data-stu-id="464e2-134">False.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="464e2-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="464e2-135">See also</span></span>

- [<span data-ttu-id="464e2-136">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="464e2-136">Agents configuration file elements for Exchange 2013</span></span>](agents-configuration-file-elements-for-exchange-2013.md)

