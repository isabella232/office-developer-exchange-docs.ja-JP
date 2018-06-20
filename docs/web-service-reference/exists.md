---
title: Exists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: Exists 要素は、アイテムに対して指定されたプロパティが存在する場合は true を返す検索式を表します。
ms.openlocfilehash: d30f4b505afcac32afbfeaf2289c964ba145668e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760368"
---
# <a name="exists"></a><span data-ttu-id="9f3f2-103">Exists</span><span class="sxs-lookup"><span data-stu-id="9f3f2-103">Exists</span></span>

<span data-ttu-id="9f3f2-104">**Exists**要素では、 **true**を返す指定されたプロパティが存在する場合、アイテムの検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="9f3f2-105">**ExistsType**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f3f2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9f3f2-106">Attributes and elements</span></span>

<span data-ttu-id="9f3f2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f3f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f3f2-108">Attributes</span></span>

<span data-ttu-id="9f3f2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9f3f2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9f3f2-110">Child elements</span></span>

|<span data-ttu-id="9f3f2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-111">**Element**</span></span>|<span data-ttu-id="9f3f2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f3f2-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="9f3f2-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="9f3f2-114">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="9f3f2-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9f3f2-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="9f3f2-116">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="9f3f2-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9f3f2-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9f3f2-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f3f2-119">親要素</span><span class="sxs-lookup"><span data-stu-id="9f3f2-119">Parent elements</span></span>

|<span data-ttu-id="9f3f2-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-120">**Element**</span></span>|<span data-ttu-id="9f3f2-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f3f2-122">Restriction</span><span class="sxs-lookup"><span data-stu-id="9f3f2-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="9f3f2-123">制限またはアイテムまたはフォルダーの FindItem/FindFolder、検索フォルダーの操作にフィルターを適用するために使用するクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="9f3f2-124">Not</span><span class="sxs-lookup"><span data-stu-id="9f3f2-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="9f3f2-125">含まれている検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="9f3f2-126">And</span><span class="sxs-lookup"><span data-stu-id="9f3f2-126">And</span></span>](and.md) <br/> |<span data-ttu-id="9f3f2-127">使用すると、2 つまたは複数の検索式間で論理 And 演算を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="9f3f2-128">**And 内に含まれるすべての検索式に**該当**する場合は、And 演算の結果は**</span><span class="sxs-lookup"><span data-stu-id="9f3f2-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="9f3f2-129">Or</span><span class="sxs-lookup"><span data-stu-id="9f3f2-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="9f3f2-130">含まれている検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="9f3f2-131">[または](or.md) **true**を返します**true**を返す任意の子の場合。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f3f2-132">備考</span><span class="sxs-lookup"><span data-stu-id="9f3f2-132">Remarks</span></span>

<span data-ttu-id="9f3f2-133">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9f3f2-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f3f2-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="9f3f2-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f3f2-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="9f3f2-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f3f2-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f3f2-136">Schema Name</span></span>  <br/> |<span data-ttu-id="9f3f2-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9f3f2-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f3f2-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f3f2-138">Validation File</span></span>  <br/> |<span data-ttu-id="9f3f2-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f3f2-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f3f2-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9f3f2-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f3f2-141">False</span><span class="sxs-lookup"><span data-stu-id="9f3f2-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f3f2-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f3f2-142">See also</span></span>



- [<span data-ttu-id="9f3f2-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f3f2-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

