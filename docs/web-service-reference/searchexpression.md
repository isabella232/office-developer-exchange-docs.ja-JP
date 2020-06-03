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
description: SearchExpression 要素は、制限内の代替要素を表す抽象要素です。 すべての検索式は、この基本型から派生します。 この要素は、XML インスタンスドキュメントでは使用されません。
ms.openlocfilehash: db06ce8e2faa0f2589963d58aab55073c618c171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530353"
---
# <a name="searchexpression"></a><span data-ttu-id="02a93-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="02a93-105">SearchExpression</span></span>

<span data-ttu-id="02a93-106">**Searchexpression**要素は、制限内の代替要素を表す抽象要素です。</span><span class="sxs-lookup"><span data-stu-id="02a93-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="02a93-107">すべての検索式は、この基本型から派生します。</span><span class="sxs-lookup"><span data-stu-id="02a93-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="02a93-108">この要素は、XML インスタンスドキュメントでは使用されません。</span><span class="sxs-lookup"><span data-stu-id="02a93-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="02a93-109">**Search式の種類**</span><span class="sxs-lookup"><span data-stu-id="02a93-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02a93-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="02a93-110">Attributes and elements</span></span>

<span data-ttu-id="02a93-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="02a93-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02a93-112">属性</span><span class="sxs-lookup"><span data-stu-id="02a93-112">Attributes</span></span>

<span data-ttu-id="02a93-113">なし。</span><span class="sxs-lookup"><span data-stu-id="02a93-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02a93-114">子要素</span><span class="sxs-lookup"><span data-stu-id="02a93-114">Child elements</span></span>

<span data-ttu-id="02a93-115">なし。</span><span class="sxs-lookup"><span data-stu-id="02a93-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02a93-116">親要素</span><span class="sxs-lookup"><span data-stu-id="02a93-116">Parent elements</span></span>

|<span data-ttu-id="02a93-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="02a93-117">**Element**</span></span>|<span data-ttu-id="02a93-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="02a93-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02a93-119">制限</span><span class="sxs-lookup"><span data-stu-id="02a93-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="02a93-120">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="02a93-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="02a93-121">Not</span><span class="sxs-lookup"><span data-stu-id="02a93-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="02a93-122">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="02a93-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="02a93-123">And</span><span class="sxs-lookup"><span data-stu-id="02a93-123">And</span></span>](and.md) <br/> |<span data-ttu-id="02a93-124">2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="02a93-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="02a93-125">And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。</span><span class="sxs-lookup"><span data-stu-id="02a93-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="02a93-126">Or</span><span class="sxs-lookup"><span data-stu-id="02a93-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="02a93-127">含まれる検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="02a93-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="02a93-128">**または**、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="02a93-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="02a93-129">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="02a93-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02a93-130">注釈</span><span class="sxs-lookup"><span data-stu-id="02a93-130">Remarks</span></span>

<span data-ttu-id="02a93-131">SearchExpression 置換グループの一部であるすべての filter 要素は、SearchExpression 要素の代わりに表示できます。</span><span class="sxs-lookup"><span data-stu-id="02a93-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="02a93-132">この要素は、インスタンスドキュメント内で直接発生することはありません。</span><span class="sxs-lookup"><span data-stu-id="02a93-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="02a93-133">次の要素は、SearchExpression 置換グループのメンバーです。</span><span class="sxs-lookup"><span data-stu-id="02a93-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="02a93-134">Exists</span><span class="sxs-lookup"><span data-stu-id="02a93-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="02a93-135">Excludes</span><span class="sxs-lookup"><span data-stu-id="02a93-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="02a93-136">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="02a93-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="02a93-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="02a93-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="02a93-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="02a93-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="02a93-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="02a93-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="02a93-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="02a93-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="02a93-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="02a93-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="02a93-142">内容</span><span class="sxs-lookup"><span data-stu-id="02a93-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="02a93-143">Not</span><span class="sxs-lookup"><span data-stu-id="02a93-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="02a93-144">And</span><span class="sxs-lookup"><span data-stu-id="02a93-144">And</span></span>](and.md)
    
- [<span data-ttu-id="02a93-145">Or</span><span class="sxs-lookup"><span data-stu-id="02a93-145">Or</span></span>](or.md)
    
<span data-ttu-id="02a93-146">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="02a93-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02a93-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="02a93-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02a93-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="02a93-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02a93-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="02a93-149">Schema Name</span></span>  <br/> |<span data-ttu-id="02a93-150">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="02a93-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="02a93-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="02a93-151">Validation File</span></span>  <br/> |<span data-ttu-id="02a93-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="02a93-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="02a93-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="02a93-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="02a93-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="02a93-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02a93-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="02a93-155">See also</span></span>



- [<span data-ttu-id="02a93-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="02a93-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

