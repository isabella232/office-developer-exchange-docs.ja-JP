---
title: 本文
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Body 要素は、アイテムの本文を指定します。
ms.openlocfilehash: a4803c0e5ac3b027396983a5524241590eac35f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759525"
---
# <a name="body"></a><span data-ttu-id="789f0-103">本文</span><span class="sxs-lookup"><span data-stu-id="789f0-103">Body</span></span>

<span data-ttu-id="789f0-104">**Body**要素は、アイテムの本文を指定します。</span><span class="sxs-lookup"><span data-stu-id="789f0-104">The **Body** element specifies the body of an item.</span></span> 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 <span data-ttu-id="789f0-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="789f0-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="789f0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="789f0-106">Attributes and elements</span></span>

<span data-ttu-id="789f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="789f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="789f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="789f0-108">Attributes</span></span>

|<span data-ttu-id="789f0-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="789f0-109">**Attribute**</span></span>|<span data-ttu-id="789f0-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="789f0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="789f0-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="789f0-111">BodyType</span></span>  <br/> |<span data-ttu-id="789f0-112">本文の種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="789f0-112">Specifies the type of the body.</span></span>  <br/> |
|<span data-ttu-id="789f0-113">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="789f0-113">IsTruncated</span></span>  <br/> |<span data-ttu-id="789f0-114">本文が切り詰められるかどうかを示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="789f0-114">Boolean value that indicates whether the body is truncated.</span></span>  <br/> |
   
#### <a name="bodytype"></a><span data-ttu-id="789f0-115">BodyType</span><span class="sxs-lookup"><span data-stu-id="789f0-115">BodyType</span></span>

|<span data-ttu-id="789f0-116">**値**</span><span class="sxs-lookup"><span data-stu-id="789f0-116">**Value**</span></span>|<span data-ttu-id="789f0-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="789f0-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="789f0-118">HTML</span><span class="sxs-lookup"><span data-stu-id="789f0-118">HTML</span></span>  <br/> |<span data-ttu-id="789f0-119">本文が html 形式でことを示します。</span><span class="sxs-lookup"><span data-stu-id="789f0-119">Indicates that the body is in HTML.</span></span>  <br/> |
|<span data-ttu-id="789f0-120">テキスト型 (Text)</span><span class="sxs-lookup"><span data-stu-id="789f0-120">Text</span></span>  <br/> |<span data-ttu-id="789f0-121">本文がテキストであることを示します。</span><span class="sxs-lookup"><span data-stu-id="789f0-121">Indicates that the body is in text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="789f0-122">子要素</span><span class="sxs-lookup"><span data-stu-id="789f0-122">Child elements</span></span>

<span data-ttu-id="789f0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="789f0-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="789f0-124">親要素</span><span class="sxs-lookup"><span data-stu-id="789f0-124">Parent elements</span></span>

|<span data-ttu-id="789f0-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="789f0-125">**Element**</span></span>|<span data-ttu-id="789f0-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="789f0-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="789f0-127">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="789f0-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="789f0-128">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="789f0-129">Contact</span><span class="sxs-lookup"><span data-stu-id="789f0-129">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="789f0-130">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-130">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="789f0-131">DistributionList</span><span class="sxs-lookup"><span data-stu-id="789f0-131">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="789f0-132">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-132">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="789f0-133">アイテム</span><span class="sxs-lookup"><span data-stu-id="789f0-133">Item</span></span>](item.md) <br/> |<span data-ttu-id="789f0-134">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-134">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="789f0-135">Message</span><span class="sxs-lookup"><span data-stu-id="789f0-135">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="789f0-136">Microsoft Exchange の電子メール メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-136">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="789f0-137">PostItem</span><span class="sxs-lookup"><span data-stu-id="789f0-137">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="789f0-138">Exchange ストア内の投稿アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-138">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="789f0-139">タスク</span><span class="sxs-lookup"><span data-stu-id="789f0-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="789f0-140">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="789f0-140">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="789f0-141">テキスト値</span><span class="sxs-lookup"><span data-stu-id="789f0-141">Text value</span></span>

<span data-ttu-id="789f0-142">**Body**要素のテキスト値は、アイテムの本文の内容です。</span><span class="sxs-lookup"><span data-stu-id="789f0-142">The text value of the **Body** element is the body content of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="789f0-143">備考</span><span class="sxs-lookup"><span data-stu-id="789f0-143">Remarks</span></span>

<span data-ttu-id="789f0-144">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="789f0-144">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="789f0-145">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="789f0-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="789f0-146">要素情報</span><span class="sxs-lookup"><span data-stu-id="789f0-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="789f0-147">名前空間</span><span class="sxs-lookup"><span data-stu-id="789f0-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="789f0-148">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="789f0-148">Schema Name</span></span>  <br/> |<span data-ttu-id="789f0-149">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="789f0-149">Type schema</span></span>  <br/> |
|<span data-ttu-id="789f0-150">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="789f0-150">Validation File</span></span>  <br/> |<span data-ttu-id="789f0-151">types.xsd</span><span class="sxs-lookup"><span data-stu-id="789f0-151">types.xsd</span></span>  <br/> |
|<span data-ttu-id="789f0-152">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="789f0-152">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="789f0-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="789f0-153">See also</span></span>



- [<span data-ttu-id="789f0-154">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="789f0-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

