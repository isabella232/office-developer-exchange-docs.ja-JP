---
title: Updates (Item)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: 5c1a855e-390d-4713-9d10-6e86ca392814
description: Updates 要素には、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。
ms.openlocfilehash: 6902ea4d3d3d9adc074745d5642cdfa6d91a9163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456354"
---
# <a name="updates-item"></a><span data-ttu-id="81ab3-103">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="81ab3-103">Updates (Item)</span></span>

<span data-ttu-id="81ab3-104">**Updates**要素には、アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81ab3-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="81ab3-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="81ab3-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="81ab3-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="81ab3-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="81ab3-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="81ab3-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="81ab3-108">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="81ab3-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="81ab3-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="81ab3-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="81ab3-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="81ab3-110">Attributes and elements</span></span>

<span data-ttu-id="81ab3-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="81ab3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81ab3-112">属性</span><span class="sxs-lookup"><span data-stu-id="81ab3-112">Attributes</span></span>

<span data-ttu-id="81ab3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="81ab3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81ab3-114">子要素</span><span class="sxs-lookup"><span data-stu-id="81ab3-114">Child elements</span></span>

|<span data-ttu-id="81ab3-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="81ab3-115">**Element**</span></span>|<span data-ttu-id="81ab3-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="81ab3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81ab3-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="81ab3-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="81ab3-118">[Updateitem 操作](updateitem-operation.md)中に、アイテムの1つのプロパティに追加するデータを表します。</span><span class="sxs-lookup"><span data-stu-id="81ab3-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="81ab3-119">SetItemField</span><span class="sxs-lookup"><span data-stu-id="81ab3-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="81ab3-120">[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。</span><span class="sxs-lookup"><span data-stu-id="81ab3-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="81ab3-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="81ab3-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="81ab3-122">[Updateitem 操作](updateitem-operation.md)中に、指定されたプロパティをアイテムから削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="81ab3-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81ab3-123">親要素</span><span class="sxs-lookup"><span data-stu-id="81ab3-123">Parent elements</span></span>

|<span data-ttu-id="81ab3-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="81ab3-124">**Element**</span></span>|<span data-ttu-id="81ab3-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="81ab3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81ab3-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="81ab3-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="81ab3-127">アイテム識別子と、アイテムに適用する更新を含みます。</span><span class="sxs-lookup"><span data-stu-id="81ab3-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="81ab3-128">この要素の XPath 式を次に示します。`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="81ab3-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81ab3-129">注釈</span><span class="sxs-lookup"><span data-stu-id="81ab3-129">Remarks</span></span>

<span data-ttu-id="81ab3-130">この要素によって定義された更新は、 [ItemId](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)要素によって識別されるアイテムに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="81ab3-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="81ab3-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="81ab3-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81ab3-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="81ab3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81ab3-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="81ab3-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81ab3-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="81ab3-134">Schema Name</span></span>  <br/> |<span data-ttu-id="81ab3-135">types スキーマ</span><span class="sxs-lookup"><span data-stu-id="81ab3-135">types schema</span></span>  <br/> |
|<span data-ttu-id="81ab3-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="81ab3-136">Validation File</span></span>  <br/> |<span data-ttu-id="81ab3-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="81ab3-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81ab3-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="81ab3-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="81ab3-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="81ab3-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81ab3-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="81ab3-140">See also</span></span>

- [<span data-ttu-id="81ab3-141">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="81ab3-141">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="81ab3-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="81ab3-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

