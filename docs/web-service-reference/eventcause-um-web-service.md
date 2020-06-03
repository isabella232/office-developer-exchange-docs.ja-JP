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
description: EventCause 要素には、GetCallInfo 操作 (UM web サービス) 要求に対する応答の呼び出しイベントの原因を示す値が含まれています。
ms.openlocfilehash: 9d49fd4b16236d0dd87889fbbd039f2e271a5968
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458678"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="0a9ad-103">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-103">EventCause (UM web service)</span></span>

<span data-ttu-id="0a9ad-104">**Eventcause**要素には、 [Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答の呼び出しイベントの原因を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="0a9ad-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="0a9ad-106">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="0a9ad-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="0a9ad-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a9ad-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0a9ad-108">Attributes and elements</span></span>

<span data-ttu-id="0a9ad-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a9ad-110">属性</span><span class="sxs-lookup"><span data-stu-id="0a9ad-110">Attributes</span></span>

<span data-ttu-id="0a9ad-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a9ad-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0a9ad-112">Child elements</span></span>

<span data-ttu-id="0a9ad-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a9ad-114">親要素</span><span class="sxs-lookup"><span data-stu-id="0a9ad-114">Parent elements</span></span>

|<span data-ttu-id="0a9ad-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="0a9ad-115">**Element**</span></span>|<span data-ttu-id="0a9ad-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="0a9ad-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a9ad-117">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="0a9ad-118">[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a9ad-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0a9ad-119">Text value</span></span>

<span data-ttu-id="0a9ad-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-120">A text value is required.</span></span> <span data-ttu-id="0a9ad-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="0a9ad-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="0a9ad-122">なし</span><span class="sxs-lookup"><span data-stu-id="0a9ad-122">None</span></span>
    
- <span data-ttu-id="0a9ad-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="0a9ad-123">UserBusy</span></span>
    
- <span data-ttu-id="0a9ad-124">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="0a9ad-124">NoAnswer</span></span>
    
- <span data-ttu-id="0a9ad-125">その他</span><span class="sxs-lookup"><span data-stu-id="0a9ad-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="0a9ad-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0a9ad-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a9ad-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a9ad-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0a9ad-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0a9ad-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0a9ad-129">メッセージ</span><span class="sxs-lookup"><span data-stu-id="0a9ad-129">Messages</span></span>  <br/> |
|<span data-ttu-id="0a9ad-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0a9ad-130">Validation File</span></span>  <br/> |<span data-ttu-id="0a9ad-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0a9ad-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0a9ad-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0a9ad-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a9ad-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="0a9ad-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a9ad-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="0a9ad-134">See also</span></span>



[<span data-ttu-id="0a9ad-135">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="0a9ad-136">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="0a9ad-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

