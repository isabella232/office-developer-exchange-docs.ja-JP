---
title: ReferenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: ReferenceItemId 要素は、応答オブジェクトを参照する項目を識別します。
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833032"
---
# <a name="referenceitemid"></a><span data-ttu-id="8fed1-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="8fed1-103">ReferenceItemId</span></span>

<span data-ttu-id="8fed1-104">**ReferenceItemId**要素は、応答オブジェクトを参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="8fed1-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="8fed1-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fed1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8fed1-106">Attributes and elements</span></span>

<span data-ttu-id="8fed1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fed1-108">属性</span><span class="sxs-lookup"><span data-stu-id="8fed1-108">Attributes</span></span>

|<span data-ttu-id="8fed1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8fed1-109">**Attribute**</span></span>|<span data-ttu-id="8fed1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8fed1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8fed1-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="8fed1-111">**Id**</span></span> <br/> |<span data-ttu-id="8fed1-112">Exchange ストア内の特定の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="8fed1-113">**変更キー**</span><span class="sxs-lookup"><span data-stu-id="8fed1-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="8fed1-114">アイテムの特定のバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8fed1-115">子要素</span><span class="sxs-lookup"><span data-stu-id="8fed1-115">Child elements</span></span>

<span data-ttu-id="8fed1-116">なし。</span><span class="sxs-lookup"><span data-stu-id="8fed1-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fed1-117">親要素</span><span class="sxs-lookup"><span data-stu-id="8fed1-117">Parent elements</span></span>

|<span data-ttu-id="8fed1-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="8fed1-118">**Element**</span></span>|<span data-ttu-id="8fed1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8fed1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fed1-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="8fed1-121">会議出席依頼、承諾の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-122">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="8fed1-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="8fed1-123">共有への招待の承諾、返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="8fed1-125">会議をキャンセルするために使用される応答オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="8fed1-127">会議出席依頼を辞退の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-128">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="8fed1-129">受信者に転送するのには、Exchange ストアの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fed1-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="8fed1-131">Exchange ストアから項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-132">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="8fed1-133">Exchange ストア内のアイテムの識別されたすべての受信者への返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fed1-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="8fed1-135">Exchange ストア内のアイテムの作成者に返信が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8fed1-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="8fed1-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="8fed1-137">読み取り受信確認の要求に応答するために使用します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="8fed1-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="8fed1-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="8fed1-139">仮の予定を表しますが、会議出席依頼に返信します。</span><span class="sxs-lookup"><span data-stu-id="8fed1-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8fed1-140">備考</span><span class="sxs-lookup"><span data-stu-id="8fed1-140">Remarks</span></span>

<span data-ttu-id="8fed1-141">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8fed1-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fed1-142">要素情報</span><span class="sxs-lookup"><span data-stu-id="8fed1-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fed1-143">名前空間</span><span class="sxs-lookup"><span data-stu-id="8fed1-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fed1-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8fed1-144">Schema Name</span></span>  <br/> |<span data-ttu-id="8fed1-145">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8fed1-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fed1-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8fed1-146">Validation File</span></span>  <br/> |<span data-ttu-id="8fed1-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fed1-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fed1-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8fed1-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fed1-149">False</span><span class="sxs-lookup"><span data-stu-id="8fed1-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fed1-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="8fed1-150">See also</span></span>



- [<span data-ttu-id="8fed1-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8fed1-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

