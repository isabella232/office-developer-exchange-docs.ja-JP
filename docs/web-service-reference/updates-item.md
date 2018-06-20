---
title: 更新 (アイテム)
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
description: 更新プログラムの要素には、定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。
ms.openlocfilehash: 13df458c783b942e1c868853c41b6247119cf123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839890"
---
# <a name="updates-item"></a><span data-ttu-id="dba90-103">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="dba90-103">Updates (Item)</span></span>

<span data-ttu-id="dba90-104">**更新プログラム**の要素には、定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="dba90-104">The **Updates** element contains a set of elements that define append, set, and delete changes to item properties.</span></span> 
  
- [<span data-ttu-id="dba90-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="dba90-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="dba90-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="dba90-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="dba90-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="dba90-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="dba90-108">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="dba90-108">Updates (Item)</span></span>](updates-item.md)
  
```xml
<Updates>
   <AppendToItemField/>
   <SetItemField/>
   <DeleteItemField/>
</Updates>
```

<span data-ttu-id="dba90-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="dba90-109">**NonEmptyArrayOfItemChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dba90-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dba90-110">Attributes and elements</span></span>

<span data-ttu-id="dba90-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dba90-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dba90-112">属性</span><span class="sxs-lookup"><span data-stu-id="dba90-112">Attributes</span></span>

<span data-ttu-id="dba90-113">なし。</span><span class="sxs-lookup"><span data-stu-id="dba90-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dba90-114">子要素</span><span class="sxs-lookup"><span data-stu-id="dba90-114">Child elements</span></span>

|<span data-ttu-id="dba90-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="dba90-115">**Element**</span></span>|<span data-ttu-id="dba90-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="dba90-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dba90-117">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="dba90-117">AppendToItemField</span></span>](appendtoitemfield.md) <br/> |<span data-ttu-id="dba90-118">[UpdateItem 操作](updateitem-operation.md)中に 1 つのアイテムのプロパティを追加するデータを表します。</span><span class="sxs-lookup"><span data-stu-id="dba90-118">Represents data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="dba90-119">SetItemField</span><span class="sxs-lookup"><span data-stu-id="dba90-119">SetItemField</span></span>](setitemfield.md) <br/> |<span data-ttu-id="dba90-120">[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。</span><span class="sxs-lookup"><span data-stu-id="dba90-120">Represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="dba90-121">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="dba90-121">DeleteItemField</span></span>](deleteitemfield.md) <br/> |<span data-ttu-id="dba90-122">[UpdateItem 操作](updateitem-operation.md)中に、アイテムから指定されたプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="dba90-122">Represents an operation to delete a given property from an item during an [UpdateItem operation](updateitem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dba90-123">親要素</span><span class="sxs-lookup"><span data-stu-id="dba90-123">Parent elements</span></span>

|<span data-ttu-id="dba90-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="dba90-124">**Element**</span></span>|<span data-ttu-id="dba90-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="dba90-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dba90-126">ItemChange</span><span class="sxs-lookup"><span data-stu-id="dba90-126">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="dba90-127">アイテム識別子と、アイテムに適用する更新プログラムが含まれています。</span><span class="sxs-lookup"><span data-stu-id="dba90-127">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> <span data-ttu-id="dba90-128">この要素への XPath 式は、次のようにします。`/UpdateItem/ItemChanges/ItemChange[i]`</span><span class="sxs-lookup"><span data-stu-id="dba90-128">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dba90-129">備考</span><span class="sxs-lookup"><span data-stu-id="dba90-129">Remarks</span></span>

<span data-ttu-id="dba90-130">[アイテム Id](itemid.md)、 [OccurrenceItemId](occurrenceitemid.md)、または[RecurringMasterItemId](recurringmasteritemid.md)の要素で識別される項目には、この要素で定義されている更新プログラムが実行されます。</span><span class="sxs-lookup"><span data-stu-id="dba90-130">The updates that are defined by this element are performed on the item that is identified by the [ItemId](itemid.md), [OccurrenceItemId](occurrenceitemid.md), or [RecurringMasterItemId](recurringmasteritemid.md) elements.</span></span> 
  
<span data-ttu-id="dba90-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="dba90-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dba90-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="dba90-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dba90-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="dba90-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dba90-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dba90-134">Schema Name</span></span>  <br/> |<span data-ttu-id="dba90-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dba90-135">types schema</span></span>  <br/> |
|<span data-ttu-id="dba90-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dba90-136">Validation File</span></span>  <br/> |<span data-ttu-id="dba90-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dba90-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dba90-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="dba90-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="dba90-139">False</span><span class="sxs-lookup"><span data-stu-id="dba90-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dba90-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="dba90-140">See also</span></span>

- <span data-ttu-id="dba90-141">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dba90-141">[UpdateItem operation](updateitem-operation.md)</span></span>
- [<span data-ttu-id="dba90-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dba90-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

