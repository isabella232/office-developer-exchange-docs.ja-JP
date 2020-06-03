---
title: CallId (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallId
api_type:
- schema
ms.assetid: 2e044109-8bf3-488c-a654-459ac62fa1e7
description: CallId 要素には、GetCallInfo (UM web サービス) 要求または Disconnect (UM web サービス) 要求の呼び出しの識別子を表す値が含まれています。
ms.openlocfilehash: 5d5f596d4a98cbfb4b53be04278dae2305fc10c3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529456"
---
# <a name="callid-um-web-service"></a><span data-ttu-id="17156-103">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-103">CallId (UM web service)</span></span>

<span data-ttu-id="17156-104">**Callid**要素には、 [Getcallinfo (um web サービス)](getcallinfo-um-web-service.md)要求または[Disconnect (um web サービス)](disconnect-um-web-service.md)要求の呼び出しの識別子を表す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17156-104">The **CallId** element contains the value that represents the identifier of the call in a [GetCallInfo (UM web service)](getcallinfo-um-web-service.md) request or [Disconnect (UM web service)](disconnect-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="17156-105">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-105">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="17156-106">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-106">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="17156-107">Disconnect (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-107">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md)
  
[<span data-ttu-id="17156-108">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-108">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
```xml
<CallId/>
```

 <span data-ttu-id="17156-109">**string**</span><span class="sxs-lookup"><span data-stu-id="17156-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17156-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17156-110">Attributes and elements</span></span>

<span data-ttu-id="17156-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17156-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17156-112">属性</span><span class="sxs-lookup"><span data-stu-id="17156-112">Attributes</span></span>

<span data-ttu-id="17156-113">なし。</span><span class="sxs-lookup"><span data-stu-id="17156-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17156-114">子要素</span><span class="sxs-lookup"><span data-stu-id="17156-114">Child elements</span></span>

<span data-ttu-id="17156-115">なし。</span><span class="sxs-lookup"><span data-stu-id="17156-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17156-116">親要素</span><span class="sxs-lookup"><span data-stu-id="17156-116">Parent elements</span></span>

|<span data-ttu-id="17156-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="17156-117">**Element**</span></span>|<span data-ttu-id="17156-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="17156-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17156-119">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-119">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md) <br/> |<span data-ttu-id="17156-120">呼び出しに関する情報を取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="17156-120">Defines a request to get information about a call.</span></span>  <br/> |
|[<span data-ttu-id="17156-121">Disconnect (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-121">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) <br/> |<span data-ttu-id="17156-122">呼び出しを切断する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="17156-122">Defines a request to disconnect a call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17156-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="17156-123">Text value</span></span>

<span data-ttu-id="17156-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="17156-124">A text value is required.</span></span> <span data-ttu-id="17156-125">テキスト値は、呼び出しの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="17156-125">The text value represents the identifier for a call.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17156-126">注釈</span><span class="sxs-lookup"><span data-stu-id="17156-126">Remarks</span></span>

<span data-ttu-id="17156-127">最初の呼び出しを開始するには、 [Playonphone 操作 (um web サービス)](playonphone-operation-um-web-service.md)または[Playonphone 機の案内応答操作 (um web サービス)](playonphonegreeting-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="17156-127">To initial a call, use the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) or [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span> <span data-ttu-id="17156-128">[PlayOnPhoneResponse (um web サービス)](playonphoneresponse-um-web-service.md)要素または[PlayOnPhoneGreetingResponse (um web サービス)](playonphonegreetingresponse-um-web-service.md)要素で、 **callid**要素のテキスト値として返されるテキスト値を使用します。</span><span class="sxs-lookup"><span data-stu-id="17156-128">Use the text value that is returned in the [PlayOnPhoneResponse (UM web service)](playonphoneresponse-um-web-service.md) or [PlayOnPhoneGreetingResponse (UM web service)](playonphonegreetingresponse-um-web-service.md) elements for the **CallId** element text value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="17156-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="17156-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17156-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="17156-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="17156-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17156-131">Schema Name</span></span>  <br/> |<span data-ttu-id="17156-132">メッセージ</span><span class="sxs-lookup"><span data-stu-id="17156-132">Messages</span></span>  <br/> |
|<span data-ttu-id="17156-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17156-133">Validation File</span></span>  <br/> |<span data-ttu-id="17156-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="17156-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="17156-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="17156-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="17156-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="17156-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17156-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="17156-137">See also</span></span>



[<span data-ttu-id="17156-138">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-138">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="17156-139">Disconnect 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-139">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)
  
[<span data-ttu-id="17156-140">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-140">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)
  
[<span data-ttu-id="17156-141">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="17156-141">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

