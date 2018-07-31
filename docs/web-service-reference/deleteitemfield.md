---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: DeleteItemField 要素は、アイテムから UpdateItem 呼び出し時に指定したプロパティを削除する操作を表します。
ms.openlocfilehash: 571227eece8f717c1bf5da27cfab8ae50dfe3572
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353883"
---
# <a name="deleteitemfield"></a><span data-ttu-id="3e6a4-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="3e6a4-103">DeleteItemField</span></span>

<span data-ttu-id="3e6a4-104">**DeleteItemField**要素は、アイテムから UpdateItem 呼び出し時に指定したプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="3e6a4-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="3e6a4-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="3e6a4-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="3e6a4-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="3e6a4-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="3e6a4-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="3e6a4-108">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="3e6a4-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="3e6a4-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="3e6a4-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

```xml
<DeleteItemField>
   <IndexedFieldURI/> 
</DeleteItemField>
```

```xml
<DeleteItemField>
   <ExtendedFieldURI/>
</DeleteItemField>
```

<span data-ttu-id="3e6a4-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="3e6a4-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3e6a4-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3e6a4-111">Attributes and elements</span></span>

<span data-ttu-id="3e6a4-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e6a4-113">属性</span><span class="sxs-lookup"><span data-stu-id="3e6a4-113">Attributes</span></span>

<span data-ttu-id="3e6a4-114">なし。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e6a4-115">子要素</span><span class="sxs-lookup"><span data-stu-id="3e6a4-115">Child elements</span></span>

|<span data-ttu-id="3e6a4-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3e6a4-116">**Element**</span></span>|<span data-ttu-id="3e6a4-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e6a4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e6a4-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="3e6a4-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="3e6a4-119">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="3e6a4-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="3e6a4-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="3e6a4-121">ディクショナリ プロパティの個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="3e6a4-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="3e6a4-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="3e6a4-123">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e6a4-124">親要素</span><span class="sxs-lookup"><span data-stu-id="3e6a4-124">Parent elements</span></span>

|<span data-ttu-id="3e6a4-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="3e6a4-125">**Element**</span></span>|<span data-ttu-id="3e6a4-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e6a4-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e6a4-127">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="3e6a4-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="3e6a4-128">定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="3e6a4-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3e6a4-130">注釈</span><span class="sxs-lookup"><span data-stu-id="3e6a4-130">Remarks</span></span>

<span data-ttu-id="3e6a4-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3e6a4-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e6a4-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="3e6a4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e6a4-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="3e6a4-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e6a4-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3e6a4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="3e6a4-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3e6a4-135">types schema</span></span>  <br/> |
|<span data-ttu-id="3e6a4-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3e6a4-136">Validation File</span></span>  <br/> |<span data-ttu-id="3e6a4-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e6a4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e6a4-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3e6a4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e6a4-139">False</span><span class="sxs-lookup"><span data-stu-id="3e6a4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e6a4-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e6a4-140">See also</span></span>

- <span data-ttu-id="3e6a4-141">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="3e6a4-141">[UpdateItem operation](updateitem-operation.md)</span></span>

