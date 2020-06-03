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
description: StandardGroupBy 要素は、グループ化された FindItem 操作の標準のグループ化および集約メカニズムを表します。
ms.openlocfilehash: 3e135feba322979de3d66d5a45d423654ccc9100
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467558"
---
# <a name="standardgroupby"></a><span data-ttu-id="1cb3b-103">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="1cb3b-103">StandardGroupBy</span></span>

<span data-ttu-id="1cb3b-104">**Standardgroupby**要素は、グループ化された FindItem 操作の標準のグループ化および集約メカニズムを表します。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-104">The **StandardGroupBy** element represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span> 
  
[<span data-ttu-id="1cb3b-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="1cb3b-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="1cb3b-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="1cb3b-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
[<span data-ttu-id="1cb3b-107">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="1cb3b-107">StandardGroupBy</span></span>](standardgroupby.md)
  
```xml
<StandardGroupBy/>
```

 <span data-ttu-id="1cb3b-108">**StandardGroupByType**</span><span class="sxs-lookup"><span data-stu-id="1cb3b-108">**StandardGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cb3b-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1cb3b-109">Attributes and elements</span></span>

<span data-ttu-id="1cb3b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cb3b-111">属性</span><span class="sxs-lookup"><span data-stu-id="1cb3b-111">Attributes</span></span>

<span data-ttu-id="1cb3b-112">なし。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cb3b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="1cb3b-113">Child elements</span></span>

<span data-ttu-id="1cb3b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1cb3b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1cb3b-115">Parent elements</span></span>

|<span data-ttu-id="1cb3b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cb3b-116">**Element**</span></span>|<span data-ttu-id="1cb3b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cb3b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cb3b-118">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="1cb3b-118">DistinguishedGroupBy</span></span>](distinguishedgroupby.md) <br/> |<span data-ttu-id="1cb3b-119">FindItem クエリの標準的なグループを提供します。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-119">Provides standard groupings for FindItem queries.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1cb3b-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1cb3b-120">Text value</span></span>

<span data-ttu-id="1cb3b-121">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-121">A text value is required.</span></span> <span data-ttu-id="1cb3b-122">この要素に使用できる値は**ConversationTopic**のみです。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-122">The only value that can be used for this element is **ConversationTopic**.</span></span> <span data-ttu-id="1cb3b-123">**ConversationTopic**によってグループ化されたメッセージ: ConversationTopic およびアイテムの集計: DateTimeReceived (最大)。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-123">**ConversationTopic** groups by message:ConversationTopic and aggregates on item:DateTimeReceived (maximum).</span></span> <span data-ttu-id="1cb3b-124">集計の詳細については、「 [AggregateOn](aggregateon.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-124">For more information about aggregation, see [AggregateOn](aggregateon.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cb3b-125">注釈</span><span class="sxs-lookup"><span data-stu-id="1cb3b-125">Remarks</span></span>

<span data-ttu-id="1cb3b-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="1cb3b-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cb3b-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1cb3b-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cb3b-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="1cb3b-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1cb3b-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cb3b-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1cb3b-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1cb3b-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1cb3b-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cb3b-131">Validation File</span></span>  <br/> |<span data-ttu-id="1cb3b-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1cb3b-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1cb3b-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1cb3b-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cb3b-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="1cb3b-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cb3b-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cb3b-135">See also</span></span>



[<span data-ttu-id="1cb3b-136">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="1cb3b-136">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="1cb3b-137">FindItem</span><span class="sxs-lookup"><span data-stu-id="1cb3b-137">FindItem</span></span>](finditem.md)


[<span data-ttu-id="1cb3b-138">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="1cb3b-138">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

