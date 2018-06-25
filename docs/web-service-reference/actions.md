---
title: アクション
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: アクション要素では、一連の条件が満たされるときに、メッセージに対して実行される利用可能なアクションを表します。
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759272"
---
# <a name="actions"></a><span data-ttu-id="18f87-103">アクション</span><span class="sxs-lookup"><span data-stu-id="18f87-103">Actions</span></span>

<span data-ttu-id="18f87-104">**アクション**要素では、一連の条件が満たされるときに、メッセージに対して実行される利用可能なアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="18f87-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="18f87-105">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="18f87-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 <span data-ttu-id="18f87-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="18f87-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18f87-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18f87-107">Attributes and elements</span></span>

<span data-ttu-id="18f87-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18f87-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18f87-109">属性</span><span class="sxs-lookup"><span data-stu-id="18f87-109">Attributes</span></span>

<span data-ttu-id="18f87-110">なし。</span><span class="sxs-lookup"><span data-stu-id="18f87-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18f87-111">子要素</span><span class="sxs-lookup"><span data-stu-id="18f87-111">Child elements</span></span>

|<span data-ttu-id="18f87-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="18f87-112">**Element**</span></span>|<span data-ttu-id="18f87-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="18f87-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18f87-114">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="18f87-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="18f87-115">電子メール メッセージにスタンプされているカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="18f87-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="18f87-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="18f87-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="18f87-117">電子メール アイテムをコピーするフォルダーの ID を識別します。</span><span class="sxs-lookup"><span data-stu-id="18f87-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="18f87-118">Delete</span><span class="sxs-lookup"><span data-stu-id="18f87-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="18f87-119">メッセージを削除済みアイテム フォルダーに移動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="18f87-120">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="18f87-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="18f87-121">メッセージが添付ファイルとして転送するのには電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="18f87-122">ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="18f87-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="18f87-123">メッセージが転送される電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="18f87-124">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="18f87-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="18f87-125">メッセージにスタンプするのには重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="18f87-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="18f87-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="18f87-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="18f87-127">メッセージは開封としてマークするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="18f87-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="18f87-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="18f87-129">電子メール アイテムに移動するフォルダーの ID を識別します。</span><span class="sxs-lookup"><span data-stu-id="18f87-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="18f87-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="18f87-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="18f87-131">メッセージを完全に削除し、削除済みアイテム フォルダーに保存されないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="18f87-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="18f87-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="18f87-133">メッセージがリダイレクトされるように電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="18f87-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="18f87-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="18f87-135">ショート メッセージ サービス (SMS) アラートが送信するのには携帯電話の番号を示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="18f87-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="18f87-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="18f87-137">示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-137">Indicates.</span></span> <span data-ttu-id="18f87-138">受信メッセージへの応答として送信するのには、テンプレートのメッセージの ID です。</span><span class="sxs-lookup"><span data-stu-id="18f87-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="18f87-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="18f87-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="18f87-140">後のルールが評価されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="18f87-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18f87-141">親要素</span><span class="sxs-lookup"><span data-stu-id="18f87-141">Parent elements</span></span>

|<span data-ttu-id="18f87-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="18f87-142">**Element**</span></span>|<span data-ttu-id="18f87-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="18f87-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18f87-144">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="18f87-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="18f87-145">ユーザーのメールボックス内の 1 つのルールを表します。</span><span class="sxs-lookup"><span data-stu-id="18f87-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18f87-146">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18f87-146">Text value</span></span>

<span data-ttu-id="18f87-147">なし。</span><span class="sxs-lookup"><span data-stu-id="18f87-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="18f87-148">備考</span><span class="sxs-lookup"><span data-stu-id="18f87-148">Remarks</span></span>

<span data-ttu-id="18f87-149">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="18f87-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18f87-150">要素情報</span><span class="sxs-lookup"><span data-stu-id="18f87-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18f87-151">名前空間</span><span class="sxs-lookup"><span data-stu-id="18f87-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="18f87-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18f87-152">Schema Name</span></span>  <br/> |<span data-ttu-id="18f87-153">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="18f87-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="18f87-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18f87-154">Validation File</span></span>  <br/> |<span data-ttu-id="18f87-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="18f87-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="18f87-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18f87-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="18f87-157">True</span><span class="sxs-lookup"><span data-stu-id="18f87-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18f87-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="18f87-158">See also</span></span>

- [<span data-ttu-id="18f87-159">条件</span><span class="sxs-lookup"><span data-stu-id="18f87-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="18f87-160">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18f87-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

