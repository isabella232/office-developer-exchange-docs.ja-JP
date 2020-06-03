---
title: Excludes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: 除外要素は、指定されたプロパティと指定された値のビット単位のマスクを実行します。
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530615"
---
# <a name="excludes"></a><span data-ttu-id="73fd9-103">Excludes</span><span class="sxs-lookup"><span data-stu-id="73fd9-103">Excludes</span></span>

<span data-ttu-id="73fd9-104">**除外**要素は、指定されたプロパティと指定された値のビット単位のマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

<span data-ttu-id="73fd9-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="73fd9-105">**ExcludesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="73fd9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="73fd9-106">Attributes and elements</span></span>

<span data-ttu-id="73fd9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73fd9-108">属性</span><span class="sxs-lookup"><span data-stu-id="73fd9-108">Attributes</span></span>

<span data-ttu-id="73fd9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="73fd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73fd9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="73fd9-110">Child elements</span></span>

|<span data-ttu-id="73fd9-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="73fd9-111">**Element**</span></span>|<span data-ttu-id="73fd9-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="73fd9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73fd9-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="73fd9-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="73fd9-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="73fd9-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="73fd9-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="73fd9-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="73fd9-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-119">示す</span><span class="sxs-lookup"><span data-stu-id="73fd9-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="73fd9-120">[除外](excludes.md)制限操作で使用する16進数または10進数のマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="73fd9-121">ビットマスクが16進数を表す場合は、0x または0X でプレフィックスする必要があります。</span><span class="sxs-lookup"><span data-stu-id="73fd9-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="73fd9-122">それ以外の場合は、10進数値と見なされます。</span><span class="sxs-lookup"><span data-stu-id="73fd9-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73fd9-123">親要素</span><span class="sxs-lookup"><span data-stu-id="73fd9-123">Parent elements</span></span>

|<span data-ttu-id="73fd9-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="73fd9-124">**Element**</span></span>|<span data-ttu-id="73fd9-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="73fd9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73fd9-126">制限</span><span class="sxs-lookup"><span data-stu-id="73fd9-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="73fd9-127">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-128">Not</span><span class="sxs-lookup"><span data-stu-id="73fd9-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="73fd9-129">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-130">And</span><span class="sxs-lookup"><span data-stu-id="73fd9-130">And</span></span>](and.md) <br/> |<span data-ttu-id="73fd9-131">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="73fd9-132">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="73fd9-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="73fd9-133">Or</span><span class="sxs-lookup"><span data-stu-id="73fd9-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="73fd9-134">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="73fd9-135">[または](or.md)のいずれかの子が**true**を返した場合、Or 要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73fd9-136">注釈</span><span class="sxs-lookup"><span data-stu-id="73fd9-136">Remarks</span></span>

<span data-ttu-id="73fd9-137">を**除外**すると、次のように実行された AND 操作が0に解決される場合は**true**になります。</span><span class="sxs-lookup"><span data-stu-id="73fd9-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="73fd9-138">プロパティのビット単位の値</span><span class="sxs-lookup"><span data-stu-id="73fd9-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="73fd9-139">プロパティのビットマスク値</span><span class="sxs-lookup"><span data-stu-id="73fd9-139">The bitmask value for the property</span></span>
    
<span data-ttu-id="73fd9-140">**除外**は、整数値を持つプロパティにのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="73fd9-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="73fd9-141">プロパティの型が整数以外の場合は、エラーコード**Error、Supportedpathforquery**が応答で返されます。</span><span class="sxs-lookup"><span data-stu-id="73fd9-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="73fd9-142">逆の操作を実行するには、Not (除外) を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="73fd9-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="73fd9-143">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="73fd9-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73fd9-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="73fd9-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73fd9-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="73fd9-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73fd9-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73fd9-146">Schema Name</span></span>  <br/> |<span data-ttu-id="73fd9-147">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="73fd9-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="73fd9-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73fd9-148">Validation File</span></span>  <br/> |<span data-ttu-id="73fd9-149">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="73fd9-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73fd9-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73fd9-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="73fd9-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="73fd9-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73fd9-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="73fd9-152">See also</span></span>

- [<span data-ttu-id="73fd9-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="73fd9-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

