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
description: Exists 要素は、指定されたプロパティがアイテムに存在する場合に true を返す検索式を表します。
ms.openlocfilehash: b5e7a24c5214574ef385cd6ffca87ed5f861c188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456949"
---
# <a name="exists"></a><span data-ttu-id="d89a5-103">Exists</span><span class="sxs-lookup"><span data-stu-id="d89a5-103">Exists</span></span>

<span data-ttu-id="d89a5-104">**Exists**要素は、指定されたプロパティがアイテムに存在する場合に**true**を返す検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="d89a5-105">**存在**</span><span class="sxs-lookup"><span data-stu-id="d89a5-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d89a5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d89a5-106">Attributes and elements</span></span>

<span data-ttu-id="d89a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d89a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="d89a5-108">Attributes</span></span>

<span data-ttu-id="d89a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d89a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d89a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d89a5-110">Child elements</span></span>

|<span data-ttu-id="d89a5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d89a5-111">**Element**</span></span>|<span data-ttu-id="d89a5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89a5-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d89a5-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="d89a5-114">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="d89a5-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d89a5-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="d89a5-116">辞書の個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="d89a5-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="d89a5-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="d89a5-118">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d89a5-119">親要素</span><span class="sxs-lookup"><span data-stu-id="d89a5-119">Parent elements</span></span>

|<span data-ttu-id="d89a5-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="d89a5-120">**Element**</span></span>|<span data-ttu-id="d89a5-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d89a5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89a5-122">制限</span><span class="sxs-lookup"><span data-stu-id="d89a5-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="d89a5-123">FindItem/FindFolder および search folder 操作のアイテムまたはフォルダーをフィルター処理するために使用される制限またはクエリを表します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="d89a5-124">Not</span><span class="sxs-lookup"><span data-stu-id="d89a5-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="d89a5-125">含まれる検索式のブール値を否定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="d89a5-126">And</span><span class="sxs-lookup"><span data-stu-id="d89a5-126">And</span></span>](and.md) <br/> |<span data-ttu-id="d89a5-127">2つ以上の検索式の間でブール値と演算を実行できる検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="d89a5-128">And 操作の結果は、に含まれるすべての検索式が**true**である場合に**true**となります。</span><span class="sxs-lookup"><span data-stu-id="d89a5-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="d89a5-129">Or</span><span class="sxs-lookup"><span data-stu-id="d89a5-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="d89a5-130">含まれる検索式に対して論理 OR を実行する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="d89a5-131">[または](or.md)、いずれかの子が**true**を返した場合は**true**を返します。</span><span class="sxs-lookup"><span data-stu-id="d89a5-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d89a5-132">注釈</span><span class="sxs-lookup"><span data-stu-id="d89a5-132">Remarks</span></span>

<span data-ttu-id="d89a5-133">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="d89a5-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d89a5-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d89a5-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d89a5-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="d89a5-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d89a5-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d89a5-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d89a5-137">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d89a5-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="d89a5-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d89a5-138">Validation File</span></span>  <br/> |<span data-ttu-id="d89a5-139">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d89a5-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d89a5-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d89a5-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d89a5-141">正しくない</span><span class="sxs-lookup"><span data-stu-id="d89a5-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d89a5-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="d89a5-142">See also</span></span>



- [<span data-ttu-id="d89a5-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d89a5-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

