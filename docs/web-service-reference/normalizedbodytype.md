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
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832554"
---
# <a name="normalizedbodytype"></a><span data-ttu-id="82200-103">NormalizedBodyType</span><span class="sxs-lookup"><span data-stu-id="82200-103">NormalizedBodyType</span></span>

<span data-ttu-id="82200-104">**NormalizedBodyType**要素は、正規化された本文がテキスト形式または HTML 形式で返されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="82200-104">The **NormalizedBodyType** element specifies whether the normalized body is returned in text or HTML format.</span></span> 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 <span data-ttu-id="82200-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="82200-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82200-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="82200-106">Attributes and elements</span></span>

<span data-ttu-id="82200-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82200-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82200-108">属性</span><span class="sxs-lookup"><span data-stu-id="82200-108">Attributes</span></span>

<span data-ttu-id="82200-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82200-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82200-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82200-110">Child elements</span></span>

<span data-ttu-id="82200-111">なし。</span><span class="sxs-lookup"><span data-stu-id="82200-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82200-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82200-112">Parent elements</span></span>

[<span data-ttu-id="82200-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="82200-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="82200-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82200-114">Text value</span></span>

<span data-ttu-id="82200-115">**NormalizedBodyType**要素のテキスト値は、正規化された本文の形式はことを示します。</span><span class="sxs-lookup"><span data-stu-id="82200-115">The text value of the **NormalizedBodyType** element indicates format the normalized body is returned in.</span></span> <span data-ttu-id="82200-116">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="82200-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="82200-117">**値**</span><span class="sxs-lookup"><span data-stu-id="82200-117">**Value**</span></span>|<span data-ttu-id="82200-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="82200-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="82200-119">ベスト</span><span class="sxs-lookup"><span data-stu-id="82200-119">Best</span></span>  <br/> |<span data-ttu-id="82200-120">応答には、本文テキストの豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="82200-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="82200-121">これは、コンテンツは、テキストまたは html 形式かどうか不明ではない場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="82200-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="82200-122">ストアド本文がテキスト形式の場合は、返された本文をテキストになります。</span><span class="sxs-lookup"><span data-stu-id="82200-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="82200-123">それ以外の場合、応答であっても、ストアドの本文が HTML または rtf 形式のいずれかの形式では場合、HTML が返されます。</span><span class="sxs-lookup"><span data-stu-id="82200-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="82200-124">既定値です。</span><span class="sxs-lookup"><span data-stu-id="82200-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="82200-125">HTML</span><span class="sxs-lookup"><span data-stu-id="82200-125">HTML</span></span>  <br/> |<span data-ttu-id="82200-126">応答では、html 形式で正規化された本文を返します。</span><span class="sxs-lookup"><span data-stu-id="82200-126">The response will return a normalized body as HTML.</span></span>  <br/> |
|<span data-ttu-id="82200-127">テキスト型 (Text)</span><span class="sxs-lookup"><span data-stu-id="82200-127">Text</span></span>  <br/> |<span data-ttu-id="82200-128">応答には、テキスト形式で正規化された本文が返されます。</span><span class="sxs-lookup"><span data-stu-id="82200-128">The response will return a normalized body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="82200-129">備考</span><span class="sxs-lookup"><span data-stu-id="82200-129">Remarks</span></span>

<span data-ttu-id="82200-130">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="82200-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="82200-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="82200-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82200-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="82200-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82200-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="82200-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82200-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82200-134">Schema Name</span></span>  <br/> |<span data-ttu-id="82200-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="82200-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="82200-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82200-136">Validation File</span></span>  <br/> |<span data-ttu-id="82200-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="82200-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82200-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82200-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="82200-139">True</span><span class="sxs-lookup"><span data-stu-id="82200-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82200-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="82200-140">See also</span></span>



[<span data-ttu-id="82200-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="82200-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="82200-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="82200-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

