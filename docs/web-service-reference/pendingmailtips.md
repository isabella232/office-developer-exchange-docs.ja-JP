---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: PendingMailTips 要素は、サーバーの処理のタイムアウト期間が経過する前にこの要素内のメール ヒントを評価できませんでしたを示します。
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="991ce-103">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="991ce-103">PendingMailTips</span></span>

<span data-ttu-id="991ce-104">**PendingMailTips**要素は、サーバーの処理のタイムアウト期間が経過する前にこの要素内のメール ヒントを評価できませんでしたを示します。</span><span class="sxs-lookup"><span data-stu-id="991ce-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="991ce-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="991ce-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="991ce-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="991ce-106">Attributes and elements</span></span>

<span data-ttu-id="991ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="991ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="991ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="991ce-108">Attributes</span></span>

<span data-ttu-id="991ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="991ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="991ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="991ce-110">Child elements</span></span>

<span data-ttu-id="991ce-111">なし。</span><span class="sxs-lookup"><span data-stu-id="991ce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="991ce-112">親要素</span><span class="sxs-lookup"><span data-stu-id="991ce-112">Parent elements</span></span>

|<span data-ttu-id="991ce-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="991ce-113">**Element**</span></span>|<span data-ttu-id="991ce-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="991ce-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="991ce-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="991ce-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="991ce-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="991ce-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="991ce-117">Text value</span></span>

<span data-ttu-id="991ce-118">次の表は、 **PendingMailTips**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="991ce-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="991ce-119">**値**</span><span class="sxs-lookup"><span data-stu-id="991ce-119">**Value**</span></span>|<span data-ttu-id="991ce-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="991ce-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="991ce-121">All</span><span class="sxs-lookup"><span data-stu-id="991ce-121">All</span></span>  <br/> |<span data-ttu-id="991ce-122">すべての利用可能なメール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="991ce-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="991ce-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="991ce-124">Office (OOF) メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="991ce-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="991ce-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="991ce-126">メールボックスがいっぱいの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="991ce-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="991ce-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="991ce-128">カスタム メール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="991ce-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="991ce-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="991ce-130">外部のメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="991ce-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="991ce-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="991ce-132">すべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="991ce-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="991ce-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="991ce-134">受信者が受け入れることができるメッセージの最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="991ce-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="991ce-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="991ce-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="991ce-136">配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="991ce-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="991ce-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="991ce-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="991ce-138">送信者のメッセージはモデレーターによって確認するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="991ce-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="991ce-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="991ce-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="991ce-140">受信者が有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="991ce-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="991ce-141">備考</span><span class="sxs-lookup"><span data-stu-id="991ce-141">Remarks</span></span>

<span data-ttu-id="991ce-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="991ce-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="991ce-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="991ce-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="991ce-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="991ce-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="991ce-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="991ce-145">Schema Name</span></span>  <br/> |<span data-ttu-id="991ce-146">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="991ce-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="991ce-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="991ce-147">Validation File</span></span>  <br/> |<span data-ttu-id="991ce-148">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="991ce-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="991ce-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="991ce-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="991ce-150">False</span><span class="sxs-lookup"><span data-stu-id="991ce-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="991ce-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="991ce-151">See also</span></span>



- [<span data-ttu-id="991ce-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="991ce-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

