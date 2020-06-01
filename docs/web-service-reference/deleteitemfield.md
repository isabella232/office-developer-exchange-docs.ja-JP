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
description: DeleteItemField 要素は、UpdateItem 呼び出し中にアイテムから特定のプロパティを削除する操作を表します。
ms.openlocfilehash: e6f5ee8a1130d7c040f3ddd94021eff6d4a758b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455675"
---
# <a name="deleteitemfield"></a><span data-ttu-id="0376c-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="0376c-103">DeleteItemField</span></span>

<span data-ttu-id="0376c-104">**Deleteitemfield**要素は、updateitem 呼び出し中にアイテムから特定のプロパティを削除する操作を表します。</span><span class="sxs-lookup"><span data-stu-id="0376c-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="0376c-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="0376c-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="0376c-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="0376c-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="0376c-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="0376c-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="0376c-108">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="0376c-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="0376c-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="0376c-109">DeleteItemField</span></span>](deleteitemfield.md)
  
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

<span data-ttu-id="0376c-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="0376c-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0376c-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0376c-111">Attributes and elements</span></span>

<span data-ttu-id="0376c-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0376c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0376c-113">属性</span><span class="sxs-lookup"><span data-stu-id="0376c-113">Attributes</span></span>

<span data-ttu-id="0376c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="0376c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0376c-115">子要素</span><span class="sxs-lookup"><span data-stu-id="0376c-115">Child elements</span></span>

|<span data-ttu-id="0376c-116">**Element**</span><span class="sxs-lookup"><span data-stu-id="0376c-116">**Element**</span></span>|<span data-ttu-id="0376c-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="0376c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0376c-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0376c-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="0376c-119">URI で頻繁に参照されるプロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="0376c-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="0376c-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0376c-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="0376c-121">Dictionary プロパティの個々のメンバーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0376c-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="0376c-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0376c-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="0376c-123">拡張 MAPI プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="0376c-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0376c-124">親要素</span><span class="sxs-lookup"><span data-stu-id="0376c-124">Parent elements</span></span>

|<span data-ttu-id="0376c-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="0376c-125">**Element**</span></span>|<span data-ttu-id="0376c-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="0376c-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0376c-127">Updates (Item)</span><span class="sxs-lookup"><span data-stu-id="0376c-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="0376c-128">アイテムのプロパティに対する追加、設定、および削除の変更を定義する一連の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0376c-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="0376c-129">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0376c-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0376c-130">注釈</span><span class="sxs-lookup"><span data-stu-id="0376c-130">Remarks</span></span>

<span data-ttu-id="0376c-131">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0376c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0376c-132">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0376c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0376c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="0376c-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0376c-134">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0376c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="0376c-135">types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0376c-135">types schema</span></span>  <br/> |
|<span data-ttu-id="0376c-136">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0376c-136">Validation File</span></span>  <br/> |<span data-ttu-id="0376c-137">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0376c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0376c-138">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0376c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="0376c-139">正しくない</span><span class="sxs-lookup"><span data-stu-id="0376c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0376c-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="0376c-140">See also</span></span>

- <span data-ttu-id="0376c-141">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="0376c-141">[UpdateItem operation](updateitem-operation.md)</span></span>

