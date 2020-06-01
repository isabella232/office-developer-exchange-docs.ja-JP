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
description: Restriction 要素は、FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。
ms.openlocfilehash: 6037ba15417d67d393ca70f3edf2248749c396e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465290"
---
# <a name="restriction"></a><span data-ttu-id="63451-103">制限</span><span class="sxs-lookup"><span data-stu-id="63451-103">Restriction</span></span>

<span data-ttu-id="63451-104">**Restriction**要素は、FindItem/findfolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="63451-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="63451-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="63451-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63451-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="63451-106">Attributes and elements</span></span>

<span data-ttu-id="63451-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="63451-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63451-108">属性</span><span class="sxs-lookup"><span data-stu-id="63451-108">Attributes</span></span>

<span data-ttu-id="63451-109">なし。</span><span class="sxs-lookup"><span data-stu-id="63451-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63451-110">子要素</span><span class="sxs-lookup"><span data-stu-id="63451-110">Child elements</span></span>

|<span data-ttu-id="63451-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="63451-111">**Element**</span></span>|<span data-ttu-id="63451-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="63451-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63451-113">And</span><span class="sxs-lookup"><span data-stu-id="63451-113">And</span></span>](and.md) <br/> |<span data-ttu-id="63451-114">2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="63451-115">Contains</span><span class="sxs-lookup"><span data-stu-id="63451-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="63451-116">指定したプロパティに指定した定数文字列値が含まれているかどうかを決定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="63451-117">Excludes</span><span class="sxs-lookup"><span data-stu-id="63451-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="63451-118">プロパティのビット単位のマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="63451-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="63451-119">Exists</span><span class="sxs-lookup"><span data-stu-id="63451-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="63451-120">指定されたプロパティがアイテムに存在する場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="63451-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="63451-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="63451-122">プロパティを定数値または別のプロパティと比較し、等しい場合は**true**に評価される検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="63451-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="63451-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="63451-124">プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティよりも大きい場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="63451-125">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="63451-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="63451-126">プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティよりも大きいか等しい場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="63451-127">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="63451-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="63451-128">プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティより小さい場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="63451-129">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="63451-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="63451-130">プロパティを定数値または別のプロパティと比較し、最初のプロパティが値またはプロパティ以下の場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="63451-131">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="63451-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="63451-132">プロパティを定数値または別のプロパティと比較し、値が同じでない場合は**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="63451-133">Not</span><span class="sxs-lookup"><span data-stu-id="63451-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="63451-134">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="63451-135">Or</span><span class="sxs-lookup"><span data-stu-id="63451-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="63451-136">含まれる検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="63451-137">**または**のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="63451-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="63451-138">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="63451-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="63451-139">制限内の代替要素を表します。</span><span class="sxs-lookup"><span data-stu-id="63451-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="63451-140">この要素は、XML インスタンスドキュメントでは使用されません。</span><span class="sxs-lookup"><span data-stu-id="63451-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63451-141">親要素</span><span class="sxs-lookup"><span data-stu-id="63451-141">Parent elements</span></span>

|<span data-ttu-id="63451-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="63451-142">**Element**</span></span>|<span data-ttu-id="63451-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="63451-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63451-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="63451-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="63451-145">メールボックス内のフォルダーを識別する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="63451-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="63451-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="63451-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="63451-147">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="63451-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="63451-148">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="63451-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="63451-149">検索フォルダーを定義するパラメーターを表します。</span><span class="sxs-lookup"><span data-stu-id="63451-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63451-150">注釈</span><span class="sxs-lookup"><span data-stu-id="63451-150">Remarks</span></span>

<span data-ttu-id="63451-151">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="63451-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63451-152">要素の情報</span><span class="sxs-lookup"><span data-stu-id="63451-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63451-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="63451-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63451-154">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="63451-154">Schema Name</span></span>  <br/> |<span data-ttu-id="63451-155">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="63451-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="63451-156">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="63451-156">Validation File</span></span>  <br/> |<span data-ttu-id="63451-157">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="63451-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63451-158">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="63451-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="63451-159">正しくない</span><span class="sxs-lookup"><span data-stu-id="63451-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63451-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="63451-160">See also</span></span>



- [<span data-ttu-id="63451-161">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="63451-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

