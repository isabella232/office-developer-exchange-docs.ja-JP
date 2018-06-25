---
title: 除外
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
description: 除外要素は、指定されたプロパティと提供された値のビットごとのマスクを実行します。
ms.openlocfilehash: 73e4eb782a4f54c113ea9a9b67fcf185a9028153
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760365"
---
# <a name="excludes"></a><span data-ttu-id="ca252-103">除外</span><span class="sxs-lookup"><span data-stu-id="ca252-103">Excludes</span></span>

<span data-ttu-id="ca252-104">**除外**要素は、指定されたプロパティと提供された値のビットごとのマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="ca252-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

 <span data-ttu-id="ca252-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="ca252-105">**ExcludesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca252-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ca252-106">Attributes and elements</span></span>

<span data-ttu-id="ca252-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ca252-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca252-108">属性</span><span class="sxs-lookup"><span data-stu-id="ca252-108">Attributes</span></span>

<span data-ttu-id="ca252-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ca252-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca252-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ca252-110">Child elements</span></span>

|<span data-ttu-id="ca252-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ca252-111">**Element**</span></span>|<span data-ttu-id="ca252-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ca252-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca252-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ca252-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ca252-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ca252-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ca252-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ca252-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ca252-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="ca252-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="ca252-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ca252-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ca252-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="ca252-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="ca252-119">ビットマスク</span><span class="sxs-lookup"><span data-stu-id="ca252-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="ca252-120">[Excludes](excludes.md)制限操作時に使用する 16 進数または 10 進数のマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="ca252-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="ca252-121">ビットマスクでは、16 進数を表している場合は、0x または 0x で始まる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca252-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="ca252-122">それ以外の場合と見なされます 10 進数です。</span><span class="sxs-lookup"><span data-stu-id="ca252-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca252-123">親要素</span><span class="sxs-lookup"><span data-stu-id="ca252-123">Parent elements</span></span>

|<span data-ttu-id="ca252-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="ca252-124">**Element**</span></span>|<span data-ttu-id="ca252-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="ca252-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca252-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="ca252-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="ca252-127">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="ca252-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="ca252-128">Not</span><span class="sxs-lookup"><span data-stu-id="ca252-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="ca252-129">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="ca252-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="ca252-130">And</span><span class="sxs-lookup"><span data-stu-id="ca252-130">And</span></span>](and.md) <br/> |<span data-ttu-id="ca252-131">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="ca252-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="ca252-132">**すべての And に含まれている検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="ca252-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="ca252-133">Or</span><span class="sxs-lookup"><span data-stu-id="ca252-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="ca252-134">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="ca252-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="ca252-135">その子のいずれかの**場合は true**を返す場合、要素[または](or.md)要素は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="ca252-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca252-136">備考</span><span class="sxs-lookup"><span data-stu-id="ca252-136">Remarks</span></span>

 <span data-ttu-id="ca252-137">**除外**は、0 に次のように実行されると操作が解決した場合を**true**に解決されます。</span><span class="sxs-lookup"><span data-stu-id="ca252-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="ca252-138">プロパティのビットごとの値</span><span class="sxs-lookup"><span data-stu-id="ca252-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="ca252-139">プロパティ ビットマスク値</span><span class="sxs-lookup"><span data-stu-id="ca252-139">The bitmask value for the property</span></span>
    
 <span data-ttu-id="ca252-140">**除外**は、整数値を持つプロパティにのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="ca252-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="ca252-141">プロパティの型が整数以外の場合は、応答に**ErrorUnsupportedPathForQuery**のエラー コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="ca252-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="ca252-142">Not(Excludes) を呼び出すことによって、逆の操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="ca252-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="ca252-143">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ca252-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca252-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="ca252-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca252-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="ca252-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca252-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ca252-146">Schema Name</span></span>  <br/> |<span data-ttu-id="ca252-147">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="ca252-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca252-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ca252-148">Validation File</span></span>  <br/> |<span data-ttu-id="ca252-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ca252-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca252-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ca252-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca252-151">False</span><span class="sxs-lookup"><span data-stu-id="ca252-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca252-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="ca252-152">See also</span></span>



- [<span data-ttu-id="ca252-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ca252-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

