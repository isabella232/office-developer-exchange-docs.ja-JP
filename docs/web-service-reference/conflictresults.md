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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460170"
---
# <a name="conflictresults"></a><span data-ttu-id="549f9-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="549f9-103">ConflictResults</span></span>

<span data-ttu-id="549f9-104">[ConflictResults](conflictresults.md)要素には、 [updateitem 操作](updateitem-operation.md)応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="549f9-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="549f9-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="549f9-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="549f9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="549f9-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="549f9-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="549f9-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="549f9-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="549f9-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="549f9-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="549f9-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="549f9-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="549f9-110">Attributes and elements</span></span>

<span data-ttu-id="549f9-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="549f9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="549f9-112">属性</span><span class="sxs-lookup"><span data-stu-id="549f9-112">Attributes</span></span>

<span data-ttu-id="549f9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="549f9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="549f9-114">子要素</span><span class="sxs-lookup"><span data-stu-id="549f9-114">Child elements</span></span>

|<span data-ttu-id="549f9-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="549f9-115">**Element**</span></span>|<span data-ttu-id="549f9-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="549f9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="549f9-117">Count</span><span class="sxs-lookup"><span data-stu-id="549f9-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="549f9-118">[Updateitem 操作](updateitem-operation.md)応答の競合の数を格納します。</span><span class="sxs-lookup"><span data-stu-id="549f9-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="549f9-119">親要素</span><span class="sxs-lookup"><span data-stu-id="549f9-119">Parent elements</span></span>

|<span data-ttu-id="549f9-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="549f9-120">**Element**</span></span>|<span data-ttu-id="549f9-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="549f9-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="549f9-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="549f9-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="549f9-123">1つの[Updateitem 操作](updateitem-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="549f9-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="549f9-124">注釈</span><span class="sxs-lookup"><span data-stu-id="549f9-124">Remarks</span></span>

<span data-ttu-id="549f9-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="549f9-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="549f9-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="549f9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="549f9-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="549f9-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="549f9-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="549f9-128">Schema Name</span></span>  <br/> |<span data-ttu-id="549f9-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="549f9-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="549f9-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="549f9-130">Validation File</span></span>  <br/> |<span data-ttu-id="549f9-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="549f9-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="549f9-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="549f9-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="549f9-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="549f9-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="549f9-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="549f9-134">See also</span></span>



<span data-ttu-id="549f9-135">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="549f9-135">[UpdateItem operation](updateitem-operation.md)</span></span>
  
 <span data-ttu-id="549f9-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="549f9-136">**ConflictResultsType**</span></span>

