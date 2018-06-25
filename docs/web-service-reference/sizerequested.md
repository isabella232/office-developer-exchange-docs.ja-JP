---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: SizeRequested 要素には、GetUserPhoto 操作の要求された写真のサイズが含まれています。
ms.openlocfilehash: 43e422512b1e8f06e410e533e9ae1dc49283d5f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833504"
---
# <a name="sizerequested"></a><span data-ttu-id="788c3-103">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="788c3-103">SizeRequested</span></span>

<span data-ttu-id="788c3-104">**SizeRequested**要素には、 **GetUserPhoto**操作の要求された写真のサイズが含まれています。</span><span class="sxs-lookup"><span data-stu-id="788c3-104">The **SizeRequested** element contains the requested photo size for a **GetUserPhoto** operation.</span></span> 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 <span data-ttu-id="788c3-105">**UserPhotoSizeType**</span><span class="sxs-lookup"><span data-stu-id="788c3-105">**UserPhotoSizeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="788c3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="788c3-106">Attributes and elements</span></span>

<span data-ttu-id="788c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="788c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="788c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="788c3-108">Attributes</span></span>

<span data-ttu-id="788c3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="788c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="788c3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="788c3-110">Child elements</span></span>

<span data-ttu-id="788c3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="788c3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="788c3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="788c3-112">Parent elements</span></span>

[<span data-ttu-id="788c3-113">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="788c3-113">GetUserPhoto</span></span>](getuserphoto.md)
  
## <a name="text-value"></a><span data-ttu-id="788c3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="788c3-114">Text value</span></span>

<span data-ttu-id="788c3-115">**SizeRequested**要素のテキスト値は、サーバーから返されるデジタル画像の写真を要求されたサイズです。</span><span class="sxs-lookup"><span data-stu-id="788c3-115">The text value of the **SizeRequested** element is the requested photo size of a digital image returned from the server.</span></span> <span data-ttu-id="788c3-116">次の表は、 **SizeRequested**要素のテキスト値を識別します。</span><span class="sxs-lookup"><span data-stu-id="788c3-116">The following table identifies the text values for the **SizeRequested** element.</span></span> 
  
|<span data-ttu-id="788c3-117">**値**</span><span class="sxs-lookup"><span data-stu-id="788c3-117">**Value**</span></span>|<span data-ttu-id="788c3-118">**意味**</span><span class="sxs-lookup"><span data-stu-id="788c3-118">**Meaning**</span></span>|
|:-----|:-----|
|<span data-ttu-id="788c3-119">HR48x48</span><span class="sxs-lookup"><span data-stu-id="788c3-119">HR48x48</span></span>  <br/> |<span data-ttu-id="788c3-120">イメージは、48 ピクセル、高さと幅 48 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-120">The image is 48 pixels high and 48 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-121">HR64x64</span><span class="sxs-lookup"><span data-stu-id="788c3-121">HR64x64</span></span>  <br/> |<span data-ttu-id="788c3-122">イメージは 64 ピクセル、高さと幅は 64 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-122">The image is 64 pixels high and 64 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-123">HR96x96</span><span class="sxs-lookup"><span data-stu-id="788c3-123">HR96x96</span></span>  <br/> |<span data-ttu-id="788c3-124">イメージは、96 ピクセル、高さと幅が 96 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-124">The image is 96 pixels high and 96 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-125">HR120x120</span><span class="sxs-lookup"><span data-stu-id="788c3-125">HR120x120</span></span>  <br/> |<span data-ttu-id="788c3-126">イメージは、120 ピクセル、高さと幅が 120 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-126">The image is 120 pixels high and 120 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-127">HR240x240</span><span class="sxs-lookup"><span data-stu-id="788c3-127">HR240x240</span></span>  <br/> |<span data-ttu-id="788c3-128">イメージは、高さ 240 ピクセル、幅 240 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-128">The image is 240 pixels high and 240 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-129">HR360x360</span><span class="sxs-lookup"><span data-stu-id="788c3-129">HR360x360</span></span>  <br/> |<span data-ttu-id="788c3-130">イメージは 360 ピクセル、高さと幅が 360 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-130">The image is 360 pixels high and 360 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-131">HR432x432</span><span class="sxs-lookup"><span data-stu-id="788c3-131">HR432x432</span></span>  <br/> |<span data-ttu-id="788c3-132">イメージは、432 ピクセル、高さと幅 432 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-132">The image is 432 pixels high and 432 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-133">HR504x504</span><span class="sxs-lookup"><span data-stu-id="788c3-133">HR504x504</span></span>  <br/> |<span data-ttu-id="788c3-134">イメージは、504 ピクセル、高さと幅は 504 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-134">The image is 504 pixels high and 504 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="788c3-135">HR648x648</span><span class="sxs-lookup"><span data-stu-id="788c3-135">HR648x648</span></span>  <br/> |<span data-ttu-id="788c3-136">イメージは、648 ピクセル、高さと幅が 648 ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="788c3-136">The image is 648 pixels high and 648 pixels wide.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="788c3-137">備考</span><span class="sxs-lookup"><span data-stu-id="788c3-137">Remarks</span></span>

<span data-ttu-id="788c3-138">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="788c3-138">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="788c3-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="788c3-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="788c3-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="788c3-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="788c3-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="788c3-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="788c3-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="788c3-142">Schema name</span></span>  <br/> |<span data-ttu-id="788c3-143">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="788c3-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="788c3-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="788c3-144">Validation file</span></span>  <br/> |<span data-ttu-id="788c3-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="788c3-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="788c3-146">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="788c3-146">Can be empty</span></span>  <br/> ||
   

