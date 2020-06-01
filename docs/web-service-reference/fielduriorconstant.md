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
description: FieldURIOrConstant 要素は、別のプロパティと比較するときに使用するプロパティまたは定数値のいずれかを表します。
ms.openlocfilehash: 8b5cb888a3bd2026b15e38fc8c005ab5ef5a2b11
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461227"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="6be84-103">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="6be84-103">FieldURIOrConstant</span></span>

<span data-ttu-id="6be84-104">**FieldURIOrConstant**要素は、別のプロパティと比較するときに使用するプロパティまたは定数値のいずれかを表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

<span data-ttu-id="6be84-105">**FieldURIOrConstantType**</span><span class="sxs-lookup"><span data-stu-id="6be84-105">**FieldURIOrConstantType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6be84-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6be84-106">Attributes and elements</span></span>

<span data-ttu-id="6be84-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6be84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6be84-108">属性</span><span class="sxs-lookup"><span data-stu-id="6be84-108">Attributes</span></span>

<span data-ttu-id="6be84-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6be84-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6be84-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6be84-110">Child elements</span></span>

|<span data-ttu-id="6be84-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6be84-111">**Element**</span></span>|<span data-ttu-id="6be84-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6be84-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be84-113">定数</span><span class="sxs-lookup"><span data-stu-id="6be84-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="6be84-114">制限で定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="6be84-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="6be84-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="6be84-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="6be84-116">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6be84-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="6be84-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="6be84-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="6be84-118">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="6be84-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="6be84-119">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="6be84-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="6be84-120">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6be84-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6be84-121">親要素</span><span class="sxs-lookup"><span data-stu-id="6be84-121">Parent elements</span></span>

|<span data-ttu-id="6be84-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="6be84-122">**Element**</span></span>|<span data-ttu-id="6be84-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="6be84-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6be84-124">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="6be84-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="6be84-125">プロパティを定数値または別のプロパティと比較し、等しい場合は true に評価される検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="6be84-126">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="6be84-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="6be84-127">プロパティを定数値または別のプロパティと比較し、最初のプロパティが大きくなる場合は true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="6be84-128">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="6be84-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="6be84-129">プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目の値またはプロパティよりも大きいか等しい場合に true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="6be84-130">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="6be84-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="6be84-131">プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目の値またはプロパティより小さい場合に true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="6be84-132">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="6be84-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="6be84-133">プロパティを定数値または別のプロパティと比較し、最初のプロパティが2番目の値またはプロパティ以下の場合に true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="6be84-134">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="6be84-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="6be84-135">プロパティを定数値または別のプロパティと比較し、値が同じでない場合は true を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="6be84-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6be84-136">注釈</span><span class="sxs-lookup"><span data-stu-id="6be84-136">Remarks</span></span>

<span data-ttu-id="6be84-137">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6be84-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6be84-138">例</span><span class="sxs-lookup"><span data-stu-id="6be84-138">Example</span></span>

<span data-ttu-id="6be84-139">次の XML の例は、定数とフィールド URI の両方で使用される FieldURIOrConstant 要素を示しています。</span><span class="sxs-lookup"><span data-stu-id="6be84-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```xml
<Restriction>
  <Or xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="6be84-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6be84-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6be84-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="6be84-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6be84-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6be84-142">Schema Name</span></span>  <br/> |<span data-ttu-id="6be84-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6be84-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="6be84-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6be84-144">Validation File</span></span>  <br/> |<span data-ttu-id="6be84-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6be84-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6be84-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6be84-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="6be84-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="6be84-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6be84-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="6be84-148">See also</span></span>

- [<span data-ttu-id="6be84-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6be84-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

