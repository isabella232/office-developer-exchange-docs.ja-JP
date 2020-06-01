---
title: DisableReason
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: DisableReason 要素は、アプリを無効にする理由を指定します。
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463672"
---
# <a name="disablereason"></a><span data-ttu-id="210b1-103">DisableReason</span><span class="sxs-lookup"><span data-stu-id="210b1-103">DisableReason</span></span>

<span data-ttu-id="210b1-104">**DisableReason**要素は、アプリを無効にする理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="210b1-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="210b1-105">**DisableReasonType**</span><span class="sxs-lookup"><span data-stu-id="210b1-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="210b1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="210b1-106">Attributes and elements</span></span>

<span data-ttu-id="210b1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="210b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="210b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="210b1-108">Attributes</span></span>

<span data-ttu-id="210b1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="210b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="210b1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="210b1-110">Child elements</span></span>

<span data-ttu-id="210b1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="210b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="210b1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="210b1-112">Parent elements</span></span>

|<span data-ttu-id="210b1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="210b1-113">**Element**</span></span>|<span data-ttu-id="210b1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="210b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="210b1-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="210b1-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="210b1-116">アプリを無効にする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="210b1-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="210b1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="210b1-117">Text value</span></span>

<span data-ttu-id="210b1-118">**DisableReason 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="210b1-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="210b1-119">**値**</span><span class="sxs-lookup"><span data-stu-id="210b1-119">**Value**</span></span>|<span data-ttu-id="210b1-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="210b1-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="210b1-121">NoReason</span><span class="sxs-lookup"><span data-stu-id="210b1-121">NoReason</span></span>  <br/> |<span data-ttu-id="210b1-122">理由の指定なし</span><span class="sxs-lookup"><span data-stu-id="210b1-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="210b1-123">OutlookClientPerformance</span><span class="sxs-lookup"><span data-stu-id="210b1-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="210b1-124">電子メールクライアントのパフォーマンスを向上させるため。</span><span class="sxs-lookup"><span data-stu-id="210b1-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="210b1-125">OWAClientPerformance</span><span class="sxs-lookup"><span data-stu-id="210b1-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="210b1-126">Web アプリクライアントのパフォーマンスを向上させる。</span><span class="sxs-lookup"><span data-stu-id="210b1-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="210b1-127">MobileClientPerformance</span><span class="sxs-lookup"><span data-stu-id="210b1-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="210b1-128">モバイルクライアントのパフォーマンスを向上させる。</span><span class="sxs-lookup"><span data-stu-id="210b1-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="210b1-129">注釈</span><span class="sxs-lookup"><span data-stu-id="210b1-129">Remarks</span></span>

<span data-ttu-id="210b1-130">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="210b1-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="210b1-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="210b1-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="210b1-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="210b1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="210b1-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="210b1-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="210b1-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="210b1-134">Schema Name</span></span>  <br/> |<span data-ttu-id="210b1-135">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="210b1-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="210b1-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="210b1-136">Validation File</span></span>  <br/> |<span data-ttu-id="210b1-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="210b1-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="210b1-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="210b1-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="210b1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="210b1-139">See also</span></span>

- [<span data-ttu-id="210b1-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="210b1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

