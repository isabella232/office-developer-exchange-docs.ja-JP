---
title: StandardGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardGroupBy
api_type:
- schema
ms.assetid: 04a84f71-b7eb-44dc-ac2c-ed504b52c463
description: StandardGroupBy 要素は、標準のグループ化と集計のグループ化された FindItem 操作のメカニズムを表します。
ms.openlocfilehash: 8e2ec72a79ebafc2e5757d6dcebb27c0c53ec0b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833542"
---
# <a name="standardgroupby"></a><span data-ttu-id="fcd1e-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="fcd1e-103">StandardGroupBy</span></span>

<span data-ttu-id="fcd1e-104">**StandardGroupBy**要素は、標準のグループ化と集計のグループ化された FindItem 操作のメカニズムを表します。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="fcd1e-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="fcd1e-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="fcd1e-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="fcd1e-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="fcd1e-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="fcd1e-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="fcd1e-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="fcd1e-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fcd1e-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fcd1e-109">Attributes and elements</span></span>

<span data-ttu-id="fcd1e-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fcd1e-111">属性</span><span class="sxs-lookup"><span data-stu-id="fcd1e-111">Attributes</span></span>

<span data-ttu-id="fcd1e-112">なし。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fcd1e-113">子要素</span><span class="sxs-lookup"><span data-stu-id="fcd1e-113">Child elements</span></span>

<span data-ttu-id="fcd1e-114">なし。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fcd1e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fcd1e-115">Parent elements</span></span>

|<span data-ttu-id="fcd1e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="fcd1e-116">**Element**</span></span>|<span data-ttu-id="fcd1e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="fcd1e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fcd1e-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="fcd1e-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="fcd1e-119">FindItem クエリの標準的なグループ化を提供します。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fcd1e-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fcd1e-120">Text value</span></span>

<span data-ttu-id="fcd1e-121">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-121">A text value is required.</span></span> <span data-ttu-id="fcd1e-122">**ConversationTopic**をこの要素のために使用できる唯一の値には。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="fcd1e-123">メッセージ: ConversationTopic および集計アイテム: DateTimeReceived (最大) を別のグループを**ConversationTopic** 。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="fcd1e-124">集計の詳細については、 [AggregateOn](aggregateon.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fcd1e-125">備考</span><span class="sxs-lookup"><span data-stu-id="fcd1e-125">Remarks</span></span>

<span data-ttu-id="fcd1e-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fcd1e-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="fcd1e-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fcd1e-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="fcd1e-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fcd1e-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fcd1e-129">Schema Name</span></span>  <br/> |<span data-ttu-id="fcd1e-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fcd1e-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="fcd1e-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fcd1e-131">Validation File</span></span>  <br/> |<span data-ttu-id="fcd1e-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fcd1e-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fcd1e-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fcd1e-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="fcd1e-134">False</span><span class="sxs-lookup"><span data-stu-id="fcd1e-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fcd1e-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="fcd1e-135">See also</span></span>



<span data-ttu-id="fcd1e-136">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="fcd1e-136">[FindItem operation](finditem-operation.md)</span></span>
  
[<span data-ttu-id="fcd1e-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="fcd1e-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="fcd1e-138">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="fcd1e-138">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

