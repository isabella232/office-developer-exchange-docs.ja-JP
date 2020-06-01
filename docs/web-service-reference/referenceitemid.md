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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457229"
---
# <a name="referenceitemid"></a><span data-ttu-id="2f064-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="2f064-103">ReferenceItemId</span></span>

<span data-ttu-id="2f064-104">**Referenceitemid**要素は、response オブジェクトが参照する項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="2f064-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="2f064-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="2f064-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f064-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2f064-106">Attributes and elements</span></span>

<span data-ttu-id="2f064-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2f064-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f064-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f064-108">Attributes</span></span>

|<span data-ttu-id="2f064-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2f064-109">**Attribute**</span></span>|<span data-ttu-id="2f064-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f064-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2f064-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="2f064-111">**Id**</span></span> <br/> |<span data-ttu-id="2f064-112">Exchange ストア内の特定のアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f064-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="2f064-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="2f064-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="2f064-114">特定のバージョンのアイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="2f064-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2f064-115">子要素</span><span class="sxs-lookup"><span data-stu-id="2f064-115">Child elements</span></span>

<span data-ttu-id="2f064-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2f064-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f064-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2f064-117">Parent elements</span></span>

|<span data-ttu-id="2f064-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2f064-118">**Element**</span></span>|<span data-ttu-id="2f064-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f064-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f064-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="2f064-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="2f064-121">会議出席依頼への返信を承諾するかを表します。</span><span class="sxs-lookup"><span data-stu-id="2f064-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2f064-122">AcceptSharingInvitation 状</span><span class="sxs-lookup"><span data-stu-id="2f064-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="2f064-123">共有への招待への返信を受け付けるかを表します。</span><span class="sxs-lookup"><span data-stu-id="2f064-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="2f064-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="2f064-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="2f064-125">会議の取り消しに使用される response オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="2f064-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="2f064-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="2f064-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="2f064-127">会議出席依頼への返信を拒否することを表します。</span><span class="sxs-lookup"><span data-stu-id="2f064-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="2f064-128">Forwarditem と</span><span class="sxs-lookup"><span data-stu-id="2f064-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="2f064-129">受信者に転送するための Exchange ストアアイテムが保存されています。</span><span class="sxs-lookup"><span data-stu-id="2f064-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="2f064-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="2f064-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="2f064-131">Exchange ストアからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="2f064-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f064-132">Replyalltoitem と</span><span class="sxs-lookup"><span data-stu-id="2f064-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="2f064-133">Exchange ストア内のアイテムの特定の受信者全員への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="2f064-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f064-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2f064-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="2f064-135">Exchange ストア内のアイテムの作成者への返信を含みます。</span><span class="sxs-lookup"><span data-stu-id="2f064-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2f064-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="2f064-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="2f064-137">開封確認メッセージ要求に応答するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="2f064-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="2f064-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="2f064-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="2f064-139">会議出席依頼に対する仮の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="2f064-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f064-140">注釈</span><span class="sxs-lookup"><span data-stu-id="2f064-140">Remarks</span></span>

<span data-ttu-id="2f064-141">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2f064-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f064-142">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2f064-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f064-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f064-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f064-144">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2f064-144">Schema Name</span></span>  <br/> |<span data-ttu-id="2f064-145">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2f064-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f064-146">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2f064-146">Validation File</span></span>  <br/> |<span data-ttu-id="2f064-147">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2f064-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f064-148">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2f064-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f064-149">正しくない</span><span class="sxs-lookup"><span data-stu-id="2f064-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f064-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="2f064-150">See also</span></span>



- [<span data-ttu-id="2f064-151">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2f064-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

