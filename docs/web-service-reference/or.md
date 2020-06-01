---
title: または
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
description: Or 要素は、それに含まれる検索式に対して論理 OR を実行する検索式を表します。 または、いずれかの子が true を返した場合は true を返します。 または、2つ以上の子を持つ必要があります。
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462480"
---
# <a name="or"></a><span data-ttu-id="425ef-105">または</span><span class="sxs-lookup"><span data-stu-id="425ef-105">Or</span></span>

<span data-ttu-id="425ef-106">**Or**要素は、それに含まれる検索式に対して論理**Or**を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="425ef-107">**または**、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="425ef-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="425ef-108">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="425ef-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="425ef-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="425ef-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="425ef-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="425ef-110">Attributes and elements</span></span>

<span data-ttu-id="425ef-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="425ef-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="425ef-112">属性</span><span class="sxs-lookup"><span data-stu-id="425ef-112">Attributes</span></span>

<span data-ttu-id="425ef-113">なし。</span><span class="sxs-lookup"><span data-stu-id="425ef-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="425ef-114">子要素</span><span class="sxs-lookup"><span data-stu-id="425ef-114">Child elements</span></span>

|<span data-ttu-id="425ef-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="425ef-115">**Element**</span></span>|<span data-ttu-id="425ef-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="425ef-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="425ef-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="425ef-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="425ef-118">制限内の式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="425ef-119">**Searchexpression**要素には、次のいずれかの要素を置き換える必要があります。</span><span class="sxs-lookup"><span data-stu-id="425ef-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="425ef-120">- [ある](exists.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="425ef-121">- [除外](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="425ef-122">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="425ef-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="425ef-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="425ef-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="425ef-126">- [Isna](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="425ef-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="425ef-128">- [含み](contains.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="425ef-129">- [じゃない](not.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="425ef-130">- [そして](and.md)</span><span class="sxs-lookup"><span data-stu-id="425ef-130">- [And](and.md)</span></span> <br/><span data-ttu-id="425ef-131">- **や**</span><span class="sxs-lookup"><span data-stu-id="425ef-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="425ef-132">親要素</span><span class="sxs-lookup"><span data-stu-id="425ef-132">Parent elements</span></span>

|<span data-ttu-id="425ef-133">**要素**</span><span class="sxs-lookup"><span data-stu-id="425ef-133">**Element**</span></span>|<span data-ttu-id="425ef-134">**説明**</span><span class="sxs-lookup"><span data-stu-id="425ef-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="425ef-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="425ef-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="425ef-136">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="425ef-137">Not</span><span class="sxs-lookup"><span data-stu-id="425ef-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="425ef-138">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="425ef-139">And</span><span class="sxs-lookup"><span data-stu-id="425ef-139">And</span></span>](and.md) <br/> |<span data-ttu-id="425ef-140">2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="425ef-141">And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。</span><span class="sxs-lookup"><span data-stu-id="425ef-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="425ef-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="425ef-142">**Or**</span></span> <br/> |<span data-ttu-id="425ef-143">含まれる検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="425ef-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="425ef-144">**または**、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="425ef-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="425ef-145">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="425ef-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="425ef-146">注釈</span><span class="sxs-lookup"><span data-stu-id="425ef-146">Remarks</span></span>

<span data-ttu-id="425ef-147">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="425ef-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="425ef-148">要素の情報</span><span class="sxs-lookup"><span data-stu-id="425ef-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="425ef-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="425ef-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="425ef-150">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="425ef-150">Schema Name</span></span>  <br/> |<span data-ttu-id="425ef-151">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="425ef-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="425ef-152">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="425ef-152">Validation File</span></span>  <br/> |<span data-ttu-id="425ef-153">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="425ef-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="425ef-154">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="425ef-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="425ef-155">正しくない</span><span class="sxs-lookup"><span data-stu-id="425ef-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="425ef-156">関連項目</span><span class="sxs-lookup"><span data-stu-id="425ef-156">See also</span></span>

- [<span data-ttu-id="425ef-157">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="425ef-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

