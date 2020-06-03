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
description: ConflictResults 要素には、UpdateItem 操作応答の競合の数が含まれています。
ms.openlocfilehash: 923c7950e21039adf28e232486f4df5fc04889d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460170"
---
# <a name="conflictresults"></a><span data-ttu-id="9ea1e-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="9ea1e-103">ConflictResults</span></span>

<span data-ttu-id="9ea1e-104">[ConflictResults](conflictresults.md)要素には、 [updateitem 操作](updateitem-operation.md)応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="9ea1e-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="9ea1e-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="9ea1e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9ea1e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="9ea1e-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9ea1e-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="9ea1e-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="9ea1e-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="9ea1e-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ea1e-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9ea1e-110">Attributes and elements</span></span>

<span data-ttu-id="9ea1e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ea1e-112">属性</span><span class="sxs-lookup"><span data-stu-id="9ea1e-112">Attributes</span></span>

<span data-ttu-id="9ea1e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ea1e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9ea1e-114">Child elements</span></span>

|<span data-ttu-id="9ea1e-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-115">**Element**</span></span>|<span data-ttu-id="9ea1e-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ea1e-117">Count</span><span class="sxs-lookup"><span data-stu-id="9ea1e-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="9ea1e-118">[Updateitem 操作](updateitem-operation.md)応答の競合の数を格納します。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ea1e-119">親要素</span><span class="sxs-lookup"><span data-stu-id="9ea1e-119">Parent elements</span></span>

|<span data-ttu-id="9ea1e-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-120">**Element**</span></span>|<span data-ttu-id="9ea1e-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ea1e-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9ea1e-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="9ea1e-123">1つの[Updateitem 操作](updateitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ea1e-124">注釈</span><span class="sxs-lookup"><span data-stu-id="9ea1e-124">Remarks</span></span>

<span data-ttu-id="9ea1e-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9ea1e-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ea1e-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9ea1e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ea1e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ea1e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ea1e-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ea1e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="9ea1e-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9ea1e-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ea1e-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ea1e-130">Validation File</span></span>  <br/> |<span data-ttu-id="9ea1e-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9ea1e-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ea1e-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ea1e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ea1e-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="9ea1e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ea1e-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ea1e-134">See also</span></span>



[<span data-ttu-id="9ea1e-135">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="9ea1e-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="9ea1e-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="9ea1e-136">**ConflictResultsType**</span></span>

