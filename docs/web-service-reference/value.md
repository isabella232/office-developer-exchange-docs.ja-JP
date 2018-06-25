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
description: 値の要素には、拡張プロパティの値が含まれています。
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839984"
---
# <a name="value"></a><span data-ttu-id="8a558-103">値</span><span class="sxs-lookup"><span data-stu-id="8a558-103">Value</span></span>

<span data-ttu-id="8a558-104">**値**の要素には、拡張プロパティの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a558-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="8a558-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="8a558-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8a558-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8a558-106">Attributes and elements</span></span>

<span data-ttu-id="8a558-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8a558-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a558-108">属性</span><span class="sxs-lookup"><span data-stu-id="8a558-108">Attributes</span></span>

<span data-ttu-id="8a558-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8a558-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a558-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8a558-110">Child elements</span></span>

<span data-ttu-id="8a558-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8a558-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a558-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8a558-112">Parent elements</span></span>

|<span data-ttu-id="8a558-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8a558-113">**Element**</span></span>|<span data-ttu-id="8a558-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8a558-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a558-115">Values</span><span class="sxs-lookup"><span data-stu-id="8a558-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="8a558-116">拡張プロパティの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8a558-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="8a558-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8a558-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="8a558-118">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="8a558-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8a558-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8a558-119">Text value</span></span>

<span data-ttu-id="8a558-120">テキスト値は、ExtendedFieldURI の登録するときの属性によって指定されている型との互換性である必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a558-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a558-121">備考</span><span class="sxs-lookup"><span data-stu-id="8a558-121">Remarks</span></span>

<span data-ttu-id="8a558-122">**値**要素は、両方の拡張プロパティの 1 つと複数値を持つインスタンスで発生します。</span><span class="sxs-lookup"><span data-stu-id="8a558-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="8a558-123">単一の値のインスタンスでは、 [ExtendedProperty](extendedproperty.md)要素の直接の子として存在します。</span><span class="sxs-lookup"><span data-stu-id="8a558-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="8a558-124">複数値を持つインスタンスの**値**のコレクションの直接の子として存在します。</span><span class="sxs-lookup"><span data-stu-id="8a558-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="8a558-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="8a558-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a558-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="8a558-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a558-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="8a558-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a558-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8a558-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8a558-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8a558-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a558-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8a558-130">Validation File</span></span>  <br/> |<span data-ttu-id="8a558-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a558-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a558-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8a558-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a558-133">False</span><span class="sxs-lookup"><span data-stu-id="8a558-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a558-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="8a558-134">See also</span></span>

- [<span data-ttu-id="8a558-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8a558-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

