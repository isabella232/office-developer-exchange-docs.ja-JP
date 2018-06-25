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
description: DistinguishedGroupBy 要素は、FindItem クエリの標準的なグループ化を提供します。
ms.openlocfilehash: 0635366447675bf28dedf3af4f7d76094ee5e0a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760129"
---
# <a name="distinguishedgroupby"></a><span data-ttu-id="cb8e6-103">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="cb8e6-103">DistinguishedGroupBy</span></span>

<span data-ttu-id="cb8e6-104">**DistinguishedGroupBy**要素は、FindItem クエリの標準的なグループ化を提供します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-104">The **DistinguishedGroupBy** element provides standard groupings for FindItem queries.</span></span> 
  
- [<span data-ttu-id="cb8e6-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="cb8e6-105">FindItem</span></span>](finditem.md) 
- [<span data-ttu-id="cb8e6-106">DistinguishedGroupBy</span><span class="sxs-lookup"><span data-stu-id="cb8e6-106">DistinguishedGroupBy</span></span>](distinguishedgroupby.md)
  
```xml
<DistinguishedGroupBy>
   <StandardGroupBy/>
</DistinguishedGroupBy>
```

 <span data-ttu-id="cb8e6-107">**DistinguishedGroupByType**</span><span class="sxs-lookup"><span data-stu-id="cb8e6-107">**DistinguishedGroupByType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb8e6-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cb8e6-108">Attributes and elements</span></span>

<span data-ttu-id="cb8e6-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb8e6-110">属性</span><span class="sxs-lookup"><span data-stu-id="cb8e6-110">Attributes</span></span>

<span data-ttu-id="cb8e6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb8e6-112">子要素</span><span class="sxs-lookup"><span data-stu-id="cb8e6-112">Child elements</span></span>

|<span data-ttu-id="cb8e6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb8e6-113">**Element**</span></span>|<span data-ttu-id="cb8e6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb8e6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb8e6-115">StandardGroupBy</span><span class="sxs-lookup"><span data-stu-id="cb8e6-115">StandardGroupBy</span></span>](standardgroupby.md) <br/> |<span data-ttu-id="cb8e6-116">標準のグループ化と集計のグループ化された FindItem 操作のメカニズムを表します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-116">Represents the standard grouping and aggregating mechanisms for a grouped FindItem operation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb8e6-117">親要素</span><span class="sxs-lookup"><span data-stu-id="cb8e6-117">Parent elements</span></span>

|<span data-ttu-id="cb8e6-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb8e6-118">**Element**</span></span>|<span data-ttu-id="cb8e6-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb8e6-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb8e6-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="cb8e6-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="cb8e6-121">メールボックス内のアイテムを検索するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-121">Defines a request to find items in a mailbox.</span></span><br/><br/><span data-ttu-id="cb8e6-122">この要素への XPath 式は、次のようにします。`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="cb8e6-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb8e6-123">備考</span><span class="sxs-lookup"><span data-stu-id="cb8e6-123">Remarks</span></span>

<span data-ttu-id="cb8e6-124">FindItem 操作に**DistinguishedGroupBy**要素を追加することがグループ化されたときの結果でなければなりませんバックアップとグループ化の要件を満たす標準的なグループの 1 つとします。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-124">The **DistinguishedGroupBy** element can be added to a FindItem operation when the results must come backed grouped and when one of the standard groups meets the grouping requirements.</span></span> <span data-ttu-id="cb8e6-125">**DistinguishedGroupBy**要素も指定しない場合、 [GroupBy](groupby.md)要素は、結果が返される FindItem グループ化を解除します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-125">If neither the **DistinguishedGroupBy** element nor the [GroupBy](groupby.md) element is specified, FindItem results will come back ungrouped.</span></span> 
  
<span data-ttu-id="cb8e6-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb8e6-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="cb8e6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb8e6-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="cb8e6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb8e6-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cb8e6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="cb8e6-130">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cb8e6-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb8e6-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cb8e6-131">Validation File</span></span>  <br/> |<span data-ttu-id="cb8e6-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cb8e6-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb8e6-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cb8e6-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb8e6-134">False</span><span class="sxs-lookup"><span data-stu-id="cb8e6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb8e6-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb8e6-135">See also</span></span>

- <span data-ttu-id="cb8e6-136">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="cb8e6-136">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="cb8e6-137">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="cb8e6-137">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

