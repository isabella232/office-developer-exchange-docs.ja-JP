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
description: CallId 要素には、GetCallInfo (UM web サービス) の要求または切断 (UM web サービス) 要求の呼び出しの id を表す値が含まれています。
ms.openlocfilehash: 49690f41b9a002b05c7c9b1a1240073c7230ab92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759604"
---
# <a name="callid-um-web-service"></a><span data-ttu-id="9268e-103">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-103">CallId (UM web service)</span></span>

<span data-ttu-id="9268e-104">**CallId**要素には、 [GetCallInfo (UM web サービス)](getcallinfo-um-web-service.md)の要求または[切断 (UM web サービス)](disconnect-um-web-service.md)要求の呼び出しの id を表す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9268e-104">The **CallId** element contains the value that represents the identifier of the call in a [GetCallInfo (UM web service)](getcallinfo-um-web-service.md) request or [Disconnect (UM web service)](disconnect-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="9268e-105">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-105">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="9268e-106">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-106">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="9268e-107">(UM web サービス) に接続を切断します。</span><span class="sxs-lookup"><span data-stu-id="9268e-107">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md)
  
[<span data-ttu-id="9268e-108">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-108">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
```xml
<CallId/>
```

 <span data-ttu-id="9268e-109">**string**</span><span class="sxs-lookup"><span data-stu-id="9268e-109">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9268e-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9268e-110">Attributes and elements</span></span>

<span data-ttu-id="9268e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9268e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9268e-112">属性</span><span class="sxs-lookup"><span data-stu-id="9268e-112">Attributes</span></span>

<span data-ttu-id="9268e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9268e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9268e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9268e-114">Child elements</span></span>

<span data-ttu-id="9268e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="9268e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9268e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="9268e-116">Parent elements</span></span>

|<span data-ttu-id="9268e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="9268e-117">**Element**</span></span>|<span data-ttu-id="9268e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="9268e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9268e-119">GetCallInfo (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-119">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md) <br/> |<span data-ttu-id="9268e-120">呼び出しに関する情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9268e-120">Defines a request to get information about a call.</span></span>  <br/> |
|[<span data-ttu-id="9268e-121">(UM web サービス) に接続を切断します。</span><span class="sxs-lookup"><span data-stu-id="9268e-121">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) <br/> |<span data-ttu-id="9268e-122">呼び出しの切断要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9268e-122">Defines a request to disconnect a call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9268e-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9268e-123">Text value</span></span>

<span data-ttu-id="9268e-124">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="9268e-124">A text value is required.</span></span> <span data-ttu-id="9268e-125">テキスト値は、呼び出しの id を表します。</span><span class="sxs-lookup"><span data-stu-id="9268e-125">The text value represents the identifier for a call.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9268e-126">備考</span><span class="sxs-lookup"><span data-stu-id="9268e-126">Remarks</span></span>

<span data-ttu-id="9268e-127">最初の呼び出しを[PlayOnPhone 操作 (UM web サービス)](playonphone-operation-um-web-service.md)または[PlayOnPhoneGreeting 操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="9268e-127">To initial a call, use the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) or [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span> <span data-ttu-id="9268e-128">**CallId**要素のテキスト値の[PlayOnPhoneResponse (UM web サービス)](playonphoneresponse-um-web-service.md)または[PlayOnPhoneGreetingResponse (UM web サービス)](playonphonegreetingresponse-um-web-service.md)の要素で返される文字列値を使用します。</span><span class="sxs-lookup"><span data-stu-id="9268e-128">Use the text value that is returned in the [PlayOnPhoneResponse (UM web service)](playonphoneresponse-um-web-service.md) or [PlayOnPhoneGreetingResponse (UM web service)](playonphonegreetingresponse-um-web-service.md) elements for the **CallId** element text value.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9268e-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="9268e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9268e-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="9268e-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9268e-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9268e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9268e-132">メッセージ</span><span class="sxs-lookup"><span data-stu-id="9268e-132">Messages</span></span>  <br/> |
|<span data-ttu-id="9268e-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9268e-133">Validation File</span></span>  <br/> |<span data-ttu-id="9268e-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9268e-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9268e-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9268e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9268e-136">False</span><span class="sxs-lookup"><span data-stu-id="9268e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9268e-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="9268e-137">See also</span></span>



[<span data-ttu-id="9268e-138">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-138">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="9268e-139">操作 (UM web サービス) に接続を切断します。</span><span class="sxs-lookup"><span data-stu-id="9268e-139">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)
  
[<span data-ttu-id="9268e-140">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-140">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)
  
[<span data-ttu-id="9268e-141">PlayOnPhoneGreeting 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9268e-141">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

