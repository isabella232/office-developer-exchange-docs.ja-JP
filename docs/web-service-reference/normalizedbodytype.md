---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: NormalizedBodyType 要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。
ms.openlocfilehash: e5d968673403eba24a68c67175e3ebcbb35eca39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462662"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="3c498-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="3c498-103">NormalizedBodyType</span></span>

<span data-ttu-id="3c498-104">**Normalizedbodytype**要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="3c498-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="3c498-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="3c498-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c498-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3c498-106">Attributes and elements</span></span>

<span data-ttu-id="3c498-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3c498-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c498-108">属性</span><span class="sxs-lookup"><span data-stu-id="3c498-108">Attributes</span></span>

<span data-ttu-id="3c498-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3c498-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c498-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3c498-110">Child elements</span></span>

<span data-ttu-id="3c498-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3c498-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c498-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3c498-112">Parent elements</span></span>

[<span data-ttu-id="3c498-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3c498-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="3c498-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3c498-114">Text value</span></span>

<span data-ttu-id="3c498-115">**Normalizedbodytype**要素のテキスト値は、正規化された本文が返される形式を示します。</span><span class="sxs-lookup"><span data-stu-id="3c498-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="3c498-116">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="3c498-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="3c498-117">**値**</span><span class="sxs-lookup"><span data-stu-id="3c498-117">**Value**</span></span>|<span data-ttu-id="3c498-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="3c498-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3c498-119">高</span><span class="sxs-lookup"><span data-stu-id="3c498-119">Best</span></span>  <br/> |<span data-ttu-id="3c498-120">応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="3c498-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="3c498-121">これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="3c498-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="3c498-122">保存された本文がプレーンテキストの場合、返される本文はテキストになります。</span><span class="sxs-lookup"><span data-stu-id="3c498-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="3c498-123">それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。</span><span class="sxs-lookup"><span data-stu-id="3c498-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="3c498-124">これは既定の値です。</span><span class="sxs-lookup"><span data-stu-id="3c498-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="3c498-125">HTML</span><span class="sxs-lookup"><span data-stu-id="3c498-125">HTML</span></span>  <br/> |<span data-ttu-id="3c498-126">応答は、正規化された本文を HTML として返します。</span><span class="sxs-lookup"><span data-stu-id="3c498-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="3c498-127">テキスト</span><span class="sxs-lookup"><span data-stu-id="3c498-127">Text</span></span>  <br/> |<span data-ttu-id="3c498-128">応答は、正規化された本文をプレーンテキストとして返します。</span><span class="sxs-lookup"><span data-stu-id="3c498-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3c498-129">注釈</span><span class="sxs-lookup"><span data-stu-id="3c498-129">Remarks</span></span>

<span data-ttu-id="3c498-130">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3c498-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3c498-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3c498-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c498-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3c498-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c498-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c498-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c498-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3c498-134">Schema Name</span></span>  <br/> |<span data-ttu-id="3c498-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="3c498-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c498-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3c498-136">Validation File</span></span>  <br/> |<span data-ttu-id="3c498-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3c498-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c498-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3c498-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c498-139">正しい</span><span class="sxs-lookup"><span data-stu-id="3c498-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c498-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="3c498-140">See also</span></span>



[<span data-ttu-id="3c498-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="3c498-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="3c498-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3c498-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

