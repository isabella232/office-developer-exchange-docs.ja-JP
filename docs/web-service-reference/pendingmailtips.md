---
title: PendingMailTips ヒント
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
description: PendingMailTips ヒント要素は、サーバーの処理タイムアウトが経過する前に、この要素のメールヒントを評価できなかったことを示します。
ms.openlocfilehash: 715d68b367c3b7251c7406c10c1ec52dcd992a59
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529967"
---
# <a name="pendingmailtips"></a><span data-ttu-id="ed92c-103">PendingMailTips ヒント</span><span class="sxs-lookup"><span data-stu-id="ed92c-103">PendingMailTips</span></span>

<span data-ttu-id="ed92c-104">**Pendingmailtips**ヒント要素は、サーバーの処理タイムアウトが経過する前に、この要素のメールヒントを評価できなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="ed92c-105">**Mailヒントの種類**</span><span class="sxs-lookup"><span data-stu-id="ed92c-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed92c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ed92c-106">Attributes and elements</span></span>

<span data-ttu-id="ed92c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed92c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed92c-108">Attributes</span></span>

<span data-ttu-id="ed92c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ed92c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed92c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ed92c-110">Child elements</span></span>

<span data-ttu-id="ed92c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ed92c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed92c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ed92c-112">Parent elements</span></span>

|<span data-ttu-id="ed92c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ed92c-113">**Element**</span></span>|<span data-ttu-id="ed92c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed92c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed92c-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="ed92c-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ed92c-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed92c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ed92c-117">Text value</span></span>

<span data-ttu-id="ed92c-118">次の表に、 **Pendingmailtips ヒント**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="ed92c-119">**値**</span><span class="sxs-lookup"><span data-stu-id="ed92c-119">**Value**</span></span>|<span data-ttu-id="ed92c-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="ed92c-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed92c-121">すべて</span><span class="sxs-lookup"><span data-stu-id="ed92c-121">All</span></span>  <br/> |<span data-ttu-id="ed92c-122">利用可能なすべてのメールヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="ed92c-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="ed92c-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="ed92c-124">不在 (OOF) メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="ed92c-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="ed92c-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="ed92c-126">メールボックスがいっぱいになったときの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="ed92c-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="ed92c-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="ed92c-128">ユーザー設定のメールヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="ed92c-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ed92c-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="ed92c-130">外部メンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="ed92c-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ed92c-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="ed92c-132">すべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="ed92c-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="ed92c-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="ed92c-134">受信者が受け付けることができる最大メッセージサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="ed92c-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="ed92c-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="ed92c-136">配信の制限によって、送信者のメッセージが受信者に届かないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="ed92c-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="ed92c-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="ed92c-138">送信者のメッセージがモデレーターによって確認されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="ed92c-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="ed92c-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="ed92c-140">受信者が無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ed92c-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ed92c-141">注釈</span><span class="sxs-lookup"><span data-stu-id="ed92c-141">Remarks</span></span>

<span data-ttu-id="ed92c-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ed92c-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed92c-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ed92c-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed92c-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed92c-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed92c-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ed92c-145">Schema Name</span></span>  <br/> |<span data-ttu-id="ed92c-146">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ed92c-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed92c-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ed92c-147">Validation File</span></span>  <br/> |<span data-ttu-id="ed92c-148">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ed92c-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed92c-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ed92c-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed92c-150">正しくない</span><span class="sxs-lookup"><span data-stu-id="ed92c-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed92c-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="ed92c-151">See also</span></span>



- [<span data-ttu-id="ed92c-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ed92c-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

