---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: And 要素は、2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。 And 操作の結果は、And 要素に含まれるすべての検索式が true である場合に true となります。
ms.openlocfilehash: f5239f19c2b5a931eefa9ff4a9dd8ed9d775bae2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464722"
---
# <a name="and"></a><span data-ttu-id="7bbe0-104">And</span><span class="sxs-lookup"><span data-stu-id="7bbe0-104">And</span></span>

<span data-ttu-id="7bbe0-105">**And**要素は、2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="7bbe0-106">And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="7bbe0-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bbe0-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7bbe0-108">Attributes and elements</span></span>

<span data-ttu-id="7bbe0-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bbe0-110">属性</span><span class="sxs-lookup"><span data-stu-id="7bbe0-110">Attributes</span></span>

<span data-ttu-id="7bbe0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bbe0-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7bbe0-112">Child elements</span></span>

|<span data-ttu-id="7bbe0-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-113">**Element**</span></span>|<span data-ttu-id="7bbe0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bbe0-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="7bbe0-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="7bbe0-116">制限内の式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="7bbe0-117">And 操作には、2つ以上の検索式を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="7bbe0-118">**Searchexpression**要素には、次のいずれかの要素を置き換える必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="7bbe0-119">Exists</span><span class="sxs-lookup"><span data-stu-id="7bbe0-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="7bbe0-120">Excludes</span><span class="sxs-lookup"><span data-stu-id="7bbe0-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="7bbe0-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="7bbe0-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="7bbe0-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="7bbe0-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="7bbe0-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="7bbe0-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="7bbe0-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="7bbe0-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="7bbe0-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="7bbe0-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="7bbe0-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="7bbe0-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="7bbe0-127">Contains</span><span class="sxs-lookup"><span data-stu-id="7bbe0-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="7bbe0-128">Not</span><span class="sxs-lookup"><span data-stu-id="7bbe0-128">Not</span></span>](not.md)</li><li><span data-ttu-id="7bbe0-129">**And**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-129">**And**</span></span></li><li>[<span data-ttu-id="7bbe0-130">Or</span><span class="sxs-lookup"><span data-stu-id="7bbe0-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="7bbe0-131">親要素</span><span class="sxs-lookup"><span data-stu-id="7bbe0-131">Parent elements</span></span>

|<span data-ttu-id="7bbe0-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-132">**Element**</span></span>|<span data-ttu-id="7bbe0-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bbe0-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="7bbe0-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="7bbe0-135">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="7bbe0-136">Not</span><span class="sxs-lookup"><span data-stu-id="7bbe0-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="7bbe0-137">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="7bbe0-138">**And**</span><span class="sxs-lookup"><span data-stu-id="7bbe0-138">**And**</span></span> <br/> |<span data-ttu-id="7bbe0-139">2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="7bbe0-140">And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="7bbe0-141">Or</span><span class="sxs-lookup"><span data-stu-id="7bbe0-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="7bbe0-142">含まれる検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="7bbe0-143">**または**、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="7bbe0-144">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7bbe0-145">注釈</span><span class="sxs-lookup"><span data-stu-id="7bbe0-145">Remarks</span></span>

<span data-ttu-id="7bbe0-146">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7bbe0-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bbe0-147">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7bbe0-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bbe0-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="7bbe0-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7bbe0-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7bbe0-149">Schema Name</span></span>  <br/> |<span data-ttu-id="7bbe0-150">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7bbe0-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="7bbe0-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7bbe0-151">Validation File</span></span>  <br/> |<span data-ttu-id="7bbe0-152">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7bbe0-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7bbe0-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7bbe0-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bbe0-154">正しくない</span><span class="sxs-lookup"><span data-stu-id="7bbe0-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bbe0-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="7bbe0-155">See also</span></span>

- [<span data-ttu-id="7bbe0-156">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7bbe0-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

