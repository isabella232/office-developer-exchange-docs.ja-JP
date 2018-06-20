---
title: CallState (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: CallState 要素には、呼び出しのステータスを示す値が含まれています。
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759605"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="fced1-103">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-103">CallState (UM web service)</span></span>

<span data-ttu-id="fced1-104">**CallState**要素には、呼び出しのステータスを示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fced1-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="fced1-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="fced1-106">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="fced1-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="fced1-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fced1-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fced1-108">Attributes and elements</span></span>

<span data-ttu-id="fced1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fced1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fced1-110">属性</span><span class="sxs-lookup"><span data-stu-id="fced1-110">Attributes</span></span>

<span data-ttu-id="fced1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fced1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fced1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fced1-112">Child elements</span></span>

<span data-ttu-id="fced1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fced1-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fced1-114">親要素</span><span class="sxs-lookup"><span data-stu-id="fced1-114">Parent elements</span></span>

|<span data-ttu-id="fced1-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="fced1-115">**Element**</span></span>|<span data-ttu-id="fced1-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="fced1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fced1-117">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="fced1-118">[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="fced1-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fced1-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fced1-119">Text value</span></span>

<span data-ttu-id="fced1-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="fced1-120">A text value is required.</span></span> <span data-ttu-id="fced1-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="fced1-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="fced1-122">アイドル</span><span class="sxs-lookup"><span data-stu-id="fced1-122">Idle</span></span>
    
- <span data-ttu-id="fced1-123">Connecting</span><span class="sxs-lookup"><span data-stu-id="fced1-123">Connecting</span></span>
    
- <span data-ttu-id="fced1-124">警告を表示</span><span class="sxs-lookup"><span data-stu-id="fced1-124">Alerted</span></span>
    
- <span data-ttu-id="fced1-125">Connected</span><span class="sxs-lookup"><span data-stu-id="fced1-125">Connected</span></span>
    
- <span data-ttu-id="fced1-126">Disconnected</span><span class="sxs-lookup"><span data-stu-id="fced1-126">Disconnected</span></span>
    
- <span data-ttu-id="fced1-127">受信</span><span class="sxs-lookup"><span data-stu-id="fced1-127">Incoming</span></span>
    
- <span data-ttu-id="fced1-128">転送します。</span><span class="sxs-lookup"><span data-stu-id="fced1-128">Transferring</span></span>
    
- <span data-ttu-id="fced1-129">転送</span><span class="sxs-lookup"><span data-stu-id="fced1-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="fced1-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="fced1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fced1-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="fced1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="fced1-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fced1-132">Schema Name</span></span>  <br/> |<span data-ttu-id="fced1-133">メッセージ</span><span class="sxs-lookup"><span data-stu-id="fced1-133">Messages</span></span>  <br/> |
|<span data-ttu-id="fced1-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fced1-134">Validation File</span></span>  <br/> |<span data-ttu-id="fced1-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fced1-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fced1-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fced1-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="fced1-137">False</span><span class="sxs-lookup"><span data-stu-id="fced1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fced1-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="fced1-138">See also</span></span>



[<span data-ttu-id="fced1-139">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="fced1-140">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="fced1-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

