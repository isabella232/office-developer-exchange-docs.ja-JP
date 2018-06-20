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
description: 条件要素が条件を識別するには、満たされるとときに、ルールのルールの処理がトリガーされます。
ms.openlocfilehash: f66777e82892122c4c7dac45bdef3c42f5c4a577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759650"
---
# <a name="conditions"></a><span data-ttu-id="24104-103">条件</span><span class="sxs-lookup"><span data-stu-id="24104-103">Conditions</span></span>

<span data-ttu-id="24104-104">**条件**要素が条件を識別するには、満たされるとときに、ルールのルールの処理がトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="24104-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
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

 <span data-ttu-id="24104-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="24104-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24104-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="24104-106">Attributes and elements</span></span>

<span data-ttu-id="24104-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="24104-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24104-108">属性</span><span class="sxs-lookup"><span data-stu-id="24104-108">Attributes</span></span>

<span data-ttu-id="24104-109">なし。</span><span class="sxs-lookup"><span data-stu-id="24104-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24104-110">子要素</span><span class="sxs-lookup"><span data-stu-id="24104-110">Child elements</span></span>

|<span data-ttu-id="24104-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="24104-111">**Element**</span></span>|<span data-ttu-id="24104-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="24104-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24104-113">Categories</span><span class="sxs-lookup"><span data-stu-id="24104-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24104-114">カテゴリ適用する場合の条件または例外の順序で受信したメッセージに適用する必要がありますにはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="24104-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="24104-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="24104-116">適用する場合の条件または例外の順序で受信メッセージの本文に表示する文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="24104-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="24104-118">適用する場合の条件または例外の順序で受信メッセージのヘッダーに表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="24104-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="24104-120">**ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティに表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="24104-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="24104-122">**** プロパティに適用する条件または例外の順序で受信したメッセージに表示する文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="24104-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="24104-124">適用する場合の条件または例外の順序で受信したメッセージの件名または本文に表示する文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="24104-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="24104-126">適用する場合の条件または例外の順序で受信したメッセージの件名に表示される文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="24104-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="24104-128">適用する場合の条件または例外の順序で受信したメッセージを表示する必要がありますアクションの値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="24104-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="24104-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="24104-130">元の条件または例外を適用する順序で受信したメッセージを送信する必要がある電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="24104-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="24104-132">受信メッセージの適用の条件または例外のために集められたを持つ必要がある電子メール アカウントの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="24104-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-133">添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="24104-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="24104-134">受信したメッセージを添付ファイルのある条件または例外を適用する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-135">Importance</span><span class="sxs-lookup"><span data-stu-id="24104-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="24104-136">適用する場合の条件または例外の順序で受信したメッセージにスタンプする重要性を指定します。</span><span class="sxs-lookup"><span data-stu-id="24104-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="24104-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="24104-138">受信メッセージに適用する条件または例外の順序で要求を承認をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="24104-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="24104-140">受信メッセージに適用する条件または例外の順に自動転送をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="24104-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="24104-142">受信メッセージに適用する条件または例外の順序で自動返信をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-143">暗号化されたチャレンジ</span><span class="sxs-lookup"><span data-stu-id="24104-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="24104-144">受信メッセージが S/MIME 暗号化を適用する場合の条件または例外の順序である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="24104-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="24104-146">かどうかメッセージを受信する必要がある会議出席依頼を適用する場合の条件または例外の順序で示します。</span><span class="sxs-lookup"><span data-stu-id="24104-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="24104-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="24104-148">受信メッセージが会議のためには条件や例外条件を適用する返答をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="24104-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="24104-150">適用する場合の条件または例外の順序で受信メッセージが配信不能レポート (Ndr) をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="24104-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="24104-152">適用する場合の条件または例外の順序で受信メッセージがアクセス許可の制御 (RMS 保護) をする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="24104-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="24104-154">かどうかの受信メッセージ読み取る必要があります適用の条件または例外のために領収書を示します。</span><span class="sxs-lookup"><span data-stu-id="24104-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-155">入手</span><span class="sxs-lookup"><span data-stu-id="24104-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="24104-156">S/MIME の署名を適用する場合の条件または例外の順序で受信したメッセージがある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="24104-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="24104-158">適用の条件または例外のためにボイス メール メッセージを受信したメッセージがある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="24104-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="24104-160">適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があります項目クラスを表します。</span><span class="sxs-lookup"><span data-stu-id="24104-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="24104-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="24104-162">メッセージの分類を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを表します。</span><span class="sxs-lookup"><span data-stu-id="24104-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="24104-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="24104-164">**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信したメッセージのメールボックスの所有者がある必要がありますいないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="24104-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="24104-166">**CcRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージのあるメールボックスの所有者があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="24104-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="24104-168">**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信メッセージの 1 つのみを使用するメールボックスの所有者があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="24104-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="24104-170">適用する条件または例外の順序でに送信されている受信メッセージを持つ電子メール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="24104-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="24104-172">**ToRecipients**プロパティを適用する場合の条件または例外の順序で受信したメッセージのあるメールボックスの所有者があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="24104-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="24104-174">**ToRecipients**または**CcRecipients**のいずれかの条件または例外を適用する順序で受信メッセージのプロパティで、メールボックスの所有者があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="24104-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="24104-176">感度を適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="24104-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="24104-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="24104-178">受信したメッセージが適用の条件または例外のために到着した日付の範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="24104-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="24104-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="24104-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="24104-180">適用する場合の条件または例外の順序で受信メッセージをする必要のある最小値と最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="24104-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24104-181">親要素</span><span class="sxs-lookup"><span data-stu-id="24104-181">Parent elements</span></span>

|<span data-ttu-id="24104-182">**要素**</span><span class="sxs-lookup"><span data-stu-id="24104-182">**Element**</span></span>|<span data-ttu-id="24104-183">**説明**</span><span class="sxs-lookup"><span data-stu-id="24104-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24104-184">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="24104-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="24104-185">1 つのルールが含まれていて、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="24104-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24104-186">テキスト値</span><span class="sxs-lookup"><span data-stu-id="24104-186">Text value</span></span>

<span data-ttu-id="24104-187">なし。</span><span class="sxs-lookup"><span data-stu-id="24104-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24104-188">備考</span><span class="sxs-lookup"><span data-stu-id="24104-188">Remarks</span></span>

<span data-ttu-id="24104-189">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="24104-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24104-190">要素情報</span><span class="sxs-lookup"><span data-stu-id="24104-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24104-191">名前空間</span><span class="sxs-lookup"><span data-stu-id="24104-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24104-192">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="24104-192">Schema Name</span></span>  <br/> |<span data-ttu-id="24104-193">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="24104-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="24104-194">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="24104-194">Validation File</span></span>  <br/> |<span data-ttu-id="24104-195">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24104-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24104-196">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="24104-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="24104-197">True</span><span class="sxs-lookup"><span data-stu-id="24104-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24104-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="24104-198">See also</span></span>



[<span data-ttu-id="24104-199">Exceptions</span><span class="sxs-lookup"><span data-stu-id="24104-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="24104-200">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="24104-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

