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
description: Groups 要素には、FindItem 操作要求で識別される検索および集約条件があるグループのコレクションが含まれています。
ms.openlocfilehash: 915d9dffd6d8cec1def6634e6b70642d563b5242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530790"
---
# <a name="groups"></a><span data-ttu-id="e9828-103">グループ</span><span class="sxs-lookup"><span data-stu-id="e9828-103">Groups</span></span>

<span data-ttu-id="e9828-104">**Groups**要素には、 [FindItem 操作](finditem-operation.md)要求で識別される検索および集約条件があるグループのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9828-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="e9828-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="e9828-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9828-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9828-106">Attributes and elements</span></span>

<span data-ttu-id="e9828-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9828-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9828-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9828-108">Attributes</span></span>

<span data-ttu-id="e9828-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e9828-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9828-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e9828-110">Child elements</span></span>

|<span data-ttu-id="e9828-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e9828-111">**Element**</span></span>|<span data-ttu-id="e9828-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9828-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9828-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="e9828-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="e9828-114">グループ化された[FindItem 操作](finditem-operation.md)呼び出しの結果であるアイテムのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9828-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9828-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e9828-115">Parent elements</span></span>

|<span data-ttu-id="e9828-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9828-116">**Element**</span></span>|<span data-ttu-id="e9828-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9828-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9828-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="e9828-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="e9828-119">[FindItem 操作](finditem-operation.md)操作の間に1つのルートフォルダーを検索した結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="e9828-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9828-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e9828-120">Remarks</span></span>

<span data-ttu-id="e9828-121">結果内の個別のグループごとに1つの[Groupeditems](groupeditems.md)インスタンスが発生します。</span><span class="sxs-lookup"><span data-stu-id="e9828-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="e9828-122">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="e9828-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9828-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9828-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9828-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9828-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9828-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9828-125">Schema name</span></span>  <br/> |<span data-ttu-id="e9828-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e9828-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9828-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9828-127">Validation file</span></span>  <br/> |<span data-ttu-id="e9828-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e9828-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9828-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9828-129">Can be empty</span></span>  <br/> |<span data-ttu-id="e9828-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="e9828-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9828-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9828-131">See also</span></span>



[<span data-ttu-id="e9828-132">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="e9828-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="e9828-133">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="e9828-133">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

