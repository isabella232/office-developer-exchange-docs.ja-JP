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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759773"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="d7199-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="d7199-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="d7199-104">**ConvertHtmlCodePageToUTF8**要素は、項目の HTML 本文が UTF8 に変換されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d7199-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="d7199-105">**xs:boolean**</span><span class="sxs-lookup"><span data-stu-id="d7199-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7199-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d7199-106">Attributes and elements</span></span>

<span data-ttu-id="d7199-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d7199-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7199-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7199-108">Attributes</span></span>

<span data-ttu-id="d7199-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d7199-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7199-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d7199-110">Child elements</span></span>

<span data-ttu-id="d7199-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d7199-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7199-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d7199-112">Parent elements</span></span>

|<span data-ttu-id="d7199-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d7199-113">**Element**</span></span>|<span data-ttu-id="d7199-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d7199-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7199-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d7199-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="d7199-116">応答で返されるプロパティのセットを識別します。</span><span class="sxs-lookup"><span data-stu-id="d7199-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7199-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d7199-117">Text value</span></span>

<span data-ttu-id="d7199-118">の**場合は true** 、 **ConvertHtmlCodePageToUTF8**要素のテキスト値は、HTML 本文が UTF8 に変換することを示します。</span><span class="sxs-lookup"><span data-stu-id="d7199-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="d7199-119">テキスト値が**false**のでは、HTML 本文が UTF8 に変換されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d7199-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d7199-120">備考</span><span class="sxs-lookup"><span data-stu-id="d7199-120">Remarks</span></span>

<span data-ttu-id="d7199-121">要求に**ConvertHtmlCodePageToUTF8**要素が指定されていない場合、既定値の**true**が使用されます。</span><span class="sxs-lookup"><span data-stu-id="d7199-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="d7199-122">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d7199-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7199-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="d7199-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7199-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="d7199-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7199-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d7199-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d7199-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d7199-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7199-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d7199-127">Validation File</span></span>  <br/> |<span data-ttu-id="d7199-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d7199-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7199-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d7199-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7199-130">False</span><span class="sxs-lookup"><span data-stu-id="d7199-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7199-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="d7199-131">See also</span></span>



- [<span data-ttu-id="d7199-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d7199-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

