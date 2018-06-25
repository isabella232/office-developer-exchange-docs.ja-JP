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
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832516"
---
# <a name="newbodycontent"></a><span data-ttu-id="1b89d-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="1b89d-103">NewBodyContent</span></span>

<span data-ttu-id="1b89d-104">**NewBodyContent**要素は、メッセージの新しい本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="1b89d-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="1b89d-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b89d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1b89d-106">Attributes and elements</span></span>

<span data-ttu-id="1b89d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b89d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b89d-108">Attributes</span></span>

|<span data-ttu-id="1b89d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1b89d-109">**Attribute**</span></span>|<span data-ttu-id="1b89d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1b89d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b89d-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="1b89d-111">**BodyType**</span></span> <br/> |<span data-ttu-id="1b89d-112">メッセージの実際の本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="1b89d-113">BodyType 属性</span><span class="sxs-lookup"><span data-stu-id="1b89d-113">BodyType Attribute</span></span>

|<span data-ttu-id="1b89d-114">**値**</span><span class="sxs-lookup"><span data-stu-id="1b89d-114">**Value**</span></span>|<span data-ttu-id="1b89d-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="1b89d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b89d-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="1b89d-116">**HTML**</span></span> <br/> |<span data-ttu-id="1b89d-117">すべての本文を HTML に変換します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="1b89d-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="1b89d-118">**Text**</span></span> <br/> |<span data-ttu-id="1b89d-119">すべての本文をテキスト形式に変換します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1b89d-120">子要素</span><span class="sxs-lookup"><span data-stu-id="1b89d-120">Child elements</span></span>

<span data-ttu-id="1b89d-121">なし。</span><span class="sxs-lookup"><span data-stu-id="1b89d-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b89d-122">親要素</span><span class="sxs-lookup"><span data-stu-id="1b89d-122">Parent elements</span></span>

|<span data-ttu-id="1b89d-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="1b89d-123">**Element**</span></span>|<span data-ttu-id="1b89d-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="1b89d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b89d-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="1b89d-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="1b89d-126">Exchange ストア内のアイテムの送信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b89d-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1b89d-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="1b89d-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="1b89d-128">Exchange ストア内のアイテムの識別されたすべての受信者と送信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b89d-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1b89d-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="1b89d-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="1b89d-130">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b89d-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="1b89d-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="1b89d-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="1b89d-132">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="1b89d-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="1b89d-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="1b89d-134">投稿アイテムへの返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b89d-134">Contains a reply to a post item.</span></span> <span data-ttu-id="1b89d-135">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1b89d-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b89d-136">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1b89d-136">Text value</span></span>

<span data-ttu-id="1b89d-137">テキスト値は、新しいメッセージの本文の内容を表します。</span><span class="sxs-lookup"><span data-stu-id="1b89d-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b89d-138">備考</span><span class="sxs-lookup"><span data-stu-id="1b89d-138">Remarks</span></span>

<span data-ttu-id="1b89d-139">EWS 仮想ディレクトリのクライアント アクセス サーバーの役割がインストールされている Exchange サーバーには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1b89d-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b89d-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="1b89d-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b89d-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="1b89d-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b89d-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1b89d-142">Schema Name</span></span>  <br/> |<span data-ttu-id="1b89d-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1b89d-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b89d-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1b89d-144">Validation File</span></span>  <br/> |<span data-ttu-id="1b89d-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1b89d-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b89d-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1b89d-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b89d-147">False</span><span class="sxs-lookup"><span data-stu-id="1b89d-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b89d-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="1b89d-148">See also</span></span>



- [<span data-ttu-id="1b89d-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1b89d-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

