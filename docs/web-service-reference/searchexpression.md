---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: SearchExpression 要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 XML インスタンス ドキュメントでは、この要素は使用されません。
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833286"
---
# <a name="searchexpression"></a><span data-ttu-id="7e9cb-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="7e9cb-105">SearchExpression</span></span>

<span data-ttu-id="7e9cb-106">**SearchExpression**要素は、制限内の代替要素を表す抽象要素です。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="7e9cb-107">すべての検索式は、この基本型から派生します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="7e9cb-108">XML インスタンス ドキュメントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="7e9cb-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="7e9cb-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e9cb-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e9cb-110">Attributes and elements</span></span>

<span data-ttu-id="7e9cb-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e9cb-112">属性</span><span class="sxs-lookup"><span data-stu-id="7e9cb-112">Attributes</span></span>

<span data-ttu-id="7e9cb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e9cb-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7e9cb-114">Child elements</span></span>

<span data-ttu-id="7e9cb-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e9cb-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7e9cb-116">Parent elements</span></span>

|<span data-ttu-id="7e9cb-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e9cb-117">**Element**</span></span>|<span data-ttu-id="7e9cb-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e9cb-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e9cb-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="7e9cb-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="7e9cb-120">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="7e9cb-121">Not</span><span class="sxs-lookup"><span data-stu-id="7e9cb-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="7e9cb-122">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="7e9cb-123">And</span><span class="sxs-lookup"><span data-stu-id="7e9cb-123">And</span></span>](and.md) <br/> |<span data-ttu-id="7e9cb-124">2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="7e9cb-125">****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="7e9cb-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="7e9cb-126">Or</span><span class="sxs-lookup"><span data-stu-id="7e9cb-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="7e9cb-127">含まれている検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="7e9cb-128">**または** **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="7e9cb-129">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e9cb-130">備考</span><span class="sxs-lookup"><span data-stu-id="7e9cb-130">Remarks</span></span>

<span data-ttu-id="7e9cb-131">SearchExpression 代替グループの一部である任意のフィルター要素は、SearchExpression 要素の代わりに表示できます。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7e9cb-132">この要素は、インスタンス ドキュメント内で直接は発生しません。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="7e9cb-133">次の要素は、SearchExpression 代替グループのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="7e9cb-134">存在します。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="7e9cb-135">除外</span><span class="sxs-lookup"><span data-stu-id="7e9cb-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="7e9cb-136">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="7e9cb-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="7e9cb-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="7e9cb-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="7e9cb-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="7e9cb-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="7e9cb-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="7e9cb-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="7e9cb-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="7e9cb-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="7e9cb-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="7e9cb-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="7e9cb-142">内容</span><span class="sxs-lookup"><span data-stu-id="7e9cb-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="7e9cb-143">Not</span><span class="sxs-lookup"><span data-stu-id="7e9cb-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="7e9cb-144">And</span><span class="sxs-lookup"><span data-stu-id="7e9cb-144">And</span></span>](and.md)
    
- [<span data-ttu-id="7e9cb-145">Or</span><span class="sxs-lookup"><span data-stu-id="7e9cb-145">Or</span></span>](or.md)
    
<span data-ttu-id="7e9cb-146">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7e9cb-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e9cb-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e9cb-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e9cb-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e9cb-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e9cb-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e9cb-149">Schema Name</span></span>  <br/> |<span data-ttu-id="7e9cb-150">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e9cb-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e9cb-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e9cb-151">Validation File</span></span>  <br/> |<span data-ttu-id="7e9cb-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e9cb-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e9cb-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e9cb-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e9cb-154">False</span><span class="sxs-lookup"><span data-stu-id="7e9cb-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e9cb-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e9cb-155">See also</span></span>



- [<span data-ttu-id="7e9cb-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e9cb-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

