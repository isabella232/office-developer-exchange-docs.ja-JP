---
title: 条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: 条件要素は、処理されるときにルールのルールの処理をトリガーする条件を示します。
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463203"
---
# <a name="conditions"></a><span data-ttu-id="74a42-103">条件</span><span class="sxs-lookup"><span data-stu-id="74a42-103">Conditions</span></span>

<span data-ttu-id="74a42-104">**条件**要素は、処理されるときにルールのルールの処理をトリガーする条件を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 <span data-ttu-id="74a42-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="74a42-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74a42-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74a42-106">Attributes and elements</span></span>

<span data-ttu-id="74a42-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74a42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74a42-108">属性</span><span class="sxs-lookup"><span data-stu-id="74a42-108">Attributes</span></span>

<span data-ttu-id="74a42-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74a42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74a42-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74a42-110">Child elements</span></span>

|<span data-ttu-id="74a42-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="74a42-111">**Element**</span></span>|<span data-ttu-id="74a42-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74a42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74a42-113">Categories</span><span class="sxs-lookup"><span data-stu-id="74a42-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="74a42-114">条件または例外を適用するために、受信メッセージに適用する必要があるカテゴリを含みます。</span><span class="sxs-lookup"><span data-stu-id="74a42-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-115">大き Body文字列</span><span class="sxs-lookup"><span data-stu-id="74a42-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="74a42-116">条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="74a42-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="74a42-118">条件または例外を適用するために、受信メッセージのヘッダーに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-119">持つ受信者文字列</span><span class="sxs-lookup"><span data-stu-id="74a42-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="74a42-120">条件または例外を適用するために、受信メッセージの**torな piの**イベントまたは**ccrecipients**各プロパティに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-121">文字列</span><span class="sxs-lookup"><span data-stu-id="74a42-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="74a42-122">条件または例外を適用するために、受信メッセージの**From**プロパティに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="74a42-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="74a42-124">条件または例外を適用するために、受信メッセージの本文または件名のどちらかに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-125">大き Subjectstrings</span><span class="sxs-lookup"><span data-stu-id="74a42-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="74a42-126">条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="74a42-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="74a42-128">条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="74a42-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="74a42-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="74a42-130">条件または例外を適用するために、受信メッセージを送信する必要がある電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="74a42-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="74a42-132">条件または例外を適用するために、受信メッセージが集計されている必要がある電子メールアカウント名を表します。</span><span class="sxs-lookup"><span data-stu-id="74a42-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="74a42-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="74a42-134">条件または例外を適用するために、受信メッセージに添付ファイルを含める必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-135">Importance</span><span class="sxs-lookup"><span data-stu-id="74a42-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="74a42-136">条件または例外を適用するために、受信メッセージにスタンプされる重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="74a42-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="74a42-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="74a42-138">条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-139">Is自動転送</span><span class="sxs-lookup"><span data-stu-id="74a42-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="74a42-140">条件または例外を適用するために、受信メッセージを自動転送する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-141">Is自動応答</span><span class="sxs-lookup"><span data-stu-id="74a42-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="74a42-142">条件または例外を適用するために、受信メッセージが自動応答である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="74a42-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="74a42-144">条件または例外を適用するために、受信メッセージを S/MIME で暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-145">Is会議要求</span><span class="sxs-lookup"><span data-stu-id="74a42-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="74a42-146">条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-147">Is会議の応答</span><span class="sxs-lookup"><span data-stu-id="74a42-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="74a42-148">条件または例外を適用するために、受信メッセージが会議出席依頼に応答する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="74a42-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="74a42-150">条件または例外を適用するために、受信メッセージが配信不能レポート (Ndr) である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="74a42-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="74a42-152">条件または例外を適用するために、受信メッセージが権限制御される (RMS 保護) 必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="74a42-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="74a42-154">条件または例外を適用するために、受信メッセージが開封確認である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="74a42-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="74a42-156">条件または例外を適用するために、受信メッセージが S/MIME で署名されている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-157">IsVoicemail メール</span><span class="sxs-lookup"><span data-stu-id="74a42-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="74a42-158">条件または例外を適用するために、受信メッセージがボイスメールメッセージである必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="74a42-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="74a42-160">条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="74a42-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="74a42-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="74a42-162">条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類を表します。</span><span class="sxs-lookup"><span data-stu-id="74a42-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="74a42-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="74a42-164">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**トーラス**プロパティに含まれないようにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-165">Ccme の説明</span><span class="sxs-lookup"><span data-stu-id="74a42-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="74a42-166">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Ccrecipients**プロパティにある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="74a42-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="74a42-168">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある唯一の所有者である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-169">住所</span><span class="sxs-lookup"><span data-stu-id="74a42-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="74a42-170">条件または例外を適用するために、受信メッセージの送信先の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="74a42-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="74a42-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="74a42-172">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-173">「Orccme」</span><span class="sxs-lookup"><span data-stu-id="74a42-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="74a42-174">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**イベントまたは**ccrecipients**プロパティのいずれかに含まれている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="74a42-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="74a42-176">条件または例外を適用するために、受信メッセージにスタンプする必要がある感度を示します。</span><span class="sxs-lookup"><span data-stu-id="74a42-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="74a42-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="74a42-178">条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="74a42-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="74a42-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="74a42-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="74a42-180">条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="74a42-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74a42-181">親要素</span><span class="sxs-lookup"><span data-stu-id="74a42-181">Parent elements</span></span>

|<span data-ttu-id="74a42-182">**要素**</span><span class="sxs-lookup"><span data-stu-id="74a42-182">**Element**</span></span>|<span data-ttu-id="74a42-183">**説明**</span><span class="sxs-lookup"><span data-stu-id="74a42-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74a42-184">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="74a42-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="74a42-185">1つのルールを含み、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="74a42-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74a42-186">テキスト値</span><span class="sxs-lookup"><span data-stu-id="74a42-186">Text value</span></span>

<span data-ttu-id="74a42-187">なし。</span><span class="sxs-lookup"><span data-stu-id="74a42-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74a42-188">注釈</span><span class="sxs-lookup"><span data-stu-id="74a42-188">Remarks</span></span>

<span data-ttu-id="74a42-189">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="74a42-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74a42-190">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74a42-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74a42-191">Namespace</span><span class="sxs-lookup"><span data-stu-id="74a42-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="74a42-192">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74a42-192">Schema Name</span></span>  <br/> |<span data-ttu-id="74a42-193">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="74a42-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="74a42-194">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74a42-194">Validation File</span></span>  <br/> |<span data-ttu-id="74a42-195">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="74a42-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="74a42-196">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74a42-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="74a42-197">正しい</span><span class="sxs-lookup"><span data-stu-id="74a42-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74a42-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="74a42-198">See also</span></span>



[<span data-ttu-id="74a42-199">例外</span><span class="sxs-lookup"><span data-stu-id="74a42-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="74a42-200">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="74a42-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

