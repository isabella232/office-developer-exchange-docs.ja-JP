---
title: アイテム (NonEmptyArrayOfUploadItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 402bfa6d-11d7-4547-b8bd-197e9922ab49
description: Items 要素には、メールボックスにアップロードするアイテムの配列が含まれています。
ms.openlocfilehash: 5c69134c1613b0a4595a6aa876fa09fde63043ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44441549"
---
# <a name="items-nonemptyarrayofuploaditemstype"></a><span data-ttu-id="0f34a-103">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="0f34a-103">Items (NonEmptyArrayOfUploadItemsType)</span></span>

<span data-ttu-id="0f34a-104">**Items**要素には、メールボックスにアップロードするアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0f34a-104">The **Items** element contains an array of items to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="0f34a-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="0f34a-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="0f34a-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="0f34a-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
```XML
<Items>
   <Item/>
</Items>
```

 <span data-ttu-id="0f34a-107">**NonEmptyArrayOfUploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="0f34a-107">**NonEmptyArrayOfUploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f34a-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0f34a-108">Attributes and elements</span></span>

<span data-ttu-id="0f34a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0f34a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f34a-110">属性</span><span class="sxs-lookup"><span data-stu-id="0f34a-110">Attributes</span></span>

<span data-ttu-id="0f34a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0f34a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f34a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0f34a-112">Child elements</span></span>

|<span data-ttu-id="0f34a-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="0f34a-113">**Element**</span></span>|<span data-ttu-id="0f34a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f34a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f34a-115">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="0f34a-115">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="0f34a-116">メールボックスにアップロードする単一のアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="0f34a-116">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f34a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0f34a-117">Parent elements</span></span>

|<span data-ttu-id="0f34a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="0f34a-118">**Element**</span></span>|<span data-ttu-id="0f34a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f34a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f34a-120">UploadItems</span><span class="sxs-lookup"><span data-stu-id="0f34a-120">UploadItems</span></span>](uploaditems.md) <br/> |<span data-ttu-id="0f34a-121">メールボックスにアイテムをアップロードする要求を表します。</span><span class="sxs-lookup"><span data-stu-id="0f34a-121">Represents a request to upload items into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f34a-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0f34a-122">Text value</span></span>

<span data-ttu-id="0f34a-123">なし。</span><span class="sxs-lookup"><span data-stu-id="0f34a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f34a-124">注釈</span><span class="sxs-lookup"><span data-stu-id="0f34a-124">Remarks</span></span>

<span data-ttu-id="0f34a-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0f34a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f34a-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0f34a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f34a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f34a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0f34a-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0f34a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0f34a-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0f34a-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="0f34a-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0f34a-130">Validation File</span></span>  <br/> |<span data-ttu-id="0f34a-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0f34a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0f34a-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0f34a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f34a-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="0f34a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f34a-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f34a-134">See also</span></span>



[<span data-ttu-id="0f34a-135">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="0f34a-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="0f34a-136">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="0f34a-136">UploadItems operation</span></span>](uploaditems-operation.md)

