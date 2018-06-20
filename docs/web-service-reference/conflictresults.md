---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: ConflictResults 要素には、競合 UpdateItem 操作の応答の数が含まれています。
ms.openlocfilehash: faa6dc6c5fbbe874438a89c810a12fa675e8a1c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759657"
---
# <a name="conflictresults"></a><span data-ttu-id="f73ee-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="f73ee-103">ConflictResults</span></span>

<span data-ttu-id="f73ee-104">[ConflictResults](conflictresults.md)要素には、競合[UpdateItem 操作](updateitem-operation.md)の応答の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f73ee-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="f73ee-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="f73ee-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="f73ee-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f73ee-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="f73ee-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f73ee-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="f73ee-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="f73ee-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="f73ee-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="f73ee-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f73ee-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f73ee-110">Attributes and elements</span></span>

<span data-ttu-id="f73ee-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f73ee-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f73ee-112">属性</span><span class="sxs-lookup"><span data-stu-id="f73ee-112">Attributes</span></span>

<span data-ttu-id="f73ee-113">なし。</span><span class="sxs-lookup"><span data-stu-id="f73ee-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f73ee-114">子要素</span><span class="sxs-lookup"><span data-stu-id="f73ee-114">Child elements</span></span>

|<span data-ttu-id="f73ee-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="f73ee-115">**Element**</span></span>|<span data-ttu-id="f73ee-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="f73ee-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ee-117">Count</span><span class="sxs-lookup"><span data-stu-id="f73ee-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="f73ee-118">[UpdateItem 操作](updateitem-operation.md)の応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f73ee-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f73ee-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f73ee-119">Parent elements</span></span>

|<span data-ttu-id="f73ee-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="f73ee-120">**Element**</span></span>|<span data-ttu-id="f73ee-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f73ee-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ee-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f73ee-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="f73ee-123">状態および 1 つの結果が含まれています[UpdateItem 操作](updateitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="f73ee-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f73ee-124">備考</span><span class="sxs-lookup"><span data-stu-id="f73ee-124">Remarks</span></span>

<span data-ttu-id="f73ee-125">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f73ee-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f73ee-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="f73ee-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f73ee-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="f73ee-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f73ee-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f73ee-128">Schema Name</span></span>  <br/> |<span data-ttu-id="f73ee-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f73ee-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="f73ee-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f73ee-130">Validation File</span></span>  <br/> |<span data-ttu-id="f73ee-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f73ee-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f73ee-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f73ee-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="f73ee-133">False</span><span class="sxs-lookup"><span data-stu-id="f73ee-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f73ee-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="f73ee-134">See also</span></span>



<span data-ttu-id="f73ee-135">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="f73ee-135">[UpdateItem operation](updateitem-operation.md)</span></span>
  
 <span data-ttu-id="f73ee-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="f73ee-136">**ConflictResultsType**</span></span>

