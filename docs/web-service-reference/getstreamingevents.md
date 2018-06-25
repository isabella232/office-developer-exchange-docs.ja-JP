---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: GetStreamingEvents 要素は、サーバーからのストリーミングの通知を要求するクライアントによって使用される演算を表します。
ms.openlocfilehash: b07015541cf9c2fbbbc11ebc9f10421bdb9ee84f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831679"
---
# <a name="getstreamingevents"></a><span data-ttu-id="0ba98-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="0ba98-103">GetStreamingEvents</span></span>

<span data-ttu-id="0ba98-104">**GetStreamingEvents**要素は、サーバーからのストリーミングの通知を要求するクライアントによって使用される演算を表します。</span><span class="sxs-lookup"><span data-stu-id="0ba98-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="0ba98-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="0ba98-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="0ba98-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="0ba98-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ba98-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0ba98-107">Attributes and elements</span></span>

<span data-ttu-id="0ba98-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0ba98-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ba98-109">属性</span><span class="sxs-lookup"><span data-stu-id="0ba98-109">Attributes</span></span>

<span data-ttu-id="0ba98-110">なし。</span><span class="sxs-lookup"><span data-stu-id="0ba98-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ba98-111">子要素</span><span class="sxs-lookup"><span data-stu-id="0ba98-111">Child elements</span></span>

|<span data-ttu-id="0ba98-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ba98-112">**Element**</span></span>|<span data-ttu-id="0ba98-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ba98-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ba98-114">サブスクリプション Id (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="0ba98-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="0ba98-115">イベントを照会するサブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="0ba98-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="0ba98-116">タイムアウト</span><span class="sxs-lookup"><span data-stu-id="0ba98-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="0ba98-117">接続を開いたままにしておく秒数を表します。</span><span class="sxs-lookup"><span data-stu-id="0ba98-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ba98-118">親要素</span><span class="sxs-lookup"><span data-stu-id="0ba98-118">Parent elements</span></span>

<span data-ttu-id="0ba98-119">なし。</span><span class="sxs-lookup"><span data-stu-id="0ba98-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0ba98-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0ba98-120">Text value</span></span>

<span data-ttu-id="0ba98-121">なし。</span><span class="sxs-lookup"><span data-stu-id="0ba98-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ba98-122">備考</span><span class="sxs-lookup"><span data-stu-id="0ba98-122">Remarks</span></span>

<span data-ttu-id="0ba98-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0ba98-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ba98-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="0ba98-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ba98-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="0ba98-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ba98-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0ba98-126">Schema name</span></span>  <br/> |<span data-ttu-id="0ba98-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0ba98-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ba98-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0ba98-128">Validation file</span></span>  <br/> |<span data-ttu-id="0ba98-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ba98-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ba98-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0ba98-130">Can be empty</span></span>  <br/> |<span data-ttu-id="0ba98-131">False</span><span class="sxs-lookup"><span data-stu-id="0ba98-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ba98-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ba98-132">See also</span></span>



[<span data-ttu-id="0ba98-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="0ba98-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0ba98-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="0ba98-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="0ba98-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="0ba98-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="0ba98-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0ba98-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

