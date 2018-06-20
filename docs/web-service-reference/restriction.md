---
title: 制限
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: 制限要素は、制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。
ms.openlocfilehash: 6b5702696db29910ae476a370bf362fe6a036ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833213"
---
# <a name="restriction"></a><span data-ttu-id="3444f-103">制限</span><span class="sxs-lookup"><span data-stu-id="3444f-103">Restriction</span></span>

<span data-ttu-id="3444f-104">**制限**要素は、制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="3444f-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="3444f-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3444f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3444f-106">Attributes and elements</span></span>

<span data-ttu-id="3444f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3444f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3444f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3444f-108">Attributes</span></span>

<span data-ttu-id="3444f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3444f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3444f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3444f-110">Child elements</span></span>

|<span data-ttu-id="3444f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3444f-111">**Element**</span></span>|<span data-ttu-id="3444f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3444f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3444f-113">And</span><span class="sxs-lookup"><span data-stu-id="3444f-113">And</span></span>](and.md) <br/> |<span data-ttu-id="3444f-114">使用すると、2 つまたは複数の検索式間でブール型の**AND**操作を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="3444f-115">内容</span><span class="sxs-lookup"><span data-stu-id="3444f-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="3444f-116">指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="3444f-117">除外</span><span class="sxs-lookup"><span data-stu-id="3444f-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="3444f-118">プロパティのビットごとのマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="3444f-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="3444f-119">存在します。</span><span class="sxs-lookup"><span data-stu-id="3444f-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="3444f-120">**True**を返す指定されたプロパティが存在する場合、アイテムの検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="3444f-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="3444f-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="3444f-122">プロパティを定数値または別のプロパティを比較し、これらが等しい場合**は true**に評価する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="3444f-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="3444f-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="3444f-124">最初のプロパティの値やプロパティよりも大きい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="3444f-125">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="3444f-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="3444f-126">最初のプロパティは、以上の値またはプロパティに値がある場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="3444f-127">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="3444f-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="3444f-128">最初のプロパティの値やプロパティよりも小さい場合、プロパティ、定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="3444f-129">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="3444f-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="3444f-130">最初のプロパティの値またはプロパティに等しいかそれより小さい場合は、プロパティ、定数値または別プロパティは、返す**場合は true**を比較するための検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="3444f-131">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="3444f-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="3444f-132">値が同じではない場合、プロパティを定数値または別プロパティは、返す**場合は true**を比較する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="3444f-133">Not</span><span class="sxs-lookup"><span data-stu-id="3444f-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="3444f-134">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="3444f-135">Or</span><span class="sxs-lookup"><span data-stu-id="3444f-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="3444f-136">含まれている検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="3444f-137">その子のいずれかの**場合は true**を返す場合、要素**または**要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="3444f-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="3444f-138">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="3444f-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="3444f-139">制限内の代替要素を表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="3444f-140">XML インスタンス ドキュメントでは、この要素は使用されません。</span><span class="sxs-lookup"><span data-stu-id="3444f-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3444f-141">親要素</span><span class="sxs-lookup"><span data-stu-id="3444f-141">Parent elements</span></span>

|<span data-ttu-id="3444f-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="3444f-142">**Element**</span></span>|<span data-ttu-id="3444f-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="3444f-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3444f-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="3444f-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="3444f-145">メールボックス内のフォルダーを識別するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3444f-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3444f-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="3444f-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="3444f-147">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3444f-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3444f-148">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="3444f-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="3444f-149">検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="3444f-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3444f-150">備考</span><span class="sxs-lookup"><span data-stu-id="3444f-150">Remarks</span></span>

<span data-ttu-id="3444f-151">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3444f-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3444f-152">要素情報</span><span class="sxs-lookup"><span data-stu-id="3444f-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3444f-153">名前空間</span><span class="sxs-lookup"><span data-stu-id="3444f-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3444f-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3444f-154">Schema Name</span></span>  <br/> |<span data-ttu-id="3444f-155">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3444f-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="3444f-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3444f-156">Validation File</span></span>  <br/> |<span data-ttu-id="3444f-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3444f-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3444f-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3444f-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="3444f-159">False</span><span class="sxs-lookup"><span data-stu-id="3444f-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3444f-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="3444f-160">See also</span></span>



- [<span data-ttu-id="3444f-161">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3444f-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

