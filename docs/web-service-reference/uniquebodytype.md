---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: UniqueBodyType 要素は、一意の本文がテキスト形式または HTML 形式のどちらで返されるかを指定します。
ms.openlocfilehash: 7e6c4631ef589555ce4d5da747c200ffe956f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459441"
---
# <a name="uniquebodytype"></a><span data-ttu-id="50343-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="50343-103">UniqueBodyType</span></span>

<span data-ttu-id="50343-104">**UniqueBodyType**要素は、一意の本文がテキスト形式または HTML 形式のどちらで返されるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="50343-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="50343-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="50343-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50343-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="50343-106">Attributes and elements</span></span>

<span data-ttu-id="50343-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50343-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50343-108">属性</span><span class="sxs-lookup"><span data-stu-id="50343-108">Attributes</span></span>

<span data-ttu-id="50343-109">なし。</span><span class="sxs-lookup"><span data-stu-id="50343-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50343-110">子要素</span><span class="sxs-lookup"><span data-stu-id="50343-110">Child elements</span></span>

<span data-ttu-id="50343-111">なし。</span><span class="sxs-lookup"><span data-stu-id="50343-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50343-112">親要素</span><span class="sxs-lookup"><span data-stu-id="50343-112">Parent elements</span></span>

[<span data-ttu-id="50343-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="50343-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="50343-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="50343-114">Text value</span></span>

<span data-ttu-id="50343-115">**UniqueBodyType**要素のテキスト値は、で一意の本文が返される形式を示します。</span><span class="sxs-lookup"><span data-stu-id="50343-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="50343-116">次の表に、この要素で使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="50343-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="50343-117">**値**</span><span class="sxs-lookup"><span data-stu-id="50343-117">**Value**</span></span>|<span data-ttu-id="50343-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="50343-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="50343-119">高</span><span class="sxs-lookup"><span data-stu-id="50343-119">Best</span></span>  <br/> |<span data-ttu-id="50343-120">応答によって、本文の中で最も豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="50343-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="50343-121">これは、コンテンツがテキストであるか HTML であるかにかかわらず、不明な場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="50343-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="50343-122">保存された本文がプレーンテキストの場合、返される本文はテキストになります。</span><span class="sxs-lookup"><span data-stu-id="50343-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="50343-123">それ以外の場合、保存された本文が HTML または RTF 形式の場合、応答は HTML を返します。</span><span class="sxs-lookup"><span data-stu-id="50343-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="50343-124">これは既定の値です。</span><span class="sxs-lookup"><span data-stu-id="50343-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="50343-125">HTML</span><span class="sxs-lookup"><span data-stu-id="50343-125">HTML</span></span>  <br/> |<span data-ttu-id="50343-126">応答は、一意の本文を HTML として返します。</span><span class="sxs-lookup"><span data-stu-id="50343-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="50343-127">テキスト</span><span class="sxs-lookup"><span data-stu-id="50343-127">Text</span></span>  <br/> |<span data-ttu-id="50343-128">応答は、プレーンテキストとして一意の本文を返します。</span><span class="sxs-lookup"><span data-stu-id="50343-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50343-129">注釈</span><span class="sxs-lookup"><span data-stu-id="50343-129">Remarks</span></span>

<span data-ttu-id="50343-130">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="50343-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="50343-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="50343-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50343-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="50343-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50343-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="50343-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50343-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="50343-134">Schema Name</span></span>  <br/> |<span data-ttu-id="50343-135">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="50343-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="50343-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="50343-136">Validation File</span></span>  <br/> |<span data-ttu-id="50343-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="50343-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50343-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="50343-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="50343-139">正しい</span><span class="sxs-lookup"><span data-stu-id="50343-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50343-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="50343-140">See also</span></span>



[<span data-ttu-id="50343-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="50343-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="50343-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="50343-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

