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
description: CallState 要素には、呼び出しの状態を示す値が含まれています。
ms.openlocfilehash: 44614c460286ff49ebc2373263c1827c6be5cc08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454611"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="ef268-103">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-103">CallState (UM web service)</span></span>

<span data-ttu-id="ef268-104">**Callstate**要素には、呼び出しの状態を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ef268-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="ef268-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="ef268-106">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="ef268-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="ef268-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef268-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ef268-108">Attributes and elements</span></span>

<span data-ttu-id="ef268-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ef268-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef268-110">属性</span><span class="sxs-lookup"><span data-stu-id="ef268-110">Attributes</span></span>

<span data-ttu-id="ef268-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ef268-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef268-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ef268-112">Child elements</span></span>

<span data-ttu-id="ef268-113">なし。</span><span class="sxs-lookup"><span data-stu-id="ef268-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef268-114">親要素</span><span class="sxs-lookup"><span data-stu-id="ef268-114">Parent elements</span></span>

|<span data-ttu-id="ef268-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="ef268-115">**Element**</span></span>|<span data-ttu-id="ef268-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="ef268-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef268-117">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="ef268-118">Getcallinfo 操作への応答を定義します[(UM web サービス)](getcallinfo-operation-um-web-service.md)。</span><span class="sxs-lookup"><span data-stu-id="ef268-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef268-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ef268-119">Text value</span></span>

<span data-ttu-id="ef268-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="ef268-120">A text value is required.</span></span> <span data-ttu-id="ef268-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="ef268-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="ef268-122">アイドル</span><span class="sxs-lookup"><span data-stu-id="ef268-122">Idle</span></span>
    
- <span data-ttu-id="ef268-123">接続中</span><span class="sxs-lookup"><span data-stu-id="ef268-123">Connecting</span></span>
    
- <span data-ttu-id="ef268-124">警告</span><span class="sxs-lookup"><span data-stu-id="ef268-124">Alerted</span></span>
    
- <span data-ttu-id="ef268-125">Connected</span><span class="sxs-lookup"><span data-stu-id="ef268-125">Connected</span></span>
    
- <span data-ttu-id="ef268-126">Disconnected</span><span class="sxs-lookup"><span data-stu-id="ef268-126">Disconnected</span></span>
    
- <span data-ttu-id="ef268-127">読み込ま</span><span class="sxs-lookup"><span data-stu-id="ef268-127">Incoming</span></span>
    
- <span data-ttu-id="ef268-128">渡す</span><span class="sxs-lookup"><span data-stu-id="ef268-128">Transferring</span></span>
    
- <span data-ttu-id="ef268-129">しよう</span><span class="sxs-lookup"><span data-stu-id="ef268-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="ef268-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ef268-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef268-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef268-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="ef268-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ef268-132">Schema Name</span></span>  <br/> |<span data-ttu-id="ef268-133">メッセージ</span><span class="sxs-lookup"><span data-stu-id="ef268-133">Messages</span></span>  <br/> |
|<span data-ttu-id="ef268-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ef268-134">Validation File</span></span>  <br/> |<span data-ttu-id="ef268-135">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ef268-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef268-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ef268-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef268-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="ef268-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef268-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="ef268-138">See also</span></span>



[<span data-ttu-id="ef268-139">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="ef268-140">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="ef268-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

