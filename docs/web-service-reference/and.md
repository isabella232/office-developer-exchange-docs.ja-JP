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
description: 要素は、2 つまたは複数の検索式間で論理 AND 演算を実行できるようにする検索式を表します。 AND 演算の結果では、要素内に含まれるすべての検索式に該当する場合は true です。
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759323"
---
# <a name="and"></a><span data-ttu-id="64fb0-104">And</span><span class="sxs-lookup"><span data-stu-id="64fb0-104">And</span></span>

<span data-ttu-id="64fb0-105">**および**要素は、2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="64fb0-106">****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="64fb0-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="64fb0-107">**実際**</span><span class="sxs-lookup"><span data-stu-id="64fb0-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64fb0-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="64fb0-108">Attributes and elements</span></span>

<span data-ttu-id="64fb0-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64fb0-110">属性</span><span class="sxs-lookup"><span data-stu-id="64fb0-110">Attributes</span></span>

<span data-ttu-id="64fb0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="64fb0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64fb0-112">子要素</span><span class="sxs-lookup"><span data-stu-id="64fb0-112">Child elements</span></span>

|<span data-ttu-id="64fb0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="64fb0-113">**Element**</span></span>|<span data-ttu-id="64fb0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="64fb0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64fb0-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="64fb0-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="64fb0-116">制限内での式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="64fb0-117">And 演算では、2 つまたは複数の検索式を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="64fb0-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="64fb0-118">次の要素の 1 つは、 **SearchExpression**要素に置き換えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="64fb0-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="64fb0-119">存在します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="64fb0-120">除外</span><span class="sxs-lookup"><span data-stu-id="64fb0-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="64fb0-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="64fb0-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="64fb0-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="64fb0-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="64fb0-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="64fb0-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="64fb0-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="64fb0-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="64fb0-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="64fb0-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="64fb0-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="64fb0-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="64fb0-127">内容</span><span class="sxs-lookup"><span data-stu-id="64fb0-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="64fb0-128">Not</span><span class="sxs-lookup"><span data-stu-id="64fb0-128">Not</span></span>](not.md)</li><li><span data-ttu-id="64fb0-129">**And**</span><span class="sxs-lookup"><span data-stu-id="64fb0-129">**And**</span></span></li><li>[<span data-ttu-id="64fb0-130">Or</span><span class="sxs-lookup"><span data-stu-id="64fb0-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="64fb0-131">親要素</span><span class="sxs-lookup"><span data-stu-id="64fb0-131">Parent elements</span></span>

|<span data-ttu-id="64fb0-132">**要素**</span><span class="sxs-lookup"><span data-stu-id="64fb0-132">**Element**</span></span>|<span data-ttu-id="64fb0-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="64fb0-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64fb0-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="64fb0-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="64fb0-135">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="64fb0-136">Not</span><span class="sxs-lookup"><span data-stu-id="64fb0-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="64fb0-137">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="64fb0-138">**And**</span><span class="sxs-lookup"><span data-stu-id="64fb0-138">**And**</span></span> <br/> |<span data-ttu-id="64fb0-139">2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="64fb0-140">****および**要素内に含まれている検索式のすべてに**該当**する場合は、 **AND**演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="64fb0-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="64fb0-141">Or</span><span class="sxs-lookup"><span data-stu-id="64fb0-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="64fb0-142">含まれている検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="64fb0-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="64fb0-143">**または** **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="64fb0-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="64fb0-144">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="64fb0-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64fb0-145">備考</span><span class="sxs-lookup"><span data-stu-id="64fb0-145">Remarks</span></span>

<span data-ttu-id="64fb0-146">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="64fb0-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64fb0-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="64fb0-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64fb0-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="64fb0-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64fb0-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="64fb0-149">Schema Name</span></span>  <br/> |<span data-ttu-id="64fb0-150">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="64fb0-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="64fb0-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="64fb0-151">Validation File</span></span>  <br/> |<span data-ttu-id="64fb0-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64fb0-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64fb0-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="64fb0-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="64fb0-154">False</span><span class="sxs-lookup"><span data-stu-id="64fb0-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64fb0-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="64fb0-155">See also</span></span>

- [<span data-ttu-id="64fb0-156">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="64fb0-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

