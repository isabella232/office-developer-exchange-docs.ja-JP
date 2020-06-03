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
description: GetStreamingEvents 要素は、サーバーからのストリーミング通知を要求するためにクライアントによって使用される操作を表します。
ms.openlocfilehash: ec133ecd69c05a2208e95f925133570af0233cf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457320"
---
# <a name="getstreamingevents"></a><span data-ttu-id="21f63-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="21f63-103">GetStreamingEvents</span></span>

<span data-ttu-id="21f63-104">**Getstreamingevents**要素は、サーバーからのストリーミング通知を要求するためにクライアントによって使用される操作を表します。</span><span class="sxs-lookup"><span data-stu-id="21f63-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="21f63-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="21f63-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="21f63-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="21f63-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21f63-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21f63-107">Attributes and elements</span></span>

<span data-ttu-id="21f63-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21f63-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21f63-109">属性</span><span class="sxs-lookup"><span data-stu-id="21f63-109">Attributes</span></span>

<span data-ttu-id="21f63-110">なし。</span><span class="sxs-lookup"><span data-stu-id="21f63-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21f63-111">子要素</span><span class="sxs-lookup"><span data-stu-id="21f63-111">Child elements</span></span>

|<span data-ttu-id="21f63-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="21f63-112">**Element**</span></span>|<span data-ttu-id="21f63-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="21f63-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21f63-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="21f63-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="21f63-115">イベントを照会するサブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="21f63-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="21f63-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="21f63-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="21f63-117">接続を開いたままにする時間を分単位で表します。</span><span class="sxs-lookup"><span data-stu-id="21f63-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21f63-118">親要素</span><span class="sxs-lookup"><span data-stu-id="21f63-118">Parent elements</span></span>

<span data-ttu-id="21f63-119">なし。</span><span class="sxs-lookup"><span data-stu-id="21f63-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="21f63-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21f63-120">Text value</span></span>

<span data-ttu-id="21f63-121">なし。</span><span class="sxs-lookup"><span data-stu-id="21f63-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21f63-122">注釈</span><span class="sxs-lookup"><span data-stu-id="21f63-122">Remarks</span></span>

<span data-ttu-id="21f63-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="21f63-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21f63-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21f63-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21f63-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="21f63-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21f63-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21f63-126">Schema name</span></span>  <br/> |<span data-ttu-id="21f63-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="21f63-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21f63-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21f63-128">Validation file</span></span>  <br/> |<span data-ttu-id="21f63-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="21f63-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21f63-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="21f63-130">Can be empty</span></span>  <br/> |<span data-ttu-id="21f63-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="21f63-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21f63-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="21f63-132">See also</span></span>



[<span data-ttu-id="21f63-133">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="21f63-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="21f63-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="21f63-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="21f63-135">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="21f63-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="21f63-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="21f63-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

