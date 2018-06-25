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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832348"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="53038-103">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="53038-103">MailTipsRequested</span></span>

<span data-ttu-id="53038-104">**MailTipsRequested**要素には、サービスから要求されたメール ヒントの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="53038-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="53038-105">**MailTipTypes**</span><span class="sxs-lookup"><span data-stu-id="53038-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53038-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="53038-106">Attributes and elements</span></span>

<span data-ttu-id="53038-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="53038-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53038-108">属性</span><span class="sxs-lookup"><span data-stu-id="53038-108">Attributes</span></span>

<span data-ttu-id="53038-109">なし。</span><span class="sxs-lookup"><span data-stu-id="53038-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53038-110">子要素</span><span class="sxs-lookup"><span data-stu-id="53038-110">Child elements</span></span>

<span data-ttu-id="53038-111">なし。</span><span class="sxs-lookup"><span data-stu-id="53038-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53038-112">親要素</span><span class="sxs-lookup"><span data-stu-id="53038-112">Parent elements</span></span>

|<span data-ttu-id="53038-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="53038-113">**Element**</span></span>|<span data-ttu-id="53038-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="53038-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53038-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="53038-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="53038-116">受信者とメール ヒントの種類を取得するのにが含まれています。</span><span class="sxs-lookup"><span data-stu-id="53038-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53038-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="53038-117">Text value</span></span>

<span data-ttu-id="53038-118">次の表は、 **MailTipsRequested**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="53038-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="53038-119">**値**</span><span class="sxs-lookup"><span data-stu-id="53038-119">**Value**</span></span>|<span data-ttu-id="53038-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="53038-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="53038-121">All</span><span class="sxs-lookup"><span data-stu-id="53038-121">All</span></span>  <br/> |<span data-ttu-id="53038-122">すべての利用可能なメール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="53038-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="53038-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="53038-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="53038-124">Office (OOF) メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="53038-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="53038-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="53038-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="53038-126">メールボックスがいっぱいの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="53038-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="53038-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="53038-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="53038-128">カスタム メール ヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="53038-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="53038-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="53038-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="53038-130">外部のメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="53038-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="53038-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="53038-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="53038-132">すべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="53038-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="53038-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="53038-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="53038-134">受信者が受け入れることができるメッセージの最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="53038-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="53038-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="53038-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="53038-136">配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53038-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="53038-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="53038-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="53038-138">送信者のメッセージはモデレーターによって確認するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53038-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="53038-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="53038-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="53038-140">受信者が有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53038-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="53038-141">備考</span><span class="sxs-lookup"><span data-stu-id="53038-141">Remarks</span></span>

<span data-ttu-id="53038-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="53038-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="53038-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="53038-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53038-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="53038-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="53038-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="53038-145">Schema Name</span></span>  <br/> |<span data-ttu-id="53038-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="53038-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="53038-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="53038-147">Validation File</span></span>  <br/> |<span data-ttu-id="53038-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="53038-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="53038-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="53038-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="53038-150">False</span><span class="sxs-lookup"><span data-stu-id="53038-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="53038-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="53038-151">See also</span></span>



- [<span data-ttu-id="53038-152">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="53038-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

