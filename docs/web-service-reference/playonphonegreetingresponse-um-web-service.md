---
title: PlayOnPhoneGreetingResponse (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreetingResponse
api_type:
- schema
ms.assetid: 7189d69a-9288-4fc8-8d78-4977ee1a7253
description: PlayOnPhoneGreetingResponse 要素は、Playon電話案内応答操作 (UM web サービス) 要求への応答を定義します。
ms.openlocfilehash: ca448860ef0e59607f73421c71d9c8f75c740773
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528854"
---
# <a name="playonphonegreetingresponse-um-web-service"></a><span data-ttu-id="b400e-103">PlayOnPhoneGreetingResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-103">PlayOnPhoneGreetingResponse (UM web service)</span></span>

<span data-ttu-id="b400e-104">**PlayOnPhoneGreetingResponse**要素は、 [Playon電話案内応答操作 (UM web サービス)](playonphonegreeting-operation-um-web-service.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b400e-104">The **PlayOnPhoneGreetingResponse** element defines a response to a [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="b400e-105">PlayOnPhoneGreetingResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-105">PlayOnPhoneGreetingResponse (UM web service)</span></span>](playonphonegreetingresponse-um-web-service.md)
  
```xml
<PlayOnPhoneGreetingResponse />
```

 <span data-ttu-id="b400e-106">**string**</span><span class="sxs-lookup"><span data-stu-id="b400e-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b400e-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b400e-107">Attributes and elements</span></span>

<span data-ttu-id="b400e-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b400e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b400e-109">属性</span><span class="sxs-lookup"><span data-stu-id="b400e-109">Attributes</span></span>

<span data-ttu-id="b400e-110">なし。</span><span class="sxs-lookup"><span data-stu-id="b400e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b400e-111">子要素</span><span class="sxs-lookup"><span data-stu-id="b400e-111">Child elements</span></span>

<span data-ttu-id="b400e-112">なし。</span><span class="sxs-lookup"><span data-stu-id="b400e-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b400e-113">親要素</span><span class="sxs-lookup"><span data-stu-id="b400e-113">Parent elements</span></span>

<span data-ttu-id="b400e-114">なし。</span><span class="sxs-lookup"><span data-stu-id="b400e-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b400e-115">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b400e-115">Text value</span></span>

<span data-ttu-id="b400e-116">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="b400e-116">A text value is required.</span></span> <span data-ttu-id="b400e-117">テキスト値には、 [Getcallinfo 操作 (um web](getcallinfo-operation-um-web-service.md)サービス) 要求または[切断操作 (um web サービス)](disconnect-operation-um-web-service.md)要求の[callid (um web サービス)](callid-um-web-service.md)の値として使用する値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b400e-117">The text value contains the value to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b400e-118">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b400e-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b400e-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="b400e-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b400e-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b400e-120">Schema Name</span></span>  <br/> |<span data-ttu-id="b400e-121">メッセージ</span><span class="sxs-lookup"><span data-stu-id="b400e-121">Messages</span></span>  <br/> |
|<span data-ttu-id="b400e-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b400e-122">Validation File</span></span>  <br/> |<span data-ttu-id="b400e-123">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b400e-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b400e-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b400e-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="b400e-125">正しくない</span><span class="sxs-lookup"><span data-stu-id="b400e-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b400e-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="b400e-126">See also</span></span>



[<span data-ttu-id="b400e-127">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-127">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)
  
[<span data-ttu-id="b400e-128">CallId (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-128">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="b400e-129">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-129">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="b400e-130">Disconnect 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="b400e-130">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)

