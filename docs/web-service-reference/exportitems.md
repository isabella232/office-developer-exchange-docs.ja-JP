---
title: ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: bbbc56e4-8cc1-43ae-b70a-9a8d6bb0f399
description: ExportItems 要素は、メールボックスからアイテムをエクスポートするための要求を表します。
ms.openlocfilehash: 055012166bb125dfcf86070f2e23496bf0209b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760377"
---
# <a name="exportitems"></a><span data-ttu-id="993b1-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="993b1-103">ExportItems</span></span>

<span data-ttu-id="993b1-104">**ExportItems**要素は、メールボックスからアイテムをエクスポートするための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="993b1-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="993b1-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="993b1-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="993b1-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="993b1-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="993b1-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="993b1-107">Attributes and elements</span></span>

<span data-ttu-id="993b1-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="993b1-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="993b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="993b1-109">Attributes</span></span>

<span data-ttu-id="993b1-110">なし。</span><span class="sxs-lookup"><span data-stu-id="993b1-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="993b1-111">子要素</span><span class="sxs-lookup"><span data-stu-id="993b1-111">Child elements</span></span>

|<span data-ttu-id="993b1-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="993b1-112">**Element**</span></span>|<span data-ttu-id="993b1-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="993b1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="993b1-114">Itemid (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="993b1-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="993b1-115">メールボックスからエクスポートする項目を識別する項目 id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="993b1-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="993b1-116">親要素</span><span class="sxs-lookup"><span data-stu-id="993b1-116">Parent elements</span></span>

<span data-ttu-id="993b1-117">なし。</span><span class="sxs-lookup"><span data-stu-id="993b1-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="993b1-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="993b1-118">Text value</span></span>

<span data-ttu-id="993b1-119">なし。</span><span class="sxs-lookup"><span data-stu-id="993b1-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="993b1-120">備考</span><span class="sxs-lookup"><span data-stu-id="993b1-120">Remarks</span></span>

<span data-ttu-id="993b1-121">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="993b1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="993b1-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="993b1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="993b1-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="993b1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="993b1-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="993b1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="993b1-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="993b1-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="993b1-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="993b1-126">Validation File</span></span>  <br/> |<span data-ttu-id="993b1-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="993b1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="993b1-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="993b1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="993b1-129">False</span><span class="sxs-lookup"><span data-stu-id="993b1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="993b1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="993b1-130">See also</span></span>



[<span data-ttu-id="993b1-131">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="993b1-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="993b1-132">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="993b1-132">UploadItems operation</span></span>](uploaditems-operation.md)

