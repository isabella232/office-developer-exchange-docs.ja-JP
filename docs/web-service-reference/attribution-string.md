---
title: 属性 (文字列)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 736be0bc-12c4-410e-bd17-a89f996ac432
description: 属性要素は、ペルソナの属性を識別するために使う文字列を指定します。
ms.openlocfilehash: 227379db8a77fb8cba7b4337e74d985bc5af65d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759463"
---
# <a name="attribution-string"></a><span data-ttu-id="9f376-103">属性 (文字列)</span><span class="sxs-lookup"><span data-stu-id="9f376-103">Attribution (string)</span></span>

<span data-ttu-id="9f376-104">**属性**要素は、ペルソナの属性を識別するために使う文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f376-104">The **Attribution** element specifies a string used to identify an attribute of a persona.</span></span> 
  
```XML
<Attribution></Attribution>
```

 <span data-ttu-id="9f376-105">**使用されています**</span><span class="sxs-lookup"><span data-stu-id="9f376-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f376-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9f376-106">Attributes and elements</span></span>

<span data-ttu-id="9f376-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f376-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f376-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f376-108">Attributes</span></span>

<span data-ttu-id="9f376-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f376-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f376-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f376-110">Child elements</span></span>

<span data-ttu-id="9f376-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9f376-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9f376-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9f376-112">Parent elements</span></span>

|<span data-ttu-id="9f376-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f376-113">**Element**</span></span>|<span data-ttu-id="9f376-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f376-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f376-115">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="9f376-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="9f376-116">帰属、関連付けられている**値**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f376-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9f376-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9f376-117">Text value</span></span>

<span data-ttu-id="9f376-118">**属性**要素のテキスト値は、属性のプロパティの値が元の連絡先にする文字列値です。</span><span class="sxs-lookup"><span data-stu-id="9f376-118">The text value of the **attribution** element is a string value that attributes a property value to the source contact.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9f376-119">備考</span><span class="sxs-lookup"><span data-stu-id="9f376-119">Remarks</span></span>

<span data-ttu-id="9f376-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9f376-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9f376-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9f376-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f376-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9f376-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f376-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9f376-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f376-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f376-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9f376-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="9f376-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9f376-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f376-126">Validation File</span></span>  <br/> |<span data-ttu-id="9f376-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f376-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f376-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9f376-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9f376-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f376-129">See also</span></span>

- [<span data-ttu-id="9f376-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f376-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

