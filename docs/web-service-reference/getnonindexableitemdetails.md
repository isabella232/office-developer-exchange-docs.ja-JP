---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: GetNonIndexableItemDetails 要素は、nonindexable の項目の詳細を取得する要求を指定します。
ms.openlocfilehash: 0aeda85973aa78eff240a017db58ffb57fc0de06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760792"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="29f59-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="29f59-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="29f59-104">**GetNonIndexableItemDetails**要素は、nonindexable の項目の詳細を取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="29f59-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="29f59-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="29f59-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29f59-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="29f59-106">Attributes and elements</span></span>

<span data-ttu-id="29f59-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29f59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29f59-108">属性</span><span class="sxs-lookup"><span data-stu-id="29f59-108">Attributes</span></span>

<span data-ttu-id="29f59-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29f59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29f59-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29f59-110">Child elements</span></span>

|<span data-ttu-id="29f59-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="29f59-111">**Element**</span></span>|<span data-ttu-id="29f59-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="29f59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29f59-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="29f59-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="29f59-114">**メールボックス**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="29f59-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="29f59-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="29f59-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="29f59-116">検索結果の 1 つのページに返される項目の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29f59-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="29f59-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="29f59-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="29f59-118">ページ アイテムへの参照を指定します。</span><span class="sxs-lookup"><span data-stu-id="29f59-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="29f59-119">PageDirection</span><span class="sxs-lookup"><span data-stu-id="29f59-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="29f59-120">検索結果の改ページ調整の方向が含まれています。</span><span class="sxs-lookup"><span data-stu-id="29f59-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29f59-121">親要素</span><span class="sxs-lookup"><span data-stu-id="29f59-121">Parent elements</span></span>

<span data-ttu-id="29f59-122">なし。</span><span class="sxs-lookup"><span data-stu-id="29f59-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29f59-123">備考</span><span class="sxs-lookup"><span data-stu-id="29f59-123">Remarks</span></span>

<span data-ttu-id="29f59-124">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29f59-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="29f59-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="29f59-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29f59-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="29f59-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29f59-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="29f59-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29f59-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29f59-128">Schema Name</span></span>  <br/> |<span data-ttu-id="29f59-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="29f59-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="29f59-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29f59-130">Validation File</span></span>  <br/> |<span data-ttu-id="29f59-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29f59-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29f59-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="29f59-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="29f59-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="29f59-133">See also</span></span>



- [<span data-ttu-id="29f59-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="29f59-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

