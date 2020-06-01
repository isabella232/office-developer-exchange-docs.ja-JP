---
title: 値
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: Value 要素には、拡張プロパティの値が含まれています。
ms.openlocfilehash: 5de1528dda6d58ea772d050e709c0720e389fae6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465213"
---
# <a name="value"></a><span data-ttu-id="a84a7-103">値</span><span class="sxs-lookup"><span data-stu-id="a84a7-103">Value</span></span>

<span data-ttu-id="a84a7-104">**Value**要素には、拡張プロパティの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a84a7-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="a84a7-105">**String**</span><span class="sxs-lookup"><span data-stu-id="a84a7-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a84a7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a84a7-106">Attributes and elements</span></span>

<span data-ttu-id="a84a7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a84a7-108">属性</span><span class="sxs-lookup"><span data-stu-id="a84a7-108">Attributes</span></span>

<span data-ttu-id="a84a7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a84a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a84a7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a84a7-110">Child elements</span></span>

<span data-ttu-id="a84a7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a84a7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a84a7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a84a7-112">Parent elements</span></span>

|<span data-ttu-id="a84a7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a84a7-113">**Element**</span></span>|<span data-ttu-id="a84a7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a84a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a84a7-115">値</span><span class="sxs-lookup"><span data-stu-id="a84a7-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="a84a7-116">拡張プロパティの値のコレクションを格納します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="a84a7-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a84a7-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="a84a7-118">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a84a7-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a84a7-119">Text value</span></span>

<span data-ttu-id="a84a7-120">テキスト値は、ExtendedFieldURI の Recordtype 属性によって示される型と互換性がある必要があります。</span><span class="sxs-lookup"><span data-stu-id="a84a7-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a84a7-121">注釈</span><span class="sxs-lookup"><span data-stu-id="a84a7-121">Remarks</span></span>

<span data-ttu-id="a84a7-122">**Value**要素は、単一および複数値の拡張プロパティインスタンスの両方で発生します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="a84a7-123">単一値インスタンスの場合、これは[Extendedproperty](extendedproperty.md)要素の直接の子として存在します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="a84a7-124">複数値インスタンスの場合、これは**Values**コレクションの直接の子として存在します。</span><span class="sxs-lookup"><span data-stu-id="a84a7-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="a84a7-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a84a7-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a84a7-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a84a7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a84a7-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="a84a7-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a84a7-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a84a7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a84a7-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a84a7-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="a84a7-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a84a7-130">Validation File</span></span>  <br/> |<span data-ttu-id="a84a7-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a84a7-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a84a7-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a84a7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a84a7-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="a84a7-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a84a7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="a84a7-134">See also</span></span>

- [<span data-ttu-id="a84a7-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a84a7-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

