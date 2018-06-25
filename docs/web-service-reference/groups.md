---
title: グループ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: グループ要素には、FindItem 操作の要求で指定されている検索と集計の基準で検出されたグループのコレクションが含まれています。
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831786"
---
# <a name="groups"></a><span data-ttu-id="57b08-103">グループ</span><span class="sxs-lookup"><span data-stu-id="57b08-103">Groups</span></span>

<span data-ttu-id="57b08-104">**グループ**要素には、 [FindItem 操作](finditem-operation.md)要求で指定されている検索と集計の基準で検出されたグループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57b08-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="57b08-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="57b08-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57b08-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57b08-106">Attributes and elements</span></span>

<span data-ttu-id="57b08-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57b08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57b08-108">属性</span><span class="sxs-lookup"><span data-stu-id="57b08-108">Attributes</span></span>

<span data-ttu-id="57b08-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57b08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57b08-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57b08-110">Child elements</span></span>

|<span data-ttu-id="57b08-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="57b08-111">**Element**</span></span>|<span data-ttu-id="57b08-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="57b08-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57b08-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="57b08-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="57b08-114">グループ化された[FindItem 操作](finditem-operation.md)の結果であるアイテムのコレクションを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="57b08-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57b08-115">親要素</span><span class="sxs-lookup"><span data-stu-id="57b08-115">Parent elements</span></span>

|<span data-ttu-id="57b08-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="57b08-116">**Element**</span></span>|<span data-ttu-id="57b08-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="57b08-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57b08-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="57b08-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="57b08-119">[FindItem 操作](finditem-operation.md)の処理中に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57b08-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57b08-120">備考</span><span class="sxs-lookup"><span data-stu-id="57b08-120">Remarks</span></span>

<span data-ttu-id="57b08-121">結果内の異なるグループごとに 1 つの[GroupedItems](groupeditems.md)インスタンスが発生します。</span><span class="sxs-lookup"><span data-stu-id="57b08-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="57b08-122">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="57b08-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57b08-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="57b08-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57b08-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="57b08-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57b08-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57b08-125">Schema name</span></span>  <br/> |<span data-ttu-id="57b08-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="57b08-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="57b08-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57b08-127">Validation file</span></span>  <br/> |<span data-ttu-id="57b08-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57b08-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57b08-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="57b08-129">Can be empty</span></span>  <br/> |<span data-ttu-id="57b08-130">False</span><span class="sxs-lookup"><span data-stu-id="57b08-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57b08-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="57b08-131">See also</span></span>



<span data-ttu-id="57b08-132">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="57b08-132">[FindItem operation](finditem-operation.md)</span></span>


[<span data-ttu-id="57b08-133">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="57b08-133">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

