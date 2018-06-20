---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: MailTipsRequested 要素には、サービスから要求されたメール ヒントの種類が含まれています。
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832348"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="782c6-103">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="782c6-103">MailTipsRequested</span></span>

<span data-ttu-id="782c6-104">**MailTipsRequested**要素には、サービスから要求されたメール ヒントの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="782c6-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="782c6-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="782c6-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="782c6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="782c6-106">Attributes and elements</span></span>

<span data-ttu-id="782c6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="782c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="782c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="782c6-108">Attributes</span></span>

<span data-ttu-id="782c6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="782c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="782c6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="782c6-110">Child elements</span></span>

<span data-ttu-id="782c6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="782c6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="782c6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="782c6-112">Parent elements</span></span>

|<span data-ttu-id="782c6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="782c6-113">**Element**</span></span>|<span data-ttu-id="782c6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="782c6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="782c6-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="782c6-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="782c6-116">受信者とメール ヒントの種類を取得するのにが含まれています。</span><span class="sxs-lookup"><span data-stu-id="782c6-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="782c6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="782c6-117">Text value</span></span>

<span data-ttu-id="782c6-118">次の表は、 **MailTipsRequested**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="782c6-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="782c6-119">**値**</span><span class="sxs-lookup"><span data-stu-id="782c6-119">**Value**</span></span>|<span data-ttu-id="782c6-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="782c6-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="782c6-121">All</span><span class="sxs-lookup"><span data-stu-id="782c6-121">All</span></span>  <br/> |<span data-ttu-id="782c6-122">すべての利用可能なメール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="782c6-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="782c6-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="782c6-124">Office (OOF) メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="782c6-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="782c6-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="782c6-126">メールボックスがいっぱいの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="782c6-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="782c6-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="782c6-128">カスタム メール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="782c6-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="782c6-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="782c6-130">外部のメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="782c6-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="782c6-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="782c6-132">すべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="782c6-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="782c6-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="782c6-134">受信者が受け入れることができるメッセージの最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="782c6-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="782c6-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="782c6-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="782c6-136">配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="782c6-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="782c6-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="782c6-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="782c6-138">送信者のメッセージはモデレーターによって確認するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="782c6-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="782c6-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="782c6-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="782c6-140">受信者が有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="782c6-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="782c6-141">備考</span><span class="sxs-lookup"><span data-stu-id="782c6-141">Remarks</span></span>

<span data-ttu-id="782c6-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="782c6-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="782c6-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="782c6-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="782c6-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="782c6-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="782c6-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="782c6-145">Schema Name</span></span>  <br/> |<span data-ttu-id="782c6-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="782c6-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="782c6-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="782c6-147">Validation File</span></span>  <br/> |<span data-ttu-id="782c6-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="782c6-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="782c6-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="782c6-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="782c6-150">False</span><span class="sxs-lookup"><span data-stu-id="782c6-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="782c6-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="782c6-151">See also</span></span>



- [<span data-ttu-id="782c6-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="782c6-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

