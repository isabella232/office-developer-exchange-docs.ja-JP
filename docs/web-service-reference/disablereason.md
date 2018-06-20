---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: DisableReason 要素は、アプリケーションを無効にする理由を指定します。
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760069"
---
# <a name="disablereason"></a><span data-ttu-id="4ee3b-103">DisableReason</span><span class="sxs-lookup"><span data-stu-id="4ee3b-103">DisableReason</span></span>

<span data-ttu-id="4ee3b-104">**DisableReason**要素は、アプリケーションを無効にする理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="4ee3b-105">**DisableReasonType**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ee3b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4ee3b-106">Attributes and elements</span></span>

<span data-ttu-id="4ee3b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ee3b-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ee3b-108">Attributes</span></span>

<span data-ttu-id="4ee3b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ee3b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ee3b-110">Child elements</span></span>

<span data-ttu-id="4ee3b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ee3b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4ee3b-112">Parent elements</span></span>

|<span data-ttu-id="4ee3b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-113">**Element**</span></span>|<span data-ttu-id="4ee3b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ee3b-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="4ee3b-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="4ee3b-116">アプリケーションを無効にする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ee3b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4ee3b-117">Text value</span></span>

<span data-ttu-id="4ee3b-118">**DisableReason 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="4ee3b-119">**値**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-119">**Value**</span></span>|<span data-ttu-id="4ee3b-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ee3b-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4ee3b-121">NoReason</span><span class="sxs-lookup"><span data-stu-id="4ee3b-121">NoReason</span></span>  <br/> |<span data-ttu-id="4ee3b-122">理由指定なし</span><span class="sxs-lookup"><span data-stu-id="4ee3b-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="4ee3b-123">OutlookClientPerformance</span><span class="sxs-lookup"><span data-stu-id="4ee3b-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="4ee3b-124">電子メール クライアントのパフォーマンスを向上させるには。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="4ee3b-125">OWAClientPerformance</span><span class="sxs-lookup"><span data-stu-id="4ee3b-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="4ee3b-126">Web アプリケーションのクライアントのパフォーマンスを向上します。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="4ee3b-127">MobileClientPerformance</span><span class="sxs-lookup"><span data-stu-id="4ee3b-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="4ee3b-128">モバイル クライアントのパフォーマンスを向上させるには。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ee3b-129">備考</span><span class="sxs-lookup"><span data-stu-id="4ee3b-129">Remarks</span></span>

<span data-ttu-id="4ee3b-130">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ee3b-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ee3b-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="4ee3b-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ee3b-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="4ee3b-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ee3b-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ee3b-134">Schema Name</span></span>  <br/> |<span data-ttu-id="4ee3b-135">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ee3b-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="4ee3b-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ee3b-136">Validation File</span></span>  <br/> |<span data-ttu-id="4ee3b-137">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ee3b-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ee3b-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4ee3b-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4ee3b-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ee3b-139">See also</span></span>

- [<span data-ttu-id="4ee3b-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ee3b-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

