---
title: Or
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: Or 要素が含まれている検索式に対して論理 OR を実行する検索式を表します。 またはその子のいずれかの場合は true を返す場合は true を返します。 または 2 つ以上の子を持つ必要があります。
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832661"
---
# <a name="or"></a><span data-ttu-id="f4e31-105">Or</span><span class="sxs-lookup"><span data-stu-id="f4e31-105">Or</span></span>

<span data-ttu-id="f4e31-106">要素**または**要素が含まれている検索式に対して、論理 **、または**を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="f4e31-107">**または** **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="f4e31-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="f4e31-108">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4e31-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="f4e31-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="f4e31-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4e31-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f4e31-110">Attributes and elements</span></span>

<span data-ttu-id="f4e31-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4e31-112">属性</span><span class="sxs-lookup"><span data-stu-id="f4e31-112">Attributes</span></span>

<span data-ttu-id="f4e31-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f4e31-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4e31-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f4e31-114">Child elements</span></span>

|<span data-ttu-id="f4e31-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4e31-115">**Element**</span></span>|<span data-ttu-id="f4e31-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4e31-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4e31-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="f4e31-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="f4e31-118">制限内での式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="f4e31-119">次の要素の 1 つは、 **SearchExpression**要素に置き換えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4e31-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="f4e31-120">- [存在します。](exists.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="f4e31-121">- [除外](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="f4e31-122">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="f4e31-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="f4e31-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="f4e31-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="f4e31-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="f4e31-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="f4e31-128">- [含まれています](contains.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="f4e31-129">- [じゃない](not.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="f4e31-130">- [そして](and.md)</span><span class="sxs-lookup"><span data-stu-id="f4e31-130">- [And](and.md)</span></span> <br/><span data-ttu-id="f4e31-131">- **または**</span><span class="sxs-lookup"><span data-stu-id="f4e31-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4e31-132">親要素</span><span class="sxs-lookup"><span data-stu-id="f4e31-132">Parent elements</span></span>

|<span data-ttu-id="f4e31-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="f4e31-133">**Element**</span></span>|<span data-ttu-id="f4e31-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="f4e31-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4e31-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="f4e31-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f4e31-136">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f4e31-137">Not</span><span class="sxs-lookup"><span data-stu-id="f4e31-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="f4e31-138">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f4e31-139">And</span><span class="sxs-lookup"><span data-stu-id="f4e31-139">And</span></span>](and.md) <br/> |<span data-ttu-id="f4e31-140">2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="f4e31-141">****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="f4e31-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="f4e31-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="f4e31-142">**Or**</span></span> <br/> |<span data-ttu-id="f4e31-143">含まれている検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="f4e31-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="f4e31-144">**または** **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="f4e31-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="f4e31-145">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4e31-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4e31-146">備考</span><span class="sxs-lookup"><span data-stu-id="f4e31-146">Remarks</span></span>

<span data-ttu-id="f4e31-147">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f4e31-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4e31-148">要素情報</span><span class="sxs-lookup"><span data-stu-id="f4e31-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4e31-149">名前空間</span><span class="sxs-lookup"><span data-stu-id="f4e31-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4e31-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f4e31-150">Schema Name</span></span>  <br/> |<span data-ttu-id="f4e31-151">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f4e31-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4e31-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f4e31-152">Validation File</span></span>  <br/> |<span data-ttu-id="f4e31-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f4e31-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4e31-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f4e31-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4e31-155">False</span><span class="sxs-lookup"><span data-stu-id="f4e31-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4e31-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="f4e31-156">See also</span></span>

- [<span data-ttu-id="f4e31-157">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f4e31-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

