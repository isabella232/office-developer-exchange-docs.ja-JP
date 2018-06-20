---
title: GetCallInfoResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: GetCallInfoResponse 要素は、GetCallInfo の操作 (UM web サービス) 要求に対する応答を定義します。
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760653"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="9434f-103">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9434f-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="9434f-104">**GetCallInfoResponse**要素は、 [GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9434f-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="9434f-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9434f-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="9434f-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="9434f-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9434f-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9434f-107">Attributes and elements</span></span>

<span data-ttu-id="9434f-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9434f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9434f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9434f-109">Attributes</span></span>

<span data-ttu-id="9434f-110">なし。</span><span class="sxs-lookup"><span data-stu-id="9434f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9434f-111">子要素</span><span class="sxs-lookup"><span data-stu-id="9434f-111">Child elements</span></span>

|<span data-ttu-id="9434f-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="9434f-112">**Element**</span></span>|<span data-ttu-id="9434f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="9434f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9434f-114">CallState</span><span class="sxs-lookup"><span data-stu-id="9434f-114">CallState</span></span>  <br/> |<span data-ttu-id="9434f-115">呼び出しのステータスを示す値が含まれています[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求します。</span><span class="sxs-lookup"><span data-stu-id="9434f-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="9434f-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="9434f-116">EventCause</span></span>  <br/> |<span data-ttu-id="9434f-117">呼び出しのイベントの原因を示す値が含まれています[GetCallInfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求します。</span><span class="sxs-lookup"><span data-stu-id="9434f-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9434f-118">親要素</span><span class="sxs-lookup"><span data-stu-id="9434f-118">Parent elements</span></span>

<span data-ttu-id="9434f-119">なし。</span><span class="sxs-lookup"><span data-stu-id="9434f-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9434f-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9434f-120">Text value</span></span>

<span data-ttu-id="9434f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="9434f-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9434f-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9434f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9434f-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9434f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9434f-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9434f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9434f-125">メッセージ</span><span class="sxs-lookup"><span data-stu-id="9434f-125">Messages</span></span>  <br/> |
|<span data-ttu-id="9434f-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9434f-126">Validation File</span></span>  <br/> |<span data-ttu-id="9434f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9434f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9434f-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9434f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9434f-129">False</span><span class="sxs-lookup"><span data-stu-id="9434f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9434f-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9434f-130">See also</span></span>



[<span data-ttu-id="9434f-131">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9434f-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="9434f-132">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9434f-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="9434f-133">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9434f-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

