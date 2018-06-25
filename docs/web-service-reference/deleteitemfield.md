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
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759986"
---
# <a name="deleteitemfield"></a><span data-ttu-id="4ec39-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="4ec39-103">DeleteItemField</span></span>

<span data-ttu-id="4ec39-104">**DeleteItemField**要素は、アイテムから UpdateItem 呼び出し時に指定したプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="4ec39-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4ec39-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="4ec39-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="4ec39-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="4ec39-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="4ec39-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="4ec39-108">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="4ec39-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="4ec39-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="4ec39-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 <span data-ttu-id="4ec39-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="4ec39-110">**DeleteItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ec39-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4ec39-111">Attributes and elements</span></span>

<span data-ttu-id="4ec39-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ec39-113">属性</span><span class="sxs-lookup"><span data-stu-id="4ec39-113">Attributes</span></span>

<span data-ttu-id="4ec39-114">なし。</span><span class="sxs-lookup"><span data-stu-id="4ec39-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ec39-115">子要素</span><span class="sxs-lookup"><span data-stu-id="4ec39-115">Child elements</span></span>

|<span data-ttu-id="4ec39-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ec39-116">**Element**</span></span>|<span data-ttu-id="4ec39-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ec39-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ec39-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="4ec39-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="4ec39-119">URI によって頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="4ec39-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4ec39-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="4ec39-121">ディクショナリ プロパティの個々 のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="4ec39-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4ec39-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="4ec39-123">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ec39-124">親要素</span><span class="sxs-lookup"><span data-stu-id="4ec39-124">Parent elements</span></span>

|<span data-ttu-id="4ec39-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ec39-125">**Element**</span></span>|<span data-ttu-id="4ec39-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ec39-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ec39-127">更新 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="4ec39-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="4ec39-128">定義する要素のセットが含まれていて、このオプションを設定すると、アイテムのプロパティの変更を削除します。</span><span class="sxs-lookup"><span data-stu-id="4ec39-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="4ec39-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4ec39-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ec39-130">備考</span><span class="sxs-lookup"><span data-stu-id="4ec39-130">Remarks</span></span>

<span data-ttu-id="4ec39-131">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4ec39-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ec39-132">要素情報</span><span class="sxs-lookup"><span data-stu-id="4ec39-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ec39-133">名前空間</span><span class="sxs-lookup"><span data-stu-id="4ec39-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ec39-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ec39-134">Schema Name</span></span>  <br/> |<span data-ttu-id="4ec39-135">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ec39-135">types schema</span></span>  <br/> |
|<span data-ttu-id="4ec39-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ec39-136">Validation File</span></span>  <br/> |<span data-ttu-id="4ec39-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ec39-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ec39-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ec39-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ec39-139">False</span><span class="sxs-lookup"><span data-stu-id="4ec39-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ec39-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ec39-140">See also</span></span>

- <span data-ttu-id="4ec39-141">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="4ec39-141">[UpdateItem operation](updateitem-operation.md)</span></span>

