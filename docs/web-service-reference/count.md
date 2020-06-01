---
title: カウント
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
description: Count 要素には、UpdateItem 操作応答の競合の数が含まれています。
ms.openlocfilehash: a43896a1b8b6a9d96ab02afe64f9e553639e478e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466760"
---
# <a name="count"></a><span data-ttu-id="75303-103">カウント</span><span class="sxs-lookup"><span data-stu-id="75303-103">Count</span></span>

<span data-ttu-id="75303-104">[Count](count.md)要素には、 [updateitem 操作](updateitem-operation.md)応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="75303-104">The [Count](count.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="75303-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="75303-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="75303-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="75303-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="75303-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="75303-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="75303-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="75303-108">ConflictResults</span></span>](conflictresults.md)
  
[<span data-ttu-id="75303-109">Count</span><span class="sxs-lookup"><span data-stu-id="75303-109">Count</span></span>](count.md)
  
```xml
<Count/>
```

 <span data-ttu-id="75303-110">**int**</span><span class="sxs-lookup"><span data-stu-id="75303-110">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75303-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="75303-111">Attributes and elements</span></span>

<span data-ttu-id="75303-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="75303-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75303-113">属性</span><span class="sxs-lookup"><span data-stu-id="75303-113">Attributes</span></span>

<span data-ttu-id="75303-114">なし。</span><span class="sxs-lookup"><span data-stu-id="75303-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75303-115">子要素</span><span class="sxs-lookup"><span data-stu-id="75303-115">Child elements</span></span>

<span data-ttu-id="75303-116">なし。</span><span class="sxs-lookup"><span data-stu-id="75303-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75303-117">親要素</span><span class="sxs-lookup"><span data-stu-id="75303-117">Parent elements</span></span>

|<span data-ttu-id="75303-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="75303-118">**Element**</span></span>|<span data-ttu-id="75303-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="75303-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75303-120">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="75303-120">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="75303-121">[Updateitem 操作](updateitem-operation.md)応答の競合の数を格納します。</span><span class="sxs-lookup"><span data-stu-id="75303-121">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75303-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="75303-122">Text value</span></span>

<span data-ttu-id="75303-123">テキスト値は、 [Updateitem 操作](updateitem-operation.md)応答の競合の数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="75303-123">The text value is an integer that represents the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75303-124">注釈</span><span class="sxs-lookup"><span data-stu-id="75303-124">Remarks</span></span>

<span data-ttu-id="75303-125">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="75303-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75303-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="75303-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75303-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="75303-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75303-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="75303-128">Schema Name</span></span>  <br/> |<span data-ttu-id="75303-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="75303-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="75303-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="75303-130">Validation File</span></span>  <br/> |<span data-ttu-id="75303-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="75303-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75303-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="75303-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="75303-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="75303-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75303-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="75303-134">See also</span></span>



<span data-ttu-id="75303-135">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75303-135">[UpdateItem operation](updateitem-operation.md)</span></span>
  
 <span data-ttu-id="75303-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="75303-136">**ConflictResultsType**</span></span>

