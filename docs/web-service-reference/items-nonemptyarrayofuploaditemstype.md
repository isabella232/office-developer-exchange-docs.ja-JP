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
description: 項目要素には、メールボックスにアップロードする項目の配列が含まれています。
ms.openlocfilehash: ac508b2026c3e0ec730154efeeff0a9669e6eff8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832156"
---
# <a name="items-nonemptyarrayofuploaditemstype"></a><span data-ttu-id="00d4b-103">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="00d4b-103">Items (NonEmptyArrayOfUploadItemsType)</span></span>

<span data-ttu-id="00d4b-104">**項目**要素には、メールボックスにアップロードする項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="00d4b-104">The **Items** element contains an array of items to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="00d4b-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="00d4b-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="00d4b-106">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="00d4b-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
```XML
<Items>
   <Item/>
</Items>
```

 <span data-ttu-id="00d4b-107">**NonEmptyArrayOfUploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="00d4b-107">**NonEmptyArrayOfUploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00d4b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="00d4b-108">Attributes and elements</span></span>

<span data-ttu-id="00d4b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="00d4b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00d4b-110">属性</span><span class="sxs-lookup"><span data-stu-id="00d4b-110">Attributes</span></span>

<span data-ttu-id="00d4b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="00d4b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00d4b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="00d4b-112">Child elements</span></span>

|<span data-ttu-id="00d4b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="00d4b-113">**Element**</span></span>|<span data-ttu-id="00d4b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="00d4b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d4b-115">項目 (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="00d4b-115">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="00d4b-116">メールボックスにアップロードする 1 つの項目を表します。</span><span class="sxs-lookup"><span data-stu-id="00d4b-116">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00d4b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="00d4b-117">Parent elements</span></span>

|<span data-ttu-id="00d4b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="00d4b-118">**Element**</span></span>|<span data-ttu-id="00d4b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="00d4b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d4b-120">UploadItems</span><span class="sxs-lookup"><span data-stu-id="00d4b-120">UploadItems</span></span>](uploaditems.md) <br/> |<span data-ttu-id="00d4b-121">メールボックスにアイテムをアップロードするための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="00d4b-121">Represents a request to upload items into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00d4b-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="00d4b-122">Text value</span></span>

<span data-ttu-id="00d4b-123">なし。</span><span class="sxs-lookup"><span data-stu-id="00d4b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00d4b-124">備考</span><span class="sxs-lookup"><span data-stu-id="00d4b-124">Remarks</span></span>

<span data-ttu-id="00d4b-125">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="00d4b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00d4b-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="00d4b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00d4b-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="00d4b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00d4b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="00d4b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="00d4b-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="00d4b-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="00d4b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="00d4b-130">Validation File</span></span>  <br/> |<span data-ttu-id="00d4b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00d4b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00d4b-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="00d4b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="00d4b-133">False</span><span class="sxs-lookup"><span data-stu-id="00d4b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00d4b-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="00d4b-134">See also</span></span>



[<span data-ttu-id="00d4b-135">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="00d4b-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="00d4b-136">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="00d4b-136">UploadItems operation</span></span>](uploaditems-operation.md)

