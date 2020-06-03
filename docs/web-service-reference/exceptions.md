---
title: Exceptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: Exceptions 要素は、受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を識別します。
ms.openlocfilehash: 1afc2980391ee588f9b9b813b87c2c699de3a6df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463357"
---
# <a name="exceptions"></a><span data-ttu-id="80f3d-103">Exceptions</span><span class="sxs-lookup"><span data-stu-id="80f3d-103">Exceptions</span></span>

<span data-ttu-id="80f3d-104">**Exceptions**要素は、受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を識別します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-104">The **Exceptions** element identifies the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span> 
  
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

 <span data-ttu-id="80f3d-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="80f3d-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="80f3d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="80f3d-106">Attributes and elements</span></span>

<span data-ttu-id="80f3d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80f3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="80f3d-108">Attributes</span></span>

<span data-ttu-id="80f3d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="80f3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80f3d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="80f3d-110">Child elements</span></span>

|<span data-ttu-id="80f3d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="80f3d-111">**Element**</span></span>|<span data-ttu-id="80f3d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="80f3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80f3d-113">Categories</span><span class="sxs-lookup"><span data-stu-id="80f3d-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="80f3d-114">条件または例外を適用するために、受信メッセージに適用する必要があるカテゴリを含みます。</span><span class="sxs-lookup"><span data-stu-id="80f3d-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-115">大き Body文字列</span><span class="sxs-lookup"><span data-stu-id="80f3d-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="80f3d-116">条件または例外を適用するために、受信メッセージの本文に表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="80f3d-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="80f3d-118">条件または例外を適用するために、受信メッセージのヘッダーに表示する必要がある文字列を Indicaqtes します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-118">Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-119">持つ受信者文字列</span><span class="sxs-lookup"><span data-stu-id="80f3d-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="80f3d-120">条件または例外を適用するために、受信メッセージの**torな piの**イベントまたは**ccrecipients**各プロパティに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-121">文字列</span><span class="sxs-lookup"><span data-stu-id="80f3d-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="80f3d-122">条件または例外を適用するために、受信メッセージの**From**プロパティに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="80f3d-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="80f3d-124">条件または例外を適用するために、受信メッセージの本文または件名のどちらかに表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-125">大き Subjectstrings</span><span class="sxs-lookup"><span data-stu-id="80f3d-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="80f3d-126">条件または例外を適用するために、受信メッセージの件名に表示する必要がある文字列を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="80f3d-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="80f3d-128">条件または例外を適用するために、受信メッセージに表示する必要があるアクション値のフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="80f3d-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="80f3d-130">条件または例外を適用するために、受信メッセージを送信する必要がある電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="80f3d-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="80f3d-132">条件または例外を適用するために、受信メッセージが集計されている必要がある電子メールアカウント名を表します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="80f3d-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="80f3d-134">条件または例外を適用するために、受信メッセージに添付ファイルを含める必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-135">Importance</span><span class="sxs-lookup"><span data-stu-id="80f3d-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="80f3d-136">条件または例外を適用するために、受信メッセージにスタンプされる重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="80f3d-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="80f3d-138">条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-139">Is自動転送</span><span class="sxs-lookup"><span data-stu-id="80f3d-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="80f3d-140">条件または例外を適用するために、受信メッセージを自動転送する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-141">Is自動応答</span><span class="sxs-lookup"><span data-stu-id="80f3d-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="80f3d-142">条件または例外を適用するために、受信メッセージが自動応答である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="80f3d-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="80f3d-144">条件または例外を適用するために、受信メッセージを S/MIME で暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-145">Is会議要求</span><span class="sxs-lookup"><span data-stu-id="80f3d-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="80f3d-146">条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-147">Is会議の応答</span><span class="sxs-lookup"><span data-stu-id="80f3d-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="80f3d-148">条件または例外を適用するために、受信メッセージが会議出席依頼に応答する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="80f3d-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="80f3d-150">条件または例外を適用するために、受信メッセージが配信不能レポート (Ndr) である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="80f3d-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="80f3d-152">条件または例外を適用するために、受信メッセージが権限制御される (RMS 保護) 必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply</span></span>  <br/> |
|[<span data-ttu-id="80f3d-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="80f3d-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="80f3d-154">条件または例外を適用するために、受信メッセージが開封確認である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="80f3d-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="80f3d-156">条件または例外を適用するために、受信メッセージが S/MIME で署名されている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-157">IsVoicemail メール</span><span class="sxs-lookup"><span data-stu-id="80f3d-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="80f3d-158">条件または例外を適用するために、受信メッセージがボイスメールメッセージである必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="80f3d-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="80f3d-160">条件または例外を適用するために、受信メッセージにスタンプする必要があるアイテムクラスを表します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="80f3d-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="80f3d-162">条件または例外を適用するために、受信メッセージにスタンプする必要があるメッセージ分類を表します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="80f3d-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="80f3d-164">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**トーラス**プロパティに含まれないようにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-165">Ccme の説明</span><span class="sxs-lookup"><span data-stu-id="80f3d-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="80f3d-166">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Ccrecipients**プロパティにある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="80f3d-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="80f3d-168">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある唯一の所有者である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-169">住所</span><span class="sxs-lookup"><span data-stu-id="80f3d-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="80f3d-170">条件または例外を適用するために、受信メッセージの送信先の電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="80f3d-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="80f3d-172">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**プロパティにある必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-173">「Orccme」</span><span class="sxs-lookup"><span data-stu-id="80f3d-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="80f3d-174">条件または例外を適用するために、メールボックスの所有者が受信メッセージの**Torecipients**イベントまたは**ccrecipients**プロパティのいずれかに含まれている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="80f3d-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="80f3d-176">条件または例外を適用するために、受信メッセージにスタンプする必要がある感度を示します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="80f3d-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="80f3d-178">条件または例外を適用するために、受信メッセージが受信される必要がある日付範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="80f3d-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="80f3d-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="80f3d-180">条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="80f3d-181">親要素</span><span class="sxs-lookup"><span data-stu-id="80f3d-181">Parent elements</span></span>

|<span data-ttu-id="80f3d-182">**要素**</span><span class="sxs-lookup"><span data-stu-id="80f3d-182">**Element**</span></span>|<span data-ttu-id="80f3d-183">**説明**</span><span class="sxs-lookup"><span data-stu-id="80f3d-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80f3d-184">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="80f3d-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="80f3d-185">1つのルールを含み、ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="80f3d-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80f3d-186">テキスト値</span><span class="sxs-lookup"><span data-stu-id="80f3d-186">Text value</span></span>

<span data-ttu-id="80f3d-187">なし。</span><span class="sxs-lookup"><span data-stu-id="80f3d-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80f3d-188">注釈</span><span class="sxs-lookup"><span data-stu-id="80f3d-188">Remarks</span></span>

<span data-ttu-id="80f3d-189">ルールの述語は、ルールの条件または例外として使用されます。</span><span class="sxs-lookup"><span data-stu-id="80f3d-189">The rule predicates are used as rule conditions or exceptions.</span></span>
  
<span data-ttu-id="80f3d-190">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="80f3d-190">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="80f3d-191">要素の情報</span><span class="sxs-lookup"><span data-stu-id="80f3d-191">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80f3d-192">Namespace</span><span class="sxs-lookup"><span data-stu-id="80f3d-192">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80f3d-193">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="80f3d-193">Schema Name</span></span>  <br/> |<span data-ttu-id="80f3d-194">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="80f3d-194">Types schema</span></span>  <br/> |
|<span data-ttu-id="80f3d-195">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="80f3d-195">Validation File</span></span>  <br/> |<span data-ttu-id="80f3d-196">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="80f3d-196">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80f3d-197">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="80f3d-197">Can be Empty</span></span>  <br/> |<span data-ttu-id="80f3d-198">正しい</span><span class="sxs-lookup"><span data-stu-id="80f3d-198">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80f3d-199">関連項目</span><span class="sxs-lookup"><span data-stu-id="80f3d-199">See also</span></span>



[<span data-ttu-id="80f3d-200">条件</span><span class="sxs-lookup"><span data-stu-id="80f3d-200">Conditions</span></span>](conditions.md)


- [<span data-ttu-id="80f3d-201">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="80f3d-201">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

