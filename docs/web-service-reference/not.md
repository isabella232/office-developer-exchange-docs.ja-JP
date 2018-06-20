---
title: Not
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: ない要素が含まれている検索式のブール値を否定する検索式を表します。
ms.openlocfilehash: f5bc709d8b1e77a13b3598905651ac1750436f03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832553"
---
# <a name="not"></a><span data-ttu-id="630d1-103">Not</span><span class="sxs-lookup"><span data-stu-id="630d1-103">Not</span></span>

<span data-ttu-id="630d1-104">**しない**要素が含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="630d1-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="630d1-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="630d1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="630d1-106">Attributes and elements</span></span>

<span data-ttu-id="630d1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="630d1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="630d1-108">属性</span><span class="sxs-lookup"><span data-stu-id="630d1-108">Attributes</span></span>

<span data-ttu-id="630d1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="630d1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="630d1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="630d1-110">Child elements</span></span>

|<span data-ttu-id="630d1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="630d1-111">**Element**</span></span>|<span data-ttu-id="630d1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="630d1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="630d1-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="630d1-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="630d1-114">制限内での式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="630d1-115">次の要素の 1 つは、 **SearchExpression**要素に置き換えられる必要があります。</span><span class="sxs-lookup"><span data-stu-id="630d1-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="630d1-116">- [存在します。](exists.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="630d1-117">- [除外](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="630d1-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="630d1-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="630d1-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="630d1-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="630d1-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="630d1-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="630d1-124">- [含まれています](contains.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="630d1-125">- **じゃない**</span><span class="sxs-lookup"><span data-stu-id="630d1-125">- **Not**</span></span> <br/><span data-ttu-id="630d1-126">- [そして](and.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-126">- [And](and.md)</span></span> <br/><span data-ttu-id="630d1-127">- [または](or.md)</span><span class="sxs-lookup"><span data-stu-id="630d1-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="630d1-128">親要素</span><span class="sxs-lookup"><span data-stu-id="630d1-128">Parent elements</span></span>

|<span data-ttu-id="630d1-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="630d1-129">**Element**</span></span>|<span data-ttu-id="630d1-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="630d1-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="630d1-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="630d1-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="630d1-132">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="630d1-133">**Not**</span><span class="sxs-lookup"><span data-stu-id="630d1-133">**Not**</span></span> <br/> |<span data-ttu-id="630d1-134">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="630d1-135">And</span><span class="sxs-lookup"><span data-stu-id="630d1-135">And</span></span>](and.md) <br/> |<span data-ttu-id="630d1-136">2 つまたは複数の検索式間でブール型の**AND**操作を実行できるようにする検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="630d1-137">****および**要素内に含まれるすべての検索式に**該当**する場合は、 **AND**演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="630d1-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="630d1-138">Or</span><span class="sxs-lookup"><span data-stu-id="630d1-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="630d1-139">含まれている検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="630d1-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="630d1-140">**または** **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="630d1-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="630d1-141">**または**2 つ以上の子が必要です。</span><span class="sxs-lookup"><span data-stu-id="630d1-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="630d1-142">備考</span><span class="sxs-lookup"><span data-stu-id="630d1-142">Remarks</span></span>

<span data-ttu-id="630d1-143">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="630d1-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="630d1-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="630d1-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="630d1-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="630d1-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="630d1-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="630d1-146">Schema Name</span></span>  <br/> |<span data-ttu-id="630d1-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="630d1-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="630d1-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="630d1-148">Validation File</span></span>  <br/> |<span data-ttu-id="630d1-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="630d1-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="630d1-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="630d1-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="630d1-151">False</span><span class="sxs-lookup"><span data-stu-id="630d1-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="630d1-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="630d1-152">See also</span></span>

- [<span data-ttu-id="630d1-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="630d1-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

