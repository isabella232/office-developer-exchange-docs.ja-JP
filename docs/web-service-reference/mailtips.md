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
description: メールヒント要素は、さまざまな種類のメールヒントの値を表します。
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447597"
---
# <a name="mailtips"></a><span data-ttu-id="8580e-103">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="8580e-103">MailTips</span></span>

<span data-ttu-id="8580e-104">メール**ヒント要素は**、さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
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

 <span data-ttu-id="8580e-105">**メールヒント**</span><span class="sxs-lookup"><span data-stu-id="8580e-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8580e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8580e-106">Attributes and elements</span></span>

<span data-ttu-id="8580e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8580e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8580e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8580e-108">Attributes</span></span>

<span data-ttu-id="8580e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8580e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8580e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8580e-110">Child elements</span></span>

|<span data-ttu-id="8580e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8580e-111">**Element**</span></span>|<span data-ttu-id="8580e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8580e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8580e-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="8580e-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="8580e-114">受信者のメールボックスを表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="8580e-115">PendingMailTips ヒント</span><span class="sxs-lookup"><span data-stu-id="8580e-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="8580e-116">この要素のメールヒントが、サーバーの処理タイムアウトが経過する前に評価されなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="8580e-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="8580e-117">不在</span><span class="sxs-lookup"><span data-stu-id="8580e-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="8580e-118">応答メッセージと、応答メッセージを送信する時間を表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="8580e-119">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="8580e-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="8580e-120">受信者のメールボックスがいっぱいになっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8580e-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="8580e-121">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="8580e-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="8580e-122">カスタマイズされたメールヒントメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="8580e-123">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8580e-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="8580e-124">グループ内のすべてのメンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="8580e-125">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8580e-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="8580e-126">グループ内の外部メンバーの数を表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="8580e-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="8580e-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="8580e-128">受信者が受け付けることができる最大メッセージサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="8580e-129">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="8580e-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="8580e-130">配信の制限によって、送信者のメッセージが受信者に届かないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8580e-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="8580e-131">IsModerated</span><span class="sxs-lookup"><span data-stu-id="8580e-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="8580e-132">受信者のメールボックスがモデレートされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8580e-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="8580e-133">InvalidRecipient (メールヒント)</span><span class="sxs-lookup"><span data-stu-id="8580e-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="8580e-134">受信者が無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8580e-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8580e-135">親要素</span><span class="sxs-lookup"><span data-stu-id="8580e-135">Parent elements</span></span>

|<span data-ttu-id="8580e-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="8580e-136">**Element**</span></span>|<span data-ttu-id="8580e-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="8580e-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8580e-138">Mailヒント Responsemessagetype</span><span class="sxs-lookup"><span data-stu-id="8580e-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="8580e-139">メールヒントの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="8580e-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8580e-140">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8580e-140">Text value</span></span>

<span data-ttu-id="8580e-141">なし。</span><span class="sxs-lookup"><span data-stu-id="8580e-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8580e-142">注釈</span><span class="sxs-lookup"><span data-stu-id="8580e-142">Remarks</span></span>

<span data-ttu-id="8580e-143">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8580e-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8580e-144">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8580e-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8580e-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="8580e-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8580e-146">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8580e-146">Schema Name</span></span>  <br/> |<span data-ttu-id="8580e-147">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8580e-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8580e-148">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8580e-148">Validation File</span></span>  <br/> |<span data-ttu-id="8580e-149">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8580e-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8580e-150">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8580e-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="8580e-151">正しくない</span><span class="sxs-lookup"><span data-stu-id="8580e-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8580e-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="8580e-152">See also</span></span>



- [<span data-ttu-id="8580e-153">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8580e-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

