---
title: DLExpansion 展開
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: DLExpansion 要素には、配布リストに含まれているメールボックスの配列が含まれています。
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456998"
---
# <a name="dlexpansion"></a><span data-ttu-id="991f0-103">DLExpansion 展開</span><span class="sxs-lookup"><span data-stu-id="991f0-103">DLExpansion</span></span>

<span data-ttu-id="991f0-104">**Dlexpansion**要素には、配布リストに含まれているメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="991f0-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="991f0-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="991f0-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="991f0-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="991f0-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="991f0-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="991f0-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="991f0-108">DLExpansion 展開</span><span class="sxs-lookup"><span data-stu-id="991f0-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="991f0-109">**Arrayofdlの種類**</span><span class="sxs-lookup"><span data-stu-id="991f0-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="991f0-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="991f0-110">Attributes and elements</span></span>

<span data-ttu-id="991f0-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="991f0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="991f0-112">属性</span><span class="sxs-lookup"><span data-stu-id="991f0-112">Attributes</span></span>

|<span data-ttu-id="991f0-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="991f0-113">**Attribute**</span></span>|<span data-ttu-id="991f0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="991f0-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="991f0-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="991f0-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="991f0-116">インデックス付きのページビューを使用している場合に、次の要求に使用する必要がある次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="991f0-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="991f0-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="991f0-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="991f0-118">分数のページビューを使用しているときに、次の要求に対して使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="991f0-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="991f0-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="991f0-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="991f0-120">分数のページビューを使用しているときに、次の要求に対して使用する次の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="991f0-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="991f0-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="991f0-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="991f0-122">追加のページングを必要としないように、現在の結果にクエリの最後のアイテムが含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="991f0-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="991f0-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="991f0-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="991f0-124">ビュー内のアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="991f0-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="991f0-125">子要素</span><span class="sxs-lookup"><span data-stu-id="991f0-125">Child elements</span></span>

|<span data-ttu-id="991f0-126">**Element**</span><span class="sxs-lookup"><span data-stu-id="991f0-126">**Element**</span></span>|<span data-ttu-id="991f0-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="991f0-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991f0-128">メールボックス</span><span class="sxs-lookup"><span data-stu-id="991f0-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="991f0-129">メールが有効な Active Directory ディレクトリサービスオブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="991f0-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="991f0-130">親要素</span><span class="sxs-lookup"><span data-stu-id="991f0-130">Parent elements</span></span>

|<span data-ttu-id="991f0-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="991f0-131">**Element**</span></span>|<span data-ttu-id="991f0-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="991f0-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991f0-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="991f0-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="991f0-134">1つの ExpandDL 要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="991f0-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="991f0-135">注釈</span><span class="sxs-lookup"><span data-stu-id="991f0-135">Remarks</span></span>

<span data-ttu-id="991f0-136">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="991f0-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="991f0-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="991f0-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="991f0-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="991f0-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="991f0-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="991f0-139">Schema Name</span></span>  <br/> |<span data-ttu-id="991f0-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="991f0-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="991f0-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="991f0-141">Validation File</span></span>  <br/> |<span data-ttu-id="991f0-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="991f0-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="991f0-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="991f0-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="991f0-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="991f0-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="991f0-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="991f0-145">See also</span></span>

- [<span data-ttu-id="991f0-146">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="991f0-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="991f0-147">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="991f0-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="991f0-148">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="991f0-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

