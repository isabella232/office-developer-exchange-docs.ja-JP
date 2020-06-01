---
title: GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce3994c1-3bb4-4571-b026-34a6c5705410
description: GetNonIndexableItemDetails 要素は、インデックス付けされていないアイテムの詳細を取得するための要求を指定します。
ms.openlocfilehash: 1c04b4cd7a86183210be869973c9779188fa0adf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458601"
---
# <a name="getnonindexableitemdetails"></a><span data-ttu-id="1a56b-103">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="1a56b-103">GetNonIndexableItemDetails</span></span>

<span data-ttu-id="1a56b-104">**Getnonindexableitemdetails**要素は、インデックス付けされていないアイテムの詳細を取得するための要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a56b-104">The **GetNonIndexableItemDetails** element specifies a request to retrieve nonindexable item details.</span></span> 
  
```XML
<GetNonIndexableItemDetails>
    <Mailboxes/>
    <PageSize/>
    <PageItemReference/>
    <PageDirection/>
</GetNonIndexableItemDetails>
```

 <span data-ttu-id="1a56b-105">**GetNonIndexableItemDetailsType**</span><span class="sxs-lookup"><span data-stu-id="1a56b-105">**GetNonIndexableItemDetailsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a56b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1a56b-106">Attributes and elements</span></span>

<span data-ttu-id="1a56b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a56b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a56b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a56b-108">Attributes</span></span>

<span data-ttu-id="1a56b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a56b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a56b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a56b-110">Child elements</span></span>

|<span data-ttu-id="1a56b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1a56b-111">**Element**</span></span>|<span data-ttu-id="1a56b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a56b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a56b-113">メールボックス (NonEmptyArrayOfLegacyDNsType)</span><span class="sxs-lookup"><span data-stu-id="1a56b-113">Mailboxes (NonEmptyArrayOfLegacyDNsType)</span></span>](mailboxes-nonemptyarrayoflegacydnstype.md) <br/> |<span data-ttu-id="1a56b-114">**メールボックス**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a56b-114">Specifies an array of **Mailbox** elements.</span></span>  <br/> |
|[<span data-ttu-id="1a56b-115">PageSize</span><span class="sxs-lookup"><span data-stu-id="1a56b-115">PageSize</span></span>](pagesize.md) <br/> |<span data-ttu-id="1a56b-116">検索結果に対して単一のページで返されるアイテムの数を格納します。</span><span class="sxs-lookup"><span data-stu-id="1a56b-116">Contains the number of items to be returned in a single page for a search result.</span></span>  <br/> |
|[<span data-ttu-id="1a56b-117">PageItemReference</span><span class="sxs-lookup"><span data-stu-id="1a56b-117">PageItemReference</span></span>](pageitemreference.md) <br/> |<span data-ttu-id="1a56b-118">ページアイテムの参照を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a56b-118">Specifies the reference for a page item.</span></span>  <br/> |
|[<span data-ttu-id="1a56b-119">ページの方向</span><span class="sxs-lookup"><span data-stu-id="1a56b-119">PageDirection</span></span>](pagedirection.md) <br/> |<span data-ttu-id="1a56b-120">検索結果の改ページ位置の方向を含みます。</span><span class="sxs-lookup"><span data-stu-id="1a56b-120">Contains the direction for pagination in the search result.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a56b-121">親要素</span><span class="sxs-lookup"><span data-stu-id="1a56b-121">Parent elements</span></span>

<span data-ttu-id="1a56b-122">なし。</span><span class="sxs-lookup"><span data-stu-id="1a56b-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a56b-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1a56b-123">Remarks</span></span>

<span data-ttu-id="1a56b-124">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1a56b-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1a56b-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1a56b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a56b-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1a56b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a56b-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a56b-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a56b-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a56b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1a56b-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1a56b-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="1a56b-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a56b-130">Validation File</span></span>  <br/> |<span data-ttu-id="1a56b-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1a56b-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a56b-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1a56b-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1a56b-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a56b-133">See also</span></span>



- [<span data-ttu-id="1a56b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a56b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

