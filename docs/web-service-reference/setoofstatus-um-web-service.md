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
description: SetOofStatus 要素は、要求を行うユーザーのユニファイドメッセージング不在 (OOF) 状態を設定するための要求を定義します。
ms.openlocfilehash: 86e056a440e282cd444cfd405e452720b26b7456
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467068"
---
# <a name="setoofstatus-um-web-service"></a><span data-ttu-id="3c9f3-103">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="3c9f3-103">SetOofStatus (UM web service)</span></span>

<span data-ttu-id="3c9f3-104">**Setoofstatus**要素は、要求を行うユーザーのユニファイドメッセージング不在 (OOF) 状態を設定するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-104">The **SetOofStatus** element defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span> 
  
[<span data-ttu-id="3c9f3-105">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="3c9f3-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="3c9f3-106">**種類**</span><span class="sxs-lookup"><span data-stu-id="3c9f3-106">**Type**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c9f3-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3c9f3-107">Attributes and elements</span></span>

<span data-ttu-id="3c9f3-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c9f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="3c9f3-109">Attributes</span></span>

<span data-ttu-id="3c9f3-110">なし。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c9f3-111">子要素</span><span class="sxs-lookup"><span data-stu-id="3c9f3-111">Child elements</span></span>

|<span data-ttu-id="3c9f3-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="3c9f3-112">**Element**</span></span>|<span data-ttu-id="3c9f3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="3c9f3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c9f3-114">状態 (UM web サービス-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="3c9f3-114">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md) <br/> |<span data-ttu-id="3c9f3-115">[Setoofstatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)要求で使用する値を定義します。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-115">Defines a value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c9f3-116">親要素</span><span class="sxs-lookup"><span data-stu-id="3c9f3-116">Parent elements</span></span>

<span data-ttu-id="3c9f3-117">なし。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3c9f3-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3c9f3-118">Text value</span></span>

<span data-ttu-id="3c9f3-119">なし。</span><span class="sxs-lookup"><span data-stu-id="3c9f3-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c9f3-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3c9f3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c9f3-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c9f3-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c9f3-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3c9f3-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3c9f3-123">メッセージ</span><span class="sxs-lookup"><span data-stu-id="3c9f3-123">Messages</span></span>  <br/> |
|<span data-ttu-id="3c9f3-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3c9f3-124">Validation File</span></span>  <br/> |<span data-ttu-id="3c9f3-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3c9f3-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c9f3-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3c9f3-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c9f3-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="3c9f3-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c9f3-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="3c9f3-128">See also</span></span>



[<span data-ttu-id="3c9f3-129">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="3c9f3-129">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
  
[<span data-ttu-id="3c9f3-130">状態 (UM web サービス-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="3c9f3-130">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

