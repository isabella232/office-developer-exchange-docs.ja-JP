---
title: データの個数
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Count
api_type:
- schema
ms.assetid: 68314b4a-1e17-4e21-9c2e-224d70ef7a32
description: 数の要素には、競合 UpdateItem 操作の応答の数が含まれています。
ms.openlocfilehash: 15cea49eb250336cdc6b7d551d53951aff1372c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759788"
---
# <a name="count"></a><span data-ttu-id="e60d9-103">データの個数</span><span class="sxs-lookup"><span data-stu-id="e60d9-103">Count</span></span>

<span data-ttu-id="e60d9-104">[数](count.md)の要素には、競合[UpdateItem 操作](updateitem-operation.md)の応答の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e60d9-104">The [Count](count.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="e60d9-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e60d9-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="e60d9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e60d9-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="e60d9-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e60d9-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="e60d9-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="e60d9-108">ConflictResults</span></span>](conflictresults.md)
  
[<span data-ttu-id="e60d9-109">Count</span><span class="sxs-lookup"><span data-stu-id="e60d9-109">Count</span></span>](count.md)
  
```xml
<Count/>
```

 <span data-ttu-id="e60d9-110">**int**</span><span class="sxs-lookup"><span data-stu-id="e60d9-110">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e60d9-111">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e60d9-111">Attributes and elements</span></span>

<span data-ttu-id="e60d9-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e60d9-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e60d9-113">属性</span><span class="sxs-lookup"><span data-stu-id="e60d9-113">Attributes</span></span>

<span data-ttu-id="e60d9-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e60d9-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e60d9-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e60d9-115">Child elements</span></span>

<span data-ttu-id="e60d9-116">なし。</span><span class="sxs-lookup"><span data-stu-id="e60d9-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e60d9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e60d9-117">Parent elements</span></span>

|<span data-ttu-id="e60d9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="e60d9-118">**Element**</span></span>|<span data-ttu-id="e60d9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="e60d9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e60d9-120">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="e60d9-120">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="e60d9-121">[UpdateItem 操作](updateitem-operation.md)の応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e60d9-121">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e60d9-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e60d9-122">Text value</span></span>

<span data-ttu-id="e60d9-123">テキスト値は、競合[UpdateItem 操作](updateitem-operation.md)の応答の数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="e60d9-123">The text value is an integer that represents the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e60d9-124">備考</span><span class="sxs-lookup"><span data-stu-id="e60d9-124">Remarks</span></span>

<span data-ttu-id="e60d9-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e60d9-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e60d9-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="e60d9-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e60d9-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="e60d9-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e60d9-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e60d9-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e60d9-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e60d9-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="e60d9-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e60d9-130">Validation File</span></span>  <br/> |<span data-ttu-id="e60d9-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e60d9-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e60d9-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e60d9-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e60d9-133">False</span><span class="sxs-lookup"><span data-stu-id="e60d9-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e60d9-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e60d9-134">See also</span></span>



<span data-ttu-id="e60d9-135">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e60d9-135">[UpdateItem operation](updateitem-operation.md)</span></span>
  
 <span data-ttu-id="e60d9-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="e60d9-136">**ConflictResultsType**</span></span>

