---
title: Itemid (NonEmptyArrayOfItemIdsType)
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
description: Itemid の要素には、メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="09054-103">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="09054-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="09054-104">**Itemid**の要素には、メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09054-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="09054-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="09054-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="09054-106">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="09054-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="09054-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="09054-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09054-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="09054-108">Attributes and elements</span></span>

<span data-ttu-id="09054-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09054-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09054-110">属性</span><span class="sxs-lookup"><span data-stu-id="09054-110">Attributes</span></span>

<span data-ttu-id="09054-111">なし。</span><span class="sxs-lookup"><span data-stu-id="09054-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09054-112">子要素</span><span class="sxs-lookup"><span data-stu-id="09054-112">Child elements</span></span>

|<span data-ttu-id="09054-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="09054-113">**Element**</span></span>|<span data-ttu-id="09054-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="09054-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09054-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="09054-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="09054-116">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09054-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09054-117">親要素</span><span class="sxs-lookup"><span data-stu-id="09054-117">Parent elements</span></span>

|<span data-ttu-id="09054-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="09054-118">**Element**</span></span>|<span data-ttu-id="09054-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="09054-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09054-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="09054-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="09054-121">メールボックスからアイテムをエクスポートするための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="09054-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09054-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09054-122">Text value</span></span>

<span data-ttu-id="09054-123">なし。</span><span class="sxs-lookup"><span data-stu-id="09054-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09054-124">備考</span><span class="sxs-lookup"><span data-stu-id="09054-124">Remarks</span></span>

<span data-ttu-id="09054-125">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="09054-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09054-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="09054-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09054-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="09054-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09054-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09054-128">Schema Name</span></span>  <br/> |<span data-ttu-id="09054-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="09054-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="09054-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09054-130">Validation File</span></span>  <br/> |<span data-ttu-id="09054-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="09054-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09054-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="09054-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="09054-133">False</span><span class="sxs-lookup"><span data-stu-id="09054-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09054-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="09054-134">See also</span></span>



[<span data-ttu-id="09054-135">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="09054-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="09054-136">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="09054-136">UploadItems operation</span></span>](uploaditems-operation.md)

