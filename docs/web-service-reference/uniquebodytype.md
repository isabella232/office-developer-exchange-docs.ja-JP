---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: UniqueBodyType 要素は、一意の本文をテキスト形式または HTML 形式で返すかどうかを指定します。
ms.openlocfilehash: c6eb4ec4e39a0c5355775a635db4c63efc666820
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839796"
---
# <a name="uniquebodytype"></a><span data-ttu-id="afb09-103">UniqueBodyType</span><span class="sxs-lookup"><span data-stu-id="afb09-103">UniqueBodyType</span></span>

<span data-ttu-id="afb09-104">**UniqueBodyType**要素は、一意の本文をテキスト形式または HTML 形式で返すかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="afb09-104">The **UniqueBodyType** element specifies whether the unique body is returned in text or HTML format.</span></span> 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 <span data-ttu-id="afb09-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="afb09-105">**BodyTypeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afb09-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="afb09-106">Attributes and elements</span></span>

<span data-ttu-id="afb09-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afb09-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afb09-108">属性</span><span class="sxs-lookup"><span data-stu-id="afb09-108">Attributes</span></span>

<span data-ttu-id="afb09-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afb09-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afb09-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afb09-110">Child elements</span></span>

<span data-ttu-id="afb09-111">なし。</span><span class="sxs-lookup"><span data-stu-id="afb09-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afb09-112">親要素</span><span class="sxs-lookup"><span data-stu-id="afb09-112">Parent elements</span></span>

[<span data-ttu-id="afb09-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="afb09-113">ItemShape</span></span>](itemshape.md)
  
## <a name="text-value"></a><span data-ttu-id="afb09-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="afb09-114">Text value</span></span>

<span data-ttu-id="afb09-115">**UniqueBodyType**要素のテキスト値に固有の本文の形式が返されることを示します。</span><span class="sxs-lookup"><span data-stu-id="afb09-115">The text value of the **UniqueBodyType** element indicates format the unique body is returned in.</span></span> <span data-ttu-id="afb09-116">次の表は、この要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="afb09-116">The following table lists the possible values for this element.</span></span> 
  
****

|<span data-ttu-id="afb09-117">**値**</span><span class="sxs-lookup"><span data-stu-id="afb09-117">**Value**</span></span>|<span data-ttu-id="afb09-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="afb09-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="afb09-119">ベスト</span><span class="sxs-lookup"><span data-stu-id="afb09-119">Best</span></span>  <br/> |<span data-ttu-id="afb09-120">応答には、本文テキストの豊富な利用可能なコンテンツが返されます。</span><span class="sxs-lookup"><span data-stu-id="afb09-120">The response will return the richest available content of body text.</span></span> <span data-ttu-id="afb09-121">これは、コンテンツは、テキストまたは html 形式かどうか不明ではない場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="afb09-121">This is useful if it is unknown whether the content is text or HTML.</span></span>  <br/> <span data-ttu-id="afb09-122">ストアド本文がテキスト形式の場合は、返された本文をテキストになります。</span><span class="sxs-lookup"><span data-stu-id="afb09-122">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="afb09-123">それ以外の場合、応答であっても、ストアドの本文が HTML または rtf 形式のいずれかの形式では場合、HTML が返されます。</span><span class="sxs-lookup"><span data-stu-id="afb09-123">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span>  <br/> <span data-ttu-id="afb09-124">既定値です。</span><span class="sxs-lookup"><span data-stu-id="afb09-124">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="afb09-125">HTML</span><span class="sxs-lookup"><span data-stu-id="afb09-125">HTML</span></span>  <br/> |<span data-ttu-id="afb09-126">応答は html 形式で一意の本文を返します。</span><span class="sxs-lookup"><span data-stu-id="afb09-126">The response will return a unique body as HTML.</span></span>  <br/> |
|<span data-ttu-id="afb09-127">テキスト型 (Text)</span><span class="sxs-lookup"><span data-stu-id="afb09-127">Text</span></span>  <br/> |<span data-ttu-id="afb09-128">応答では、プレーン テキストとして独自の本文を返します。</span><span class="sxs-lookup"><span data-stu-id="afb09-128">The response will return a unique body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="afb09-129">備考</span><span class="sxs-lookup"><span data-stu-id="afb09-129">Remarks</span></span>

<span data-ttu-id="afb09-130">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="afb09-130">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="afb09-131">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="afb09-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afb09-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="afb09-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afb09-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="afb09-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afb09-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afb09-134">Schema Name</span></span>  <br/> |<span data-ttu-id="afb09-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="afb09-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="afb09-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afb09-136">Validation File</span></span>  <br/> |<span data-ttu-id="afb09-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="afb09-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afb09-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="afb09-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="afb09-139">True</span><span class="sxs-lookup"><span data-stu-id="afb09-139">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afb09-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="afb09-140">See also</span></span>



[<span data-ttu-id="afb09-141">ItemShape</span><span class="sxs-lookup"><span data-stu-id="afb09-141">ItemShape</span></span>](itemshape.md)


- [<span data-ttu-id="afb09-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="afb09-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

