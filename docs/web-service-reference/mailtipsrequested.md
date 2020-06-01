---
title: Mailヒント要求
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
description: Mailヒント要求要素には、サービスから要求されたメールヒントの種類が含まれています。
ms.openlocfilehash: bcb2ebf15e628a04e8507f938d385cf113f2f2a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465899"
---
# <a name="mailtipsrequested"></a><span data-ttu-id="3f78f-103">Mailヒント要求</span><span class="sxs-lookup"><span data-stu-id="3f78f-103">MailTipsRequested</span></span>

<span data-ttu-id="3f78f-104">**Mailヒント要求**要素には、サービスから要求されたメールヒントの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3f78f-104">The **MailTipsRequested** element contains the types of mail tips requested from the service.</span></span> 
  
```XML
<MailTipsRequested/>
```

 <span data-ttu-id="3f78f-105">**Mailヒントの種類**</span><span class="sxs-lookup"><span data-stu-id="3f78f-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f78f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3f78f-106">Attributes and elements</span></span>

<span data-ttu-id="3f78f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f78f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f78f-108">Attributes</span></span>

<span data-ttu-id="3f78f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3f78f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f78f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3f78f-110">Child elements</span></span>

<span data-ttu-id="3f78f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3f78f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f78f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3f78f-112">Parent elements</span></span>

|<span data-ttu-id="3f78f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3f78f-113">**Element**</span></span>|<span data-ttu-id="3f78f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f78f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f78f-115">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="3f78f-115">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="3f78f-116">取得するメールヒントの受信者と種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3f78f-116">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f78f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3f78f-117">Text value</span></span>

<span data-ttu-id="3f78f-118">次の表に、 **Mailヒントの要求さ**れた要素に使用できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-118">The following table lists the possible values for the **MailTipsRequested** element.</span></span> 
  
|<span data-ttu-id="3f78f-119">**値**</span><span class="sxs-lookup"><span data-stu-id="3f78f-119">**Value**</span></span>|<span data-ttu-id="3f78f-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f78f-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f78f-121">すべて</span><span class="sxs-lookup"><span data-stu-id="3f78f-121">All</span></span>  <br/> |<span data-ttu-id="3f78f-122">利用可能なすべてのメールヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="3f78f-123">OutOfOfficeMessage</span><span class="sxs-lookup"><span data-stu-id="3f78f-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="3f78f-124">不在 (OOF) メッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="3f78f-125">MailboxFullStatus</span><span class="sxs-lookup"><span data-stu-id="3f78f-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="3f78f-126">フルのメールボックスの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-126">Represents the status for a mailbox that is full.</span></span>  <br/> |
|<span data-ttu-id="3f78f-127">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="3f78f-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="3f78f-128">ユーザー設定のメールヒントを表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="3f78f-129">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="3f78f-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="3f78f-130">外部メンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="3f78f-131">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="3f78f-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="3f78f-132">すべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="3f78f-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="3f78f-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="3f78f-134">受信者が受け付けることができる最大メッセージサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="3f78f-135">DeliveryRestriction</span><span class="sxs-lookup"><span data-stu-id="3f78f-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="3f78f-136">配信の制限によって、送信者のメッセージが受信者に届かないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="3f78f-137">ModerationStatus</span><span class="sxs-lookup"><span data-stu-id="3f78f-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="3f78f-138">送信者のメッセージがモデレーターによって確認されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="3f78f-139">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="3f78f-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="3f78f-140">受信者が無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f78f-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f78f-141">注釈</span><span class="sxs-lookup"><span data-stu-id="3f78f-141">Remarks</span></span>

<span data-ttu-id="3f78f-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3f78f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f78f-143">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3f78f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f78f-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f78f-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3f78f-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3f78f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="3f78f-146">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3f78f-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3f78f-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3f78f-147">Validation File</span></span>  <br/> |<span data-ttu-id="3f78f-148">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3f78f-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3f78f-149">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3f78f-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f78f-150">正しくない</span><span class="sxs-lookup"><span data-stu-id="3f78f-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f78f-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="3f78f-151">See also</span></span>



- [<span data-ttu-id="3f78f-152">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3f78f-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

