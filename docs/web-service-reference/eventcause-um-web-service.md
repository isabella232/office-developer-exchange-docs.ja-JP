---
title: EventCause (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: EventCause 要素には、GetCallInfo 操作 (UM web サービス) 要求に対する応答で呼び出しイベントの原因を示す値が含まれています。
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760335"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="4a37d-103">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-103">EventCause (UM web service)</span></span>

<span data-ttu-id="4a37d-104">**EventCause**要素には、 [GetCallInfo 操作 (UM web サービス](getcallinfo-operation-um-web-service.md)要求への応答で呼び出しイベントの原因を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a37d-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="4a37d-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="4a37d-106">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="4a37d-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="4a37d-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a37d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4a37d-108">Attributes and elements</span></span>

<span data-ttu-id="4a37d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a37d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a37d-110">属性</span><span class="sxs-lookup"><span data-stu-id="4a37d-110">Attributes</span></span>

<span data-ttu-id="4a37d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4a37d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a37d-112">子要素</span><span class="sxs-lookup"><span data-stu-id="4a37d-112">Child elements</span></span>

<span data-ttu-id="4a37d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="4a37d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a37d-114">親要素</span><span class="sxs-lookup"><span data-stu-id="4a37d-114">Parent elements</span></span>

|<span data-ttu-id="4a37d-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a37d-115">**Element**</span></span>|<span data-ttu-id="4a37d-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a37d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a37d-117">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="4a37d-118">[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4a37d-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a37d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a37d-119">Text value</span></span>

<span data-ttu-id="4a37d-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="4a37d-120">A text value is required.</span></span> <span data-ttu-id="4a37d-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="4a37d-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="4a37d-122">なし</span><span class="sxs-lookup"><span data-stu-id="4a37d-122">None</span></span>
    
- <span data-ttu-id="4a37d-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="4a37d-123">UserBusy</span></span>
    
- <span data-ttu-id="4a37d-124">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="4a37d-124">NoAnswer</span></span>
    
- <span data-ttu-id="4a37d-125">その他</span><span class="sxs-lookup"><span data-stu-id="4a37d-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="4a37d-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="4a37d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a37d-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="4a37d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a37d-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a37d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4a37d-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="4a37d-129">Messages</span></span>  <br/> |
|<span data-ttu-id="4a37d-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a37d-130">Validation File</span></span>  <br/> |<span data-ttu-id="4a37d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4a37d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a37d-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4a37d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a37d-133">False</span><span class="sxs-lookup"><span data-stu-id="4a37d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a37d-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a37d-134">See also</span></span>



[<span data-ttu-id="4a37d-135">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="4a37d-136">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="4a37d-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

