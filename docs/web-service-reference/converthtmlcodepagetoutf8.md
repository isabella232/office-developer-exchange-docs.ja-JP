---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: ConvertHtmlCodePageToUTF8 要素は、アイテムの HTML 本文が UTF8 に変換されるかどうかを示します。
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457593"
---
# <a name="converthtmlcodepagetoutf8"></a><span data-ttu-id="29af4-103">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="29af4-103">ConvertHtmlCodePageToUTF8</span></span>

<span data-ttu-id="29af4-104">**ConvertHtmlCodePageToUTF8**要素は、アイテムの HTML 本文が UTF8 に変換されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29af4-104">The **ConvertHtmlCodePageToUTF8** element indicates whether the item HTML body is converted to UTF8.</span></span> 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 <span data-ttu-id="29af4-105">**xs: boolean**</span><span class="sxs-lookup"><span data-stu-id="29af4-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29af4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29af4-106">Attributes and elements</span></span>

<span data-ttu-id="29af4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29af4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29af4-108">属性</span><span class="sxs-lookup"><span data-stu-id="29af4-108">Attributes</span></span>

<span data-ttu-id="29af4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29af4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29af4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29af4-110">Child elements</span></span>

<span data-ttu-id="29af4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="29af4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29af4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="29af4-112">Parent elements</span></span>

|<span data-ttu-id="29af4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="29af4-113">**Element**</span></span>|<span data-ttu-id="29af4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="29af4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29af4-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="29af4-115">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="29af4-116">応答で返される一連のプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="29af4-116">Identifies a set of properties to return in a response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="29af4-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29af4-117">Text value</span></span>

<span data-ttu-id="29af4-118">**ConvertHtmlCodePageToUTF8**要素のテキスト値が**true**の場合は、HTML 本文が UTF8 に変換されることを示します。</span><span class="sxs-lookup"><span data-stu-id="29af4-118">A text value of **true** for the **ConvertHtmlCodePageToUTF8** element indicates that the HTML body is converted to UTF8.</span></span> <span data-ttu-id="29af4-119">テキスト値が**false**の場合は、HTML 本文が UTF8 に変換されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="29af4-119">A text value of **false** indicates that the HTML body is not converted to UTF8.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="29af4-120">注釈</span><span class="sxs-lookup"><span data-stu-id="29af4-120">Remarks</span></span>

<span data-ttu-id="29af4-121">**ConvertHtmlCodePageToUTF8**要素が要求で指定されていない場合は、既定値の**true**が使用されます。</span><span class="sxs-lookup"><span data-stu-id="29af4-121">The default value of **true** is used if the **ConvertHtmlCodePageToUTF8** element is not specified in a request.</span></span> 
  
<span data-ttu-id="29af4-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29af4-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29af4-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29af4-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29af4-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="29af4-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29af4-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29af4-125">Schema Name</span></span>  <br/> |<span data-ttu-id="29af4-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="29af4-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="29af4-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29af4-127">Validation File</span></span>  <br/> |<span data-ttu-id="29af4-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29af4-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29af4-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29af4-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="29af4-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="29af4-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29af4-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="29af4-131">See also</span></span>



- [<span data-ttu-id="29af4-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29af4-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

