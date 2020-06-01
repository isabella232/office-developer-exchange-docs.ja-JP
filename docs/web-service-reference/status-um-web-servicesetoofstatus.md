---
title: 状態 (UM web サービス-SetOofStatus)
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
description: Status 要素は、SetOofStatus 操作 (UM web サービス) 要求で使用する値を定義します。
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459981"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="aa6ec-103">状態 (UM web サービス-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="aa6ec-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="aa6ec-104">**Status**要素は、 [setoofstatus 操作 (UM web サービス)](setoofstatus-operation-um-web-service.md)要求で使用する値を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="aa6ec-105">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa6ec-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="aa6ec-106">状態 (UM web サービス-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="aa6ec-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="aa6ec-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="aa6ec-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa6ec-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aa6ec-108">Attributes and elements</span></span>

<span data-ttu-id="aa6ec-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa6ec-110">属性</span><span class="sxs-lookup"><span data-stu-id="aa6ec-110">Attributes</span></span>

<span data-ttu-id="aa6ec-111">なし。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa6ec-112">子要素</span><span class="sxs-lookup"><span data-stu-id="aa6ec-112">Child elements</span></span>

<span data-ttu-id="aa6ec-113">なし。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa6ec-114">親要素</span><span class="sxs-lookup"><span data-stu-id="aa6ec-114">Parent elements</span></span>

|<span data-ttu-id="aa6ec-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa6ec-115">**Element**</span></span>|<span data-ttu-id="aa6ec-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa6ec-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa6ec-117">SetOofStatus (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa6ec-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="aa6ec-118">要求を行ったユーザーのユニファイドメッセージングの不在 (OOF) 状態を設定するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa6ec-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aa6ec-119">Text value</span></span>

<span data-ttu-id="aa6ec-120">ブール値が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-120">A Boolean value is required.</span></span> <span data-ttu-id="aa6ec-121">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="aa6ec-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="aa6ec-122">True</span><span class="sxs-lookup"><span data-stu-id="aa6ec-122">True</span></span>
    
- <span data-ttu-id="aa6ec-123">False</span><span class="sxs-lookup"><span data-stu-id="aa6ec-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="aa6ec-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aa6ec-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa6ec-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa6ec-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="aa6ec-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa6ec-126">Schema Name</span></span>  <br/> |<span data-ttu-id="aa6ec-127">メッセージ</span><span class="sxs-lookup"><span data-stu-id="aa6ec-127">Messages</span></span>  <br/> |
|<span data-ttu-id="aa6ec-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa6ec-128">Validation File</span></span>  <br/> |<span data-ttu-id="aa6ec-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aa6ec-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa6ec-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa6ec-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa6ec-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="aa6ec-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa6ec-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa6ec-132">See also</span></span>



[<span data-ttu-id="aa6ec-133">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="aa6ec-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

