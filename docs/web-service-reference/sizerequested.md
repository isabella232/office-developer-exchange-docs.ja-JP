---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: SizeRequested 要素には、GetUserPhoto 操作に対して要求された写真のサイズが含まれています。
ms.openlocfilehash: 2e79bbb158fa9a22cbd3ec08fcd6e60429e113b4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460457"
---
# <a name="sizerequested"></a><span data-ttu-id="4bd46-103">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="4bd46-103">SizeRequested</span></span>

<span data-ttu-id="4bd46-104">**SizeRequested**要素には、 **getuserphoto**操作に対して要求された写真のサイズが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4bd46-104">The **SizeRequested** element contains the requested photo size for a **GetUserPhoto** operation.</span></span> 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 <span data-ttu-id="4bd46-105">**UserPhotoSizeType**</span><span class="sxs-lookup"><span data-stu-id="4bd46-105">**UserPhotoSizeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bd46-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4bd46-106">Attributes and elements</span></span>

<span data-ttu-id="4bd46-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4bd46-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bd46-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bd46-108">Attributes</span></span>

<span data-ttu-id="4bd46-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4bd46-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bd46-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4bd46-110">Child elements</span></span>

<span data-ttu-id="4bd46-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4bd46-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4bd46-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4bd46-112">Parent elements</span></span>

[<span data-ttu-id="4bd46-113">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="4bd46-113">GetUserPhoto</span></span>](getuserphoto.md)
  
## <a name="text-value"></a><span data-ttu-id="4bd46-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4bd46-114">Text value</span></span>

<span data-ttu-id="4bd46-115">**SizeRequested**要素のテキスト値は、サーバーから返されるデジタルイメージの要求された写真のサイズです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-115">The text value of the **SizeRequested** element is the requested photo size of a digital image returned from the server.</span></span> <span data-ttu-id="4bd46-116">次の表は、 **SizeRequested**要素のテキスト値を示しています。</span><span class="sxs-lookup"><span data-stu-id="4bd46-116">The following table identifies the text values for the **SizeRequested** element.</span></span> 
  
|<span data-ttu-id="4bd46-117">**値**</span><span class="sxs-lookup"><span data-stu-id="4bd46-117">**Value**</span></span>|<span data-ttu-id="4bd46-118">**意味**</span><span class="sxs-lookup"><span data-stu-id="4bd46-118">**Meaning**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4bd46-119">HR48x48</span><span class="sxs-lookup"><span data-stu-id="4bd46-119">HR48x48</span></span>  <br/> |<span data-ttu-id="4bd46-120">画像の幅は48ピクセル、高さは48ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-120">The image is 48 pixels high and 48 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-121">HR64x64</span><span class="sxs-lookup"><span data-stu-id="4bd46-121">HR64x64</span></span>  <br/> |<span data-ttu-id="4bd46-122">画像の幅は64ピクセル、高さは64ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-122">The image is 64 pixels high and 64 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-123">HR96x96</span><span class="sxs-lookup"><span data-stu-id="4bd46-123">HR96x96</span></span>  <br/> |<span data-ttu-id="4bd46-124">画像の幅は96ピクセル、高さは96ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-124">The image is 96 pixels high and 96 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-125">HR120x120</span><span class="sxs-lookup"><span data-stu-id="4bd46-125">HR120x120</span></span>  <br/> |<span data-ttu-id="4bd46-126">画像の幅は120ピクセル、高さは120ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-126">The image is 120 pixels high and 120 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-127">HR240x240</span><span class="sxs-lookup"><span data-stu-id="4bd46-127">HR240x240</span></span>  <br/> |<span data-ttu-id="4bd46-128">画像の幅は240ピクセル、高さは240ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-128">The image is 240 pixels high and 240 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-129">HR360x360</span><span class="sxs-lookup"><span data-stu-id="4bd46-129">HR360x360</span></span>  <br/> |<span data-ttu-id="4bd46-130">画像の幅は360ピクセル、高さは360ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-130">The image is 360 pixels high and 360 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-131">HR432x432</span><span class="sxs-lookup"><span data-stu-id="4bd46-131">HR432x432</span></span>  <br/> |<span data-ttu-id="4bd46-132">画像の幅は432ピクセル、高さは432ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-132">The image is 432 pixels high and 432 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-133">HR504x504</span><span class="sxs-lookup"><span data-stu-id="4bd46-133">HR504x504</span></span>  <br/> |<span data-ttu-id="4bd46-134">画像の幅は504ピクセル、高さは504ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-134">The image is 504 pixels high and 504 pixels wide.</span></span>  <br/> |
|<span data-ttu-id="4bd46-135">HR648x648</span><span class="sxs-lookup"><span data-stu-id="4bd46-135">HR648x648</span></span>  <br/> |<span data-ttu-id="4bd46-136">画像の幅は648ピクセル、高さは648ピクセルです。</span><span class="sxs-lookup"><span data-stu-id="4bd46-136">The image is 648 pixels high and 648 pixels wide.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4bd46-137">注釈</span><span class="sxs-lookup"><span data-stu-id="4bd46-137">Remarks</span></span>

<span data-ttu-id="4bd46-138">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4bd46-138">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4bd46-139">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4bd46-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bd46-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4bd46-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bd46-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bd46-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4bd46-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4bd46-142">Schema name</span></span>  <br/> |<span data-ttu-id="4bd46-143">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4bd46-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4bd46-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4bd46-144">Validation file</span></span>  <br/> |<span data-ttu-id="4bd46-145">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4bd46-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4bd46-146">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4bd46-146">Can be empty</span></span>  <br/> ||
   

