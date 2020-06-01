---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: NewBodyContent 要素は、メッセージの新しい本文の内容を表します。
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466858"
---
# <a name="newbodycontent"></a><span data-ttu-id="e0c50-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="e0c50-103">NewBodyContent</span></span>

<span data-ttu-id="e0c50-104">**Newbodycontent**要素は、メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="e0c50-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="e0c50-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0c50-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e0c50-106">Attributes and elements</span></span>

<span data-ttu-id="e0c50-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0c50-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0c50-108">Attributes</span></span>

|<span data-ttu-id="e0c50-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e0c50-109">**Attribute**</span></span>|<span data-ttu-id="e0c50-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0c50-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0c50-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="e0c50-111">**BodyType**</span></span> <br/> |<span data-ttu-id="e0c50-112">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="e0c50-113">BodyType 属性</span><span class="sxs-lookup"><span data-stu-id="e0c50-113">BodyType Attribute</span></span>

|<span data-ttu-id="e0c50-114">**値**</span><span class="sxs-lookup"><span data-stu-id="e0c50-114">**Value**</span></span>|<span data-ttu-id="e0c50-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0c50-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0c50-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="e0c50-116">**HTML**</span></span> <br/> |<span data-ttu-id="e0c50-117">すべての本文を HTML に変換します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="e0c50-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="e0c50-118">**Text**</span></span> <br/> |<span data-ttu-id="e0c50-119">すべての本文をテキスト形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e0c50-120">子要素</span><span class="sxs-lookup"><span data-stu-id="e0c50-120">Child elements</span></span>

<span data-ttu-id="e0c50-121">なし。</span><span class="sxs-lookup"><span data-stu-id="e0c50-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0c50-122">親要素</span><span class="sxs-lookup"><span data-stu-id="e0c50-122">Parent elements</span></span>

|<span data-ttu-id="e0c50-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="e0c50-123">**Element**</span></span>|<span data-ttu-id="e0c50-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0c50-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0c50-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="e0c50-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="e0c50-126">Exchange ストア内のアイテムの送信者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="e0c50-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e0c50-127">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="e0c50-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="e0c50-128">Exchange ストア内のアイテムの送信者および特定の受信者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="e0c50-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="e0c50-129">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="e0c50-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="e0c50-130">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="e0c50-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="e0c50-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="e0c50-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="e0c50-132">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e0c50-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="e0c50-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="e0c50-134">投稿アイテムへの返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="e0c50-134">Contains a reply to a post item.</span></span> <span data-ttu-id="e0c50-135">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e0c50-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e0c50-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e0c50-136">Text value</span></span>

<span data-ttu-id="e0c50-137">Text 値は、メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="e0c50-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0c50-138">注釈</span><span class="sxs-lookup"><span data-stu-id="e0c50-138">Remarks</span></span>

<span data-ttu-id="e0c50-139">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange サーバーの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e0c50-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0c50-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e0c50-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0c50-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="e0c50-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0c50-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e0c50-142">Schema Name</span></span>  <br/> |<span data-ttu-id="e0c50-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e0c50-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0c50-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e0c50-144">Validation File</span></span>  <br/> |<span data-ttu-id="e0c50-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e0c50-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0c50-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e0c50-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0c50-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="e0c50-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0c50-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="e0c50-148">See also</span></span>



- [<span data-ttu-id="e0c50-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e0c50-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

