---
title: 状態 (UM web サービス - SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: 状態の要素は、SetOofStatus 操作 (UM web サービス) 要求に使用する値を定義します。
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833583"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="aa93b-103">状態 (UM web サービス - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="aa93b-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="aa93b-104">**状態**の要素は、 [SetOofStatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)の要求で使用する値を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa93b-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="aa93b-105">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa93b-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="aa93b-106">状態 (UM web サービス - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="aa93b-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="aa93b-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="aa93b-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa93b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="aa93b-108">Attributes and elements</span></span>

<span data-ttu-id="aa93b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa93b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa93b-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa93b-110">Attributes</span></span>

<span data-ttu-id="aa93b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="aa93b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa93b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="aa93b-112">Child elements</span></span>

<span data-ttu-id="aa93b-113">なし。</span><span class="sxs-lookup"><span data-stu-id="aa93b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa93b-114">親要素</span><span class="sxs-lookup"><span data-stu-id="aa93b-114">Parent elements</span></span>

|<span data-ttu-id="aa93b-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa93b-115">**Element**</span></span>|<span data-ttu-id="aa93b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa93b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa93b-117">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa93b-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="aa93b-118">要求は、ユーザーのユニファイド メッセージングの Office (OOF) の状態を設定する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa93b-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa93b-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aa93b-119">Text value</span></span>

<span data-ttu-id="aa93b-120">ブール値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa93b-120">A Boolean value is required.</span></span> <span data-ttu-id="aa93b-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="aa93b-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="aa93b-122">True</span><span class="sxs-lookup"><span data-stu-id="aa93b-122">True</span></span>
    
- <span data-ttu-id="aa93b-123">False</span><span class="sxs-lookup"><span data-stu-id="aa93b-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="aa93b-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="aa93b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa93b-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="aa93b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa93b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa93b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="aa93b-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="aa93b-127">Messages</span></span>  <br/> |
|<span data-ttu-id="aa93b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa93b-128">Validation File</span></span>  <br/> |<span data-ttu-id="aa93b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aa93b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa93b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa93b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa93b-131">False</span><span class="sxs-lookup"><span data-stu-id="aa93b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa93b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa93b-132">See also</span></span>



[<span data-ttu-id="aa93b-133">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa93b-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

