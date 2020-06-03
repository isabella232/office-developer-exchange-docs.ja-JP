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
description: ReferenceItemId 要素は、response オブジェクトが参照する項目を識別します。
ms.openlocfilehash: 3b77d75de91af8ec8fb7ae2d507377d1d976febf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457229"
---
# <a name="referenceitemid"></a><span data-ttu-id="0c53b-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="0c53b-103">ReferenceItemId</span></span>

<span data-ttu-id="0c53b-104">**Referenceitemid**要素は、response オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="0c53b-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="0c53b-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c53b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0c53b-106">Attributes and elements</span></span>

<span data-ttu-id="0c53b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c53b-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c53b-108">Attributes</span></span>

|<span data-ttu-id="0c53b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="0c53b-109">**Attribute**</span></span>|<span data-ttu-id="0c53b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c53b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0c53b-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="0c53b-111">**Id**</span></span> <br/> |<span data-ttu-id="0c53b-112">Exchange ストア内の特定のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="0c53b-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="0c53b-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="0c53b-114">特定のバージョンのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0c53b-115">子要素</span><span class="sxs-lookup"><span data-stu-id="0c53b-115">Child elements</span></span>

<span data-ttu-id="0c53b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0c53b-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0c53b-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0c53b-117">Parent elements</span></span>

|<span data-ttu-id="0c53b-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="0c53b-118">**Element**</span></span>|<span data-ttu-id="0c53b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c53b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c53b-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0c53b-121">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-122">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="0c53b-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="0c53b-123">共有への招待への返信を受け付けるかを表します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0c53b-125">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0c53b-127">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-128">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="0c53b-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0c53b-129">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="0c53b-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="0c53b-131">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-132">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="0c53b-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0c53b-133">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="0c53b-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0c53b-135">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="0c53b-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="0c53b-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="0c53b-137">開封確認メッセージ要求に応答するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0c53b-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="0c53b-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0c53b-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0c53b-139">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0c53b-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c53b-140">注釈</span><span class="sxs-lookup"><span data-stu-id="0c53b-140">Remarks</span></span>

<span data-ttu-id="0c53b-141">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0c53b-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c53b-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0c53b-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c53b-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c53b-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c53b-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0c53b-144">Schema Name</span></span>  <br/> |<span data-ttu-id="0c53b-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0c53b-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c53b-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0c53b-146">Validation File</span></span>  <br/> |<span data-ttu-id="0c53b-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0c53b-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c53b-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0c53b-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c53b-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="0c53b-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c53b-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c53b-150">See also</span></span>



- [<span data-ttu-id="0c53b-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0c53b-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

