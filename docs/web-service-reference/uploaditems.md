---
title: UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: fd2b9545-7213-4427-95ae-71a155b75971
description: UploadItems 要素は、メールボックスにアイテムをアップロードするための要求を表します。
ms.openlocfilehash: d3cd69cdb744431daeede736c2e156c8ab92a79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839900"
---
# <a name="uploaditems"></a><span data-ttu-id="ce2f2-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="ce2f2-103">UploadItems</span></span>

<span data-ttu-id="ce2f2-104">**UploadItems**要素は、メールボックスにアイテムをアップロードするための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="ce2f2-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="ce2f2-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="ce2f2-106">**UploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="ce2f2-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce2f2-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ce2f2-107">Attributes and elements</span></span>

<span data-ttu-id="ce2f2-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce2f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce2f2-109">Attributes</span></span>

<span data-ttu-id="ce2f2-110">なし。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce2f2-111">子要素</span><span class="sxs-lookup"><span data-stu-id="ce2f2-111">Child elements</span></span>

|<span data-ttu-id="ce2f2-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="ce2f2-112">**Element**</span></span>|<span data-ttu-id="ce2f2-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce2f2-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce2f2-114">アイテム (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="ce2f2-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="ce2f2-115">メールボックスにアップロードする項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce2f2-116">親要素</span><span class="sxs-lookup"><span data-stu-id="ce2f2-116">Parent elements</span></span>

<span data-ttu-id="ce2f2-117">なし。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ce2f2-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ce2f2-118">Text value</span></span>

<span data-ttu-id="ce2f2-119">なし。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce2f2-120">備考</span><span class="sxs-lookup"><span data-stu-id="ce2f2-120">Remarks</span></span>

<span data-ttu-id="ce2f2-121">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ce2f2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce2f2-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="ce2f2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce2f2-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="ce2f2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce2f2-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce2f2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ce2f2-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ce2f2-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="ce2f2-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce2f2-126">Validation File</span></span>  <br/> |<span data-ttu-id="ce2f2-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce2f2-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce2f2-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ce2f2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce2f2-129">False</span><span class="sxs-lookup"><span data-stu-id="ce2f2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce2f2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce2f2-130">See also</span></span>



[<span data-ttu-id="ce2f2-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="ce2f2-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="ce2f2-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="ce2f2-132">UploadItems operation</span></span>](uploaditems-operation.md)

