---
title: DLExpansion
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
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760141"
---
# <a name="dlexpansion"></a><span data-ttu-id="469e6-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="469e6-103">DLExpansion</span></span>

<span data-ttu-id="469e6-104">**DLExpansion**要素には、配布リストに含まれているメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="469e6-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="469e6-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="469e6-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="469e6-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="469e6-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="469e6-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="469e6-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="469e6-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="469e6-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="469e6-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="469e6-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="469e6-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="469e6-110">Attributes and elements</span></span>

<span data-ttu-id="469e6-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="469e6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="469e6-112">属性</span><span class="sxs-lookup"><span data-stu-id="469e6-112">Attributes</span></span>

|<span data-ttu-id="469e6-113">**属性**</span><span class="sxs-lookup"><span data-stu-id="469e6-113">**Attribute**</span></span>|<span data-ttu-id="469e6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="469e6-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="469e6-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="469e6-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="469e6-116">次に、インデックス付きページング ビューを使用しているときに次の要求に使用するインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="469e6-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="469e6-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="469e6-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="469e6-118">分数のページ ビューを使用しているときに、次の要求に使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="469e6-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="469e6-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="469e6-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="469e6-120">分母分数のページ ビューを使用しているときに、次の要求に使用するを表します。</span><span class="sxs-lookup"><span data-stu-id="469e6-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="469e6-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="469e6-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="469e6-122">現在の結果では、追加のページングが必要ないように、クエリの最後の項目が含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="469e6-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="469e6-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="469e6-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="469e6-124">ビュー内の項目の合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="469e6-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="469e6-125">子要素</span><span class="sxs-lookup"><span data-stu-id="469e6-125">Child elements</span></span>

|<span data-ttu-id="469e6-126">**要素**</span><span class="sxs-lookup"><span data-stu-id="469e6-126">**Element**</span></span>|<span data-ttu-id="469e6-127">**説明**</span><span class="sxs-lookup"><span data-stu-id="469e6-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="469e6-128">メールボックス</span><span class="sxs-lookup"><span data-stu-id="469e6-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="469e6-129">メールが有効な Active Directory ディレクトリ サービス オブジェクトを識別します。</span><span class="sxs-lookup"><span data-stu-id="469e6-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="469e6-130">親要素</span><span class="sxs-lookup"><span data-stu-id="469e6-130">Parent elements</span></span>

|<span data-ttu-id="469e6-131">**要素**</span><span class="sxs-lookup"><span data-stu-id="469e6-131">**Element**</span></span>|<span data-ttu-id="469e6-132">**説明**</span><span class="sxs-lookup"><span data-stu-id="469e6-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="469e6-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="469e6-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="469e6-134">状態および 1 つの ExpandDL 要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="469e6-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="469e6-135">備考</span><span class="sxs-lookup"><span data-stu-id="469e6-135">Remarks</span></span>

<span data-ttu-id="469e6-136">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="469e6-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="469e6-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="469e6-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="469e6-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="469e6-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="469e6-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="469e6-139">Schema Name</span></span>  <br/> |<span data-ttu-id="469e6-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="469e6-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="469e6-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="469e6-141">Validation File</span></span>  <br/> |<span data-ttu-id="469e6-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="469e6-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="469e6-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="469e6-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="469e6-144">False</span><span class="sxs-lookup"><span data-stu-id="469e6-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="469e6-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="469e6-145">See also</span></span>

- [<span data-ttu-id="469e6-146">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="469e6-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="469e6-147">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="469e6-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- <span data-ttu-id="469e6-148">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="469e6-148">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>

