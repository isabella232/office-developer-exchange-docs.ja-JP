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
description: Actions 要素は、条件が満たされたときにメッセージに対して実行できる一連のアクションを表します。
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465066"
---
# <a name="actions"></a><span data-ttu-id="558f0-103">アクション</span><span class="sxs-lookup"><span data-stu-id="558f0-103">Actions</span></span>

<span data-ttu-id="558f0-104">**Actions**要素は、条件が満たされたときにメッセージに対して実行できる一連のアクションを表します。</span><span class="sxs-lookup"><span data-stu-id="558f0-104">The **Actions** element represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span> 
  
[<span data-ttu-id="558f0-105">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="558f0-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
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

 <span data-ttu-id="558f0-106">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="558f0-106">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="558f0-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="558f0-107">Attributes and elements</span></span>

<span data-ttu-id="558f0-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="558f0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="558f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="558f0-109">Attributes</span></span>

<span data-ttu-id="558f0-110">なし。</span><span class="sxs-lookup"><span data-stu-id="558f0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="558f0-111">子要素</span><span class="sxs-lookup"><span data-stu-id="558f0-111">Child elements</span></span>

|<span data-ttu-id="558f0-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="558f0-112">**Element**</span></span>|<span data-ttu-id="558f0-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="558f0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="558f0-114">カテゴリを割り当てる</span><span class="sxs-lookup"><span data-stu-id="558f0-114">AssignCategories</span></span>](assigncategories.md) <br/> |<span data-ttu-id="558f0-115">電子メールメッセージにスタンプされている分類項目を表します。</span><span class="sxs-lookup"><span data-stu-id="558f0-115">Represents the categories that are stamped on e-mail messages.</span></span>  <br/> |
|[<span data-ttu-id="558f0-116">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="558f0-116">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="558f0-117">電子メールアイテムがコピーされるフォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="558f0-117">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="558f0-118">Delete</span><span class="sxs-lookup"><span data-stu-id="558f0-118">Delete</span></span>](delete.md) <br/> |<span data-ttu-id="558f0-119">メッセージを [削除済みアイテム] フォルダーに移動するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-119">Indicates whether messages are to be moved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="558f0-120">ForwardAsAttachmentToRecipients 添付ファイル</span><span class="sxs-lookup"><span data-stu-id="558f0-120">ForwardAsAttachmentToRecipients</span></span>](forwardasattachmenttorecipients.md) <br/> |<span data-ttu-id="558f0-121">添付ファイルとして転送されるメッセージの送信先の電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-121">Indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span>  <br/> |
|[<span data-ttu-id="558f0-122">Forwardトーラス (Pitor)</span><span class="sxs-lookup"><span data-stu-id="558f0-122">ForwardToRecipients</span></span>](forwardtorecipients.md) <br/> |<span data-ttu-id="558f0-123">メッセージが転送される電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-123">Indicates the e-mail addresses to which messages are to be forwarded.</span></span>  <br/> |
|[<span data-ttu-id="558f0-124">マーク (重要)</span><span class="sxs-lookup"><span data-stu-id="558f0-124">MarkImportance</span></span>](markimportance.md) <br/> |<span data-ttu-id="558f0-125">メッセージに対してスタンプされる重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="558f0-125">Specifies the importance that is to be stamped on messages.</span></span>  <br/> |
|[<span data-ttu-id="558f0-126">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="558f0-126">MarkAsRead</span></span>](markasread.md) <br/> |<span data-ttu-id="558f0-127">メッセージを開封済みとしてマークするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-127">Indicates whether messages are to be marked as read.</span></span>  <br/> |
|[<span data-ttu-id="558f0-128">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="558f0-128">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="558f0-129">電子メールアイテムの移動先フォルダーの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="558f0-129">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
|[<span data-ttu-id="558f0-130">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="558f0-130">PermanentDelete</span></span>](permanentdelete.md) <br/> |<span data-ttu-id="558f0-131">メッセージが完全に削除され、削除済みアイテムフォルダーに保存されないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-131">Indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span>  <br/> |
|[<span data-ttu-id="558f0-132">RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="558f0-132">RedirectToRecipients</span></span>](redirecttorecipients.md) <br/> |<span data-ttu-id="558f0-133">メッセージがリダイレクトされる電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-133">Indicates the e-mail addresses to which messages are to be redirected.</span></span>  <br/> |
|[<span data-ttu-id="558f0-134">SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="558f0-134">SendSMSAlertToRecipients</span></span>](sendsmsalerttorecipients.md) <br/> |<span data-ttu-id="558f0-135">短いメッセージサービス (SMS) の通知が送信される携帯電話の番号を示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-135">Indicates the mobile phone numbers to which a Short Message Service (SMS) alert is to be sent.</span></span>  <br/> |
|[<span data-ttu-id="558f0-136">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="558f0-136">ServerReplyWithMessage</span></span>](serverreplywithmessage.md) <br/> |<span data-ttu-id="558f0-137">を示し.</span><span class="sxs-lookup"><span data-stu-id="558f0-137">Indicates.</span></span> <span data-ttu-id="558f0-138">受信メッセージへの返信として送信されるテンプレートメッセージの ID です。</span><span class="sxs-lookup"><span data-stu-id="558f0-138">the ID of the template message that is to be sent as a reply to incoming messages.</span></span>  <br/> |
|[<span data-ttu-id="558f0-139">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="558f0-139">StopProcessingRules</span></span>](stopprocessingrules.md) <br/> |<span data-ttu-id="558f0-140">後続のルールを評価するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="558f0-140">Indicates whether subsequent rules are to be evaluated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="558f0-141">親要素</span><span class="sxs-lookup"><span data-stu-id="558f0-141">Parent elements</span></span>

|<span data-ttu-id="558f0-142">**要素**</span><span class="sxs-lookup"><span data-stu-id="558f0-142">**Element**</span></span>|<span data-ttu-id="558f0-143">**説明**</span><span class="sxs-lookup"><span data-stu-id="558f0-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="558f0-144">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="558f0-144">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="558f0-145">ユーザーのメールボックス内の1つのルールを表します。</span><span class="sxs-lookup"><span data-stu-id="558f0-145">Represents a single rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="558f0-146">テキスト値</span><span class="sxs-lookup"><span data-stu-id="558f0-146">Text value</span></span>

<span data-ttu-id="558f0-147">なし。</span><span class="sxs-lookup"><span data-stu-id="558f0-147">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="558f0-148">注釈</span><span class="sxs-lookup"><span data-stu-id="558f0-148">Remarks</span></span>

<span data-ttu-id="558f0-149">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="558f0-149">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="558f0-150">要素の情報</span><span class="sxs-lookup"><span data-stu-id="558f0-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="558f0-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="558f0-151">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="558f0-152">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="558f0-152">Schema Name</span></span>  <br/> |<span data-ttu-id="558f0-153">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="558f0-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="558f0-154">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="558f0-154">Validation File</span></span>  <br/> |<span data-ttu-id="558f0-155">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="558f0-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="558f0-156">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="558f0-156">Can be Empty</span></span>  <br/> |<span data-ttu-id="558f0-157">正しい</span><span class="sxs-lookup"><span data-stu-id="558f0-157">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="558f0-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="558f0-158">See also</span></span>

- [<span data-ttu-id="558f0-159">条件</span><span class="sxs-lookup"><span data-stu-id="558f0-159">Conditions</span></span>](conditions.md)
- [<span data-ttu-id="558f0-160">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="558f0-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

