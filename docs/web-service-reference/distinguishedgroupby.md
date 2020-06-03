---
title: DistinguishedGroupBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedGroupBy
api_type:
- schema
ms.assetid: 6ff3ac48-02ba-40ec-a71b-c401bb2b127c
description: DistinguishedGroupBy 要素は、FindItem クエリの標準的なグループを提供します。
ms.openlocfilehash: 004613d55419a19f69e960203ae13d8d906b74c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463140"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="1c2aa-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="1c2aa-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="1c2aa-104">**DistinguishedGroupBy**要素は、FindItem クエリの標準的なグループを提供します。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="1c2aa-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="1c2aa-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="1c2aa-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="1c2aa-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="1c2aa-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="1c2aa-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c2aa-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1c2aa-108">Attributes and elements</span></span>

<span data-ttu-id="1c2aa-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c2aa-110">属性</span><span class="sxs-lookup"><span data-stu-id="1c2aa-110">Attributes</span></span>

<span data-ttu-id="1c2aa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c2aa-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1c2aa-112">Child elements</span></span>

|<span data-ttu-id="1c2aa-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="1c2aa-113">**Element**</span></span>|<span data-ttu-id="1c2aa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c2aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c2aa-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="1c2aa-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="1c2aa-116">グループ化された FindItem 操作の標準のグループ化および集約メカニズムを表します。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c2aa-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1c2aa-117">Parent elements</span></span>

|<span data-ttu-id="1c2aa-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c2aa-118">**Element**</span></span>|<span data-ttu-id="1c2aa-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c2aa-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c2aa-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="1c2aa-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="1c2aa-121">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="1c2aa-122">この要素の XPath 式を次に示します。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="1c2aa-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c2aa-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1c2aa-123">Remarks</span></span>

<span data-ttu-id="1c2aa-124">**DistinguishedGroupBy**要素は、結果がグループ化され、グループの要件を満たしている場合に、その結果がグループ化されている必要があるときに、FindItem 操作に追加できます。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="1c2aa-125">**DistinguishedGroupBy**要素も[GroupBy](groupby.md)要素も指定されていない場合、FindItem 結果はグループ解除されます。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="1c2aa-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="1c2aa-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c2aa-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1c2aa-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c2aa-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c2aa-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1c2aa-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1c2aa-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1c2aa-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1c2aa-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1c2aa-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1c2aa-131">Validation File</span></span>  <br/> |<span data-ttu-id="1c2aa-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1c2aa-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1c2aa-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1c2aa-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c2aa-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="1c2aa-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c2aa-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c2aa-135">See also</span></span>

- [<span data-ttu-id="1c2aa-136">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="1c2aa-136">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="1c2aa-137">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="1c2aa-137">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

