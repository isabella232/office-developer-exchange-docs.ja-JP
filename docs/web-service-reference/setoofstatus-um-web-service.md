---
title: SetOofStatus (UM web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 9fc0ea9c-7a98-4fd7-a90c-cf5639c63a3a
description: SetOofStatus 要素は、要求したユーザーのユニファイド メッセージングの Office (OOF) の状態を設定する要求を定義します。
ms.openlocfilehash: df28c98013e1d5c00ea120ce1aa342e9fc2c6f31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833447"
---
# <a name="setoofstatus-um-web-service"></a><span data-ttu-id="40a93-103">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="40a93-103">SetOofStatus (UM web service)</span></span>

<span data-ttu-id="40a93-104">**SetOofStatus**要素は、要求したユーザーのユニファイド メッセージングの Office (OOF) の状態を設定する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="40a93-104">The **SetOofStatus** element defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span> 
  
[<span data-ttu-id="40a93-105">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="40a93-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="40a93-106">**型**</span><span class="sxs-lookup"><span data-stu-id="40a93-106">**Type**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40a93-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="40a93-107">Attributes and elements</span></span>

<span data-ttu-id="40a93-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="40a93-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40a93-109">属性</span><span class="sxs-lookup"><span data-stu-id="40a93-109">Attributes</span></span>

<span data-ttu-id="40a93-110">なし。</span><span class="sxs-lookup"><span data-stu-id="40a93-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40a93-111">子要素</span><span class="sxs-lookup"><span data-stu-id="40a93-111">Child elements</span></span>

|<span data-ttu-id="40a93-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="40a93-112">**Element**</span></span>|<span data-ttu-id="40a93-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="40a93-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40a93-114">状態 (UM web サービス - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="40a93-114">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md) <br/> |<span data-ttu-id="40a93-115">[SetOofStatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)の要求で使用する値を定義します。</span><span class="sxs-lookup"><span data-stu-id="40a93-115">Defines a value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40a93-116">親要素</span><span class="sxs-lookup"><span data-stu-id="40a93-116">Parent elements</span></span>

<span data-ttu-id="40a93-117">なし。</span><span class="sxs-lookup"><span data-stu-id="40a93-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="40a93-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="40a93-118">Text value</span></span>

<span data-ttu-id="40a93-119">なし。</span><span class="sxs-lookup"><span data-stu-id="40a93-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40a93-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="40a93-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40a93-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="40a93-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="40a93-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="40a93-122">Schema Name</span></span>  <br/> |<span data-ttu-id="40a93-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="40a93-123">Messages</span></span>  <br/> |
|<span data-ttu-id="40a93-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="40a93-124">Validation File</span></span>  <br/> |<span data-ttu-id="40a93-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="40a93-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="40a93-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="40a93-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="40a93-127">False</span><span class="sxs-lookup"><span data-stu-id="40a93-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40a93-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="40a93-128">See also</span></span>



[<span data-ttu-id="40a93-129">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="40a93-129">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
  
[<span data-ttu-id="40a93-130">状態 (UM web サービス - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="40a93-130">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

