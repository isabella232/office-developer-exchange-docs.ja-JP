---
title: FieldOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldOrder
api_type:
- schema
ms.assetid: b9364842-bbe2-4221-afef-bf5022bc89ec
description: FieldOrder 要素は、結果の並べ替えに使用する単一のフィールドを表し、並べ替えの方向を示します。
ms.openlocfilehash: 10e28f066f7fa6799bf6b03b694d98825f95626d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760471"
---
# <a name="fieldorder"></a><span data-ttu-id="0fe06-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="0fe06-103">FieldOrder</span></span>

<span data-ttu-id="0fe06-104">**FieldOrder**要素は、結果の並べ替えに使用する単一のフィールドを表し、並べ替えの方向を示します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

 <span data-ttu-id="0fe06-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="0fe06-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0fe06-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0fe06-106">Attributes and elements</span></span>

<span data-ttu-id="0fe06-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fe06-108">属性</span><span class="sxs-lookup"><span data-stu-id="0fe06-108">Attributes</span></span>

|<span data-ttu-id="0fe06-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="0fe06-109">**Attribute**</span></span>|<span data-ttu-id="0fe06-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fe06-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0fe06-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="0fe06-111">**Order**</span></span> <br/> | <span data-ttu-id="0fe06-112">並べ替え順序の方向を説明します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="0fe06-113">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="0fe06-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="0fe06-114">-昇順</span><span class="sxs-lookup"><span data-stu-id="0fe06-114">-  Ascending</span></span>  <br/><span data-ttu-id="0fe06-115">降下</span><span class="sxs-lookup"><span data-stu-id="0fe06-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0fe06-116">子要素</span><span class="sxs-lookup"><span data-stu-id="0fe06-116">Child elements</span></span>

|<span data-ttu-id="0fe06-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0fe06-117">**Element**</span></span>|<span data-ttu-id="0fe06-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fe06-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fe06-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0fe06-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="0fe06-120">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="0fe06-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0fe06-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="0fe06-122">辞書の個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="0fe06-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0fe06-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="0fe06-124">MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fe06-125">親要素</span><span class="sxs-lookup"><span data-stu-id="0fe06-125">Parent elements</span></span>

|<span data-ttu-id="0fe06-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="0fe06-126">**Element**</span></span>|<span data-ttu-id="0fe06-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="0fe06-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fe06-128">並べ替え順序</span><span class="sxs-lookup"><span data-stu-id="0fe06-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="0fe06-129">FindItem 要求内のアイテムの並べ替え方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="0fe06-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="0fe06-130">この要素への XPath 式は、次のようにします。`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="0fe06-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0fe06-131">備考</span><span class="sxs-lookup"><span data-stu-id="0fe06-131">Remarks</span></span>

<span data-ttu-id="0fe06-132">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0fe06-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fe06-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="0fe06-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fe06-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="0fe06-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fe06-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0fe06-135">Schema Name</span></span>  <br/> |<span data-ttu-id="0fe06-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0fe06-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fe06-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0fe06-137">Validation File</span></span>  <br/> |<span data-ttu-id="0fe06-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fe06-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fe06-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0fe06-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="0fe06-140">False</span><span class="sxs-lookup"><span data-stu-id="0fe06-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fe06-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="0fe06-141">See also</span></span>

- [<span data-ttu-id="0fe06-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0fe06-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

