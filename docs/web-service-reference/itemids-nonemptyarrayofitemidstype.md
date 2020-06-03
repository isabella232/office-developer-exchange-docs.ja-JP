---
title: ItemIds (非 Emptyarrayofitemidstype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: e895782a-74fe-4216-8ac2-c3c88c4b232d
description: ItemIds 要素には、メールボックスからエクスポートするアイテムを識別するアイテム識別子の配列が含まれています。
ms.openlocfilehash: 16c2633528e2ecbc863cfdde645e0f431b4c4297
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468594"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="05db3-103">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="05db3-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="05db3-104">**Itemids**要素には、メールボックスからエクスポートするアイテムを識別するアイテム識別子の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="05db3-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="05db3-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="05db3-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="05db3-106">ItemIds (非 Emptyarrayofitemidstype)</span><span class="sxs-lookup"><span data-stu-id="05db3-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="05db3-107">**非 Emptyarrayofitemidstype**</span><span class="sxs-lookup"><span data-stu-id="05db3-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05db3-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="05db3-108">Attributes and elements</span></span>

<span data-ttu-id="05db3-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="05db3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05db3-110">属性</span><span class="sxs-lookup"><span data-stu-id="05db3-110">Attributes</span></span>

<span data-ttu-id="05db3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="05db3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05db3-112">子要素</span><span class="sxs-lookup"><span data-stu-id="05db3-112">Child elements</span></span>

|<span data-ttu-id="05db3-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="05db3-113">**Element**</span></span>|<span data-ttu-id="05db3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="05db3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05db3-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="05db3-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="05db3-116">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="05db3-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05db3-117">親要素</span><span class="sxs-lookup"><span data-stu-id="05db3-117">Parent elements</span></span>

|<span data-ttu-id="05db3-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="05db3-118">**Element**</span></span>|<span data-ttu-id="05db3-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="05db3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05db3-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="05db3-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="05db3-121">メールボックスからアイテムをエクスポートするための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="05db3-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05db3-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="05db3-122">Text value</span></span>

<span data-ttu-id="05db3-123">なし。</span><span class="sxs-lookup"><span data-stu-id="05db3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05db3-124">注釈</span><span class="sxs-lookup"><span data-stu-id="05db3-124">Remarks</span></span>

<span data-ttu-id="05db3-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="05db3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05db3-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="05db3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05db3-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="05db3-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="05db3-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="05db3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="05db3-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="05db3-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="05db3-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="05db3-130">Validation File</span></span>  <br/> |<span data-ttu-id="05db3-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="05db3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="05db3-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="05db3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="05db3-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="05db3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05db3-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="05db3-134">See also</span></span>



[<span data-ttu-id="05db3-135">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="05db3-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="05db3-136">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="05db3-136">UploadItems operation</span></span>](uploaditems-operation.md)

