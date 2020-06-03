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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463672"
---
# <a name="disablereason"></a><span data-ttu-id="675fc-103">DisableReason</span><span class="sxs-lookup"><span data-stu-id="675fc-103">DisableReason</span></span>

<span data-ttu-id="675fc-104">**DisableReason**要素は、アプリを無効にする理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="675fc-104">The **DisableReason** element specifies the reason for disabling an app.</span></span> 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 <span data-ttu-id="675fc-105">**DisableReasonType**</span><span class="sxs-lookup"><span data-stu-id="675fc-105">**DisableReasonType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="675fc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="675fc-106">Attributes and elements</span></span>

<span data-ttu-id="675fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="675fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="675fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="675fc-108">Attributes</span></span>

<span data-ttu-id="675fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="675fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="675fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="675fc-110">Child elements</span></span>

<span data-ttu-id="675fc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="675fc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="675fc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="675fc-112">Parent elements</span></span>

|<span data-ttu-id="675fc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="675fc-113">**Element**</span></span>|<span data-ttu-id="675fc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="675fc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="675fc-115">DisableApp</span><span class="sxs-lookup"><span data-stu-id="675fc-115">DisableApp</span></span>](disableapp.md) <br/> |<span data-ttu-id="675fc-116">アプリを無効にする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="675fc-116">Specifies a request to disable an app.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="675fc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="675fc-117">Text value</span></span>

<span data-ttu-id="675fc-118">**DisableReason 要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="675fc-118">**DisableReason element text value**</span></span>

|<span data-ttu-id="675fc-119">**値**</span><span class="sxs-lookup"><span data-stu-id="675fc-119">**Value**</span></span>|<span data-ttu-id="675fc-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="675fc-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="675fc-121">NoReason</span><span class="sxs-lookup"><span data-stu-id="675fc-121">NoReason</span></span>  <br/> |<span data-ttu-id="675fc-122">理由の指定なし</span><span class="sxs-lookup"><span data-stu-id="675fc-122">No reason given</span></span>  <br/> |
|<span data-ttu-id="675fc-123">OutlookClientPerformance</span><span class="sxs-lookup"><span data-stu-id="675fc-123">OutlookClientPerformance</span></span>  <br/> |<span data-ttu-id="675fc-124">電子メールクライアントのパフォーマンスを向上させるため。</span><span class="sxs-lookup"><span data-stu-id="675fc-124">To improve email client performance.</span></span>  <br/> |
|<span data-ttu-id="675fc-125">OWAClientPerformance</span><span class="sxs-lookup"><span data-stu-id="675fc-125">OWAClientPerformance</span></span>  <br/> |<span data-ttu-id="675fc-126">Web アプリクライアントのパフォーマンスを向上させる。</span><span class="sxs-lookup"><span data-stu-id="675fc-126">To improve Web app client performance.</span></span>  <br/> |
|<span data-ttu-id="675fc-127">MobileClientPerformance</span><span class="sxs-lookup"><span data-stu-id="675fc-127">MobileClientPerformance</span></span>  <br/> |<span data-ttu-id="675fc-128">モバイルクライアントのパフォーマンスを向上させる。</span><span class="sxs-lookup"><span data-stu-id="675fc-128">To improve mobile client performance.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="675fc-129">注釈</span><span class="sxs-lookup"><span data-stu-id="675fc-129">Remarks</span></span>

<span data-ttu-id="675fc-130">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="675fc-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="675fc-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="675fc-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="675fc-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="675fc-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="675fc-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="675fc-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="675fc-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="675fc-134">Schema Name</span></span>  <br/> |<span data-ttu-id="675fc-135">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="675fc-135">Type schema</span></span>  <br/> |
|<span data-ttu-id="675fc-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="675fc-136">Validation File</span></span>  <br/> |<span data-ttu-id="675fc-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="675fc-137">types.xsd</span></span>  <br/> |
|<span data-ttu-id="675fc-138">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="675fc-138">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="675fc-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="675fc-139">See also</span></span>

- [<span data-ttu-id="675fc-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="675fc-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

