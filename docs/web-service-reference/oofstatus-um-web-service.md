---
title: OofStatus (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: OofStatus 要素には、その indicaties GetUMProperties 操作 (UM web サービス) 要求を行っているユーザーのメッセージングの Office を統合の状態の値が含まれています。
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832650"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="9d214-103">OofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="9d214-104">**OofStatus**要素には、その indicaties [GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求を行っているユーザーのメッセージングの Office を統合の状態の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d214-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="9d214-105">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="9d214-106">OofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="9d214-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9d214-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d214-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d214-108">Attributes and elements</span></span>

<span data-ttu-id="9d214-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d214-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d214-110">属性</span><span class="sxs-lookup"><span data-stu-id="9d214-110">Attributes</span></span>

<span data-ttu-id="9d214-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9d214-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d214-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9d214-112">Child elements</span></span>

<span data-ttu-id="9d214-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9d214-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d214-114">親要素</span><span class="sxs-lookup"><span data-stu-id="9d214-114">Parent elements</span></span>

|<span data-ttu-id="9d214-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d214-115">**Element**</span></span>|<span data-ttu-id="9d214-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d214-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d214-117">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="9d214-118">[GetUMProperties 操作 (UM web サービス)](getumproperties-operation-um-web-service.md)要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9d214-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d214-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d214-119">Text value</span></span>

<span data-ttu-id="9d214-120">ブール値のテキスト値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d214-120">A Boolean text value is required.</span></span> <span data-ttu-id="9d214-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="9d214-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="9d214-122">True</span><span class="sxs-lookup"><span data-stu-id="9d214-122">True</span></span>
    
- <span data-ttu-id="9d214-123">False</span><span class="sxs-lookup"><span data-stu-id="9d214-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="9d214-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d214-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d214-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d214-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d214-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d214-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9d214-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="9d214-127">Messages</span></span>  <br/> |
|<span data-ttu-id="9d214-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d214-128">Validation File</span></span>  <br/> |<span data-ttu-id="9d214-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d214-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d214-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d214-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d214-131">False</span><span class="sxs-lookup"><span data-stu-id="9d214-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d214-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d214-132">See also</span></span>



[<span data-ttu-id="9d214-133">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="9d214-134">GetUMPropertiesResponse (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="9d214-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

