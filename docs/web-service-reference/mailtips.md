---
title: メール ヒント
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: メール ヒントの要素は、さまざまな種類のメール ヒントの値を表します。
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832311"
---
# <a name="mailtips"></a><span data-ttu-id="d3390-103">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="d3390-103">MailTips</span></span>

<span data-ttu-id="d3390-104">**メール ヒント**の要素は、さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 <span data-ttu-id="d3390-105">**メール ヒント**</span><span class="sxs-lookup"><span data-stu-id="d3390-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3390-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d3390-106">Attributes and elements</span></span>

<span data-ttu-id="d3390-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3390-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3390-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3390-108">Attributes</span></span>

<span data-ttu-id="d3390-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d3390-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3390-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d3390-110">Child elements</span></span>

|<span data-ttu-id="d3390-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3390-111">**Element**</span></span>|<span data-ttu-id="d3390-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3390-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3390-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="d3390-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="d3390-114">受信者のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="d3390-115">PendingMailTips</span><span class="sxs-lookup"><span data-stu-id="d3390-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="d3390-116">サーバーの処理のタイムアウト期間が経過する前にこの要素内のメール ヒントを評価できませんでしたを示します。</span><span class="sxs-lookup"><span data-stu-id="d3390-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="d3390-117">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="d3390-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="d3390-118">応答メッセージと応答メッセージを送信するための継続時間を表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="d3390-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="d3390-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="d3390-120">受信者のメールボックスがいっぱいであるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3390-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="d3390-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="d3390-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="d3390-122">カスタマイズしたメール ヒントのメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="d3390-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d3390-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="d3390-124">グループ内のすべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="d3390-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d3390-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="d3390-126">グループ内の外部のメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="d3390-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="d3390-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="d3390-128">受信者が受け入れることができるメッセージの最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="d3390-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="d3390-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="d3390-130">配信の制限が、送信者のメッセージを防ぐため、受信者に到達できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3390-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="d3390-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="d3390-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="d3390-132">受信者のメールボックスがモデレートされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3390-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="d3390-133">InvalidRecipient (メール ヒント)</span><span class="sxs-lookup"><span data-stu-id="d3390-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="d3390-134">受信者が有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d3390-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3390-135">親要素</span><span class="sxs-lookup"><span data-stu-id="d3390-135">Parent elements</span></span>

|<span data-ttu-id="d3390-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3390-136">**Element**</span></span>|<span data-ttu-id="d3390-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3390-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3390-138">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="d3390-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="d3390-139">メールのヒントの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="d3390-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3390-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d3390-140">Text value</span></span>

<span data-ttu-id="d3390-141">なし。</span><span class="sxs-lookup"><span data-stu-id="d3390-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3390-142">備考</span><span class="sxs-lookup"><span data-stu-id="d3390-142">Remarks</span></span>

<span data-ttu-id="d3390-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d3390-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3390-144">要素情報</span><span class="sxs-lookup"><span data-stu-id="d3390-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3390-145">名前空間</span><span class="sxs-lookup"><span data-stu-id="d3390-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3390-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3390-146">Schema Name</span></span>  <br/> |<span data-ttu-id="d3390-147">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d3390-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3390-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3390-148">Validation File</span></span>  <br/> |<span data-ttu-id="d3390-149">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d3390-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3390-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d3390-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3390-151">False</span><span class="sxs-lookup"><span data-stu-id="d3390-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3390-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3390-152">See also</span></span>



- [<span data-ttu-id="d3390-153">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d3390-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

