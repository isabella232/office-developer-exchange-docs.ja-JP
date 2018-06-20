---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: FieldURIOrConstant 要素は、プロパティ、または別のプロパティを比較するときに使用する定数値を表します。
ms.openlocfilehash: 5195feec2a314d9ec15dc4a25a7a014aded1696a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760477"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="c064e-103">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="c064e-103">FieldURIOrConstant</span></span>

<span data-ttu-id="c064e-104">**FieldURIOrConstant**要素は、プロパティ、または別のプロパティを比較するときに使用する定数値を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

 <span data-ttu-id="c064e-105">**FieldURIOrConstantType**</span><span class="sxs-lookup"><span data-stu-id="c064e-105">**FieldURIOrConstantType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c064e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c064e-106">Attributes and elements</span></span>

<span data-ttu-id="c064e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c064e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c064e-108">属性</span><span class="sxs-lookup"><span data-stu-id="c064e-108">Attributes</span></span>

<span data-ttu-id="c064e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c064e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c064e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c064e-110">Child elements</span></span>

|<span data-ttu-id="c064e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="c064e-111">**Element**</span></span>|<span data-ttu-id="c064e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c064e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c064e-113">定数</span><span class="sxs-lookup"><span data-stu-id="c064e-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="c064e-114">制限における定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="c064e-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="c064e-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c064e-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c064e-116">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c064e-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c064e-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c064e-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c064e-118">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c064e-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c064e-119">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c064e-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c064e-120">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="c064e-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c064e-121">親要素</span><span class="sxs-lookup"><span data-stu-id="c064e-121">Parent elements</span></span>

|<span data-ttu-id="c064e-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="c064e-122">**Element**</span></span>|<span data-ttu-id="c064e-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="c064e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c064e-124">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="c064e-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="c064e-125">プロパティを定数値または別のプロパティを比較し、両者が等しい場合に true に評価する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="c064e-126">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="c064e-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="c064e-127">定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティ値が大きい場合に true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="c064e-128">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="c064e-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="c064e-129">プロパティに定数値または別のプロパティを比較し、true を指定すると、最初のプロパティは、以上の 2 番目の値またはプロパティに値を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="c064e-130">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="c064e-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="c064e-131">定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティは、2 番目の値やプロパティよりも小さい場合は true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="c064e-132">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="c064e-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="c064e-133">定数値を持つプロパティ、または別のプロパティを比較し、最初のプロパティは、2 番目の値またはプロパティに等しいかそれより小さい場合は true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="c064e-134">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="c064e-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="c064e-135">定数値を持つプロパティ、または別のプロパティを比較し、値が同じではない場合は true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="c064e-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c064e-136">備考</span><span class="sxs-lookup"><span data-stu-id="c064e-136">Remarks</span></span>

<span data-ttu-id="c064e-137">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c064e-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="c064e-138">例</span><span class="sxs-lookup"><span data-stu-id="c064e-138">Example</span></span>

<span data-ttu-id="c064e-139">次の XML の例では、定数と URI のフィールドの両方で使用する FieldURIOrConstant 要素を示します。</span><span class="sxs-lookup"><span data-stu-id="c064e-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```
[xml]
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a><span data-ttu-id="c064e-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="c064e-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c064e-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="c064e-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c064e-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c064e-142">Schema Name</span></span>  <br/> |<span data-ttu-id="c064e-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c064e-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="c064e-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c064e-144">Validation File</span></span>  <br/> |<span data-ttu-id="c064e-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c064e-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c064e-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c064e-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="c064e-147">False</span><span class="sxs-lookup"><span data-stu-id="c064e-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c064e-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="c064e-148">See also</span></span>



- [<span data-ttu-id="c064e-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c064e-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

