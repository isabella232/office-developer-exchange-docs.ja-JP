---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: ConvertHtmlCodePageToUTF8 要素は、項目の HTML 本文が UTF8 に変換されるかどうかを示します。
ms.openlocfilehash: aff6579835097a273101188c02a9919003b71b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759773"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="9d0b0-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="9d0b0-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="9d0b0-104">**ConvertHtmlCodePageToUTF8**要素は、項目の HTML 本文が UTF8 に変換されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="9d0b0-105">**xs:boolean**</span><span class="sxs-lookup"><span data-stu-id="9d0b0-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d0b0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d0b0-106">Attributes and elements</span></span>

<span data-ttu-id="9d0b0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d0b0-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d0b0-108">Attributes</span></span>

<span data-ttu-id="9d0b0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d0b0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d0b0-110">Child elements</span></span>

<span data-ttu-id="9d0b0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d0b0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d0b0-112">Parent elements</span></span>

|<span data-ttu-id="9d0b0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d0b0-113">**Element**</span></span>|<span data-ttu-id="9d0b0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d0b0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d0b0-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="9d0b0-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="9d0b0-116">応答で返されるプロパティのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d0b0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d0b0-117">Text value</span></span>

<span data-ttu-id="9d0b0-118">の**場合は true** 、 **ConvertHtmlCodePageToUTF8**要素のテキスト値は、HTML 本文が UTF8 に変換することを示します。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="9d0b0-119">テキスト値が**false**のでは、HTML 本文が UTF8 に変換されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d0b0-120">備考</span><span class="sxs-lookup"><span data-stu-id="9d0b0-120">Remarks</span></span>

<span data-ttu-id="9d0b0-121">要求に**ConvertHtmlCodePageToUTF8**要素が指定されていない場合、既定値の**true**が使用されます。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="9d0b0-122">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9d0b0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d0b0-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d0b0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d0b0-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d0b0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d0b0-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d0b0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9d0b0-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d0b0-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d0b0-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d0b0-127">Validation File</span></span>  <br/> |<span data-ttu-id="9d0b0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d0b0-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d0b0-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d0b0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d0b0-130">False</span><span class="sxs-lookup"><span data-stu-id="9d0b0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d0b0-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d0b0-131">See also</span></span>



- [<span data-ttu-id="9d0b0-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d0b0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

