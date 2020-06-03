---
title: 未サポート
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
description: Not 要素は、それに含まれる検索式の Boolean 値を否定する検索式を表します。
ms.openlocfilehash: 84c64a6d9d39f260d416fc32e4e5f5fcdef027e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466718"
---
# <a name="not"></a><span data-ttu-id="86b5c-103">未サポート</span><span class="sxs-lookup"><span data-stu-id="86b5c-103">Not</span></span>

<span data-ttu-id="86b5c-104">**Not**要素は、それに含まれる検索式の Boolean 値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="86b5c-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="86b5c-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86b5c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="86b5c-106">Attributes and elements</span></span>

<span data-ttu-id="86b5c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86b5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="86b5c-108">Attributes</span></span>

<span data-ttu-id="86b5c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="86b5c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86b5c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="86b5c-110">Child elements</span></span>

|<span data-ttu-id="86b5c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="86b5c-111">**Element**</span></span>|<span data-ttu-id="86b5c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="86b5c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86b5c-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="86b5c-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="86b5c-114">制限内の式の基本クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="86b5c-115">**Searchexpression**要素には、次のいずれかの要素を置き換える必要があります。</span><span class="sxs-lookup"><span data-stu-id="86b5c-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="86b5c-116">- [ある](exists.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="86b5c-117">- [除外](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="86b5c-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="86b5c-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="86b5c-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="86b5c-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="86b5c-122">- [Isna](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="86b5c-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="86b5c-124">- [含み](contains.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="86b5c-125">- **じゃない**</span><span class="sxs-lookup"><span data-stu-id="86b5c-125">- **Not**</span></span> <br/><span data-ttu-id="86b5c-126">- [そして](and.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-126">- [And](and.md)</span></span> <br/><span data-ttu-id="86b5c-127">- [や](or.md)</span><span class="sxs-lookup"><span data-stu-id="86b5c-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86b5c-128">親要素</span><span class="sxs-lookup"><span data-stu-id="86b5c-128">Parent elements</span></span>

|<span data-ttu-id="86b5c-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="86b5c-129">**Element**</span></span>|<span data-ttu-id="86b5c-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="86b5c-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86b5c-131">制限</span><span class="sxs-lookup"><span data-stu-id="86b5c-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="86b5c-132">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="86b5c-133">**Not**</span><span class="sxs-lookup"><span data-stu-id="86b5c-133">**Not**</span></span> <br/> |<span data-ttu-id="86b5c-134">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="86b5c-135">And</span><span class="sxs-lookup"><span data-stu-id="86b5c-135">And</span></span>](and.md) <br/> |<span data-ttu-id="86b5c-136">2つ以上の検索式の間でブール値**と**演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="86b5c-137">And 操作の結果は、 **and**要素に含まれるすべての検索式が**true**である場合に**true** **となり**ます。</span><span class="sxs-lookup"><span data-stu-id="86b5c-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="86b5c-138">Or</span><span class="sxs-lookup"><span data-stu-id="86b5c-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="86b5c-139">含まれる検索式に対して論理**OR**演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="86b5c-140">**または**、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="86b5c-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="86b5c-141">**または、** 2 つ以上の子を持つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="86b5c-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86b5c-142">注釈</span><span class="sxs-lookup"><span data-stu-id="86b5c-142">Remarks</span></span>

<span data-ttu-id="86b5c-143">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="86b5c-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86b5c-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="86b5c-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86b5c-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="86b5c-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86b5c-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86b5c-146">Schema Name</span></span>  <br/> |<span data-ttu-id="86b5c-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="86b5c-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="86b5c-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86b5c-148">Validation File</span></span>  <br/> |<span data-ttu-id="86b5c-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="86b5c-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86b5c-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="86b5c-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="86b5c-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="86b5c-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86b5c-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="86b5c-152">See also</span></span>

- [<span data-ttu-id="86b5c-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="86b5c-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

