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
description: GetCallInfoResponse 要素は、GetCallInfo 操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461206"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="04d69-103">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="04d69-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="04d69-104">**GetCallInfoResponse**要素は、 [Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="04d69-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="04d69-105">GetCallInfoResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="04d69-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="04d69-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="04d69-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04d69-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="04d69-107">Attributes and elements</span></span>

<span data-ttu-id="04d69-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04d69-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04d69-109">属性</span><span class="sxs-lookup"><span data-stu-id="04d69-109">Attributes</span></span>

<span data-ttu-id="04d69-110">なし。</span><span class="sxs-lookup"><span data-stu-id="04d69-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04d69-111">子要素</span><span class="sxs-lookup"><span data-stu-id="04d69-111">Child elements</span></span>

|<span data-ttu-id="04d69-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="04d69-112">**Element**</span></span>|<span data-ttu-id="04d69-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="04d69-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04d69-114">CallState</span><span class="sxs-lookup"><span data-stu-id="04d69-114">CallState</span></span>  <br/> |<span data-ttu-id="04d69-115">[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した通話の状態を示す値を格納します。</span><span class="sxs-lookup"><span data-stu-id="04d69-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="04d69-116">イベント原因</span><span class="sxs-lookup"><span data-stu-id="04d69-116">EventCause</span></span>  <br/> |<span data-ttu-id="04d69-117">[Getcallinfo 操作 (UM web サービス)](getcallinfo-operation-um-web-service.md)が情報を要求した呼び出しに対するイベントの原因を示す値を格納します。</span><span class="sxs-lookup"><span data-stu-id="04d69-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04d69-118">親要素</span><span class="sxs-lookup"><span data-stu-id="04d69-118">Parent elements</span></span>

<span data-ttu-id="04d69-119">なし。</span><span class="sxs-lookup"><span data-stu-id="04d69-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="04d69-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04d69-120">Text value</span></span>

<span data-ttu-id="04d69-121">なし。</span><span class="sxs-lookup"><span data-stu-id="04d69-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04d69-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="04d69-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04d69-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="04d69-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04d69-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04d69-124">Schema Name</span></span>  <br/> |<span data-ttu-id="04d69-125">メッセージ</span><span class="sxs-lookup"><span data-stu-id="04d69-125">Messages</span></span>  <br/> |
|<span data-ttu-id="04d69-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04d69-126">Validation File</span></span>  <br/> |<span data-ttu-id="04d69-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="04d69-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04d69-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04d69-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="04d69-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="04d69-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04d69-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="04d69-130">See also</span></span>



[<span data-ttu-id="04d69-131">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="04d69-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="04d69-132">CallState (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="04d69-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="04d69-133">EventCause (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="04d69-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

