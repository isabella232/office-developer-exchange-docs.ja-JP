---
title: FieldUri (ルール)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: FieldURI 要素は、検証エラーの原因となったルールフィールドへの URI を指定します。
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461248"
---
# <a name="fielduri-rule"></a><span data-ttu-id="54ff2-103">FieldUri (ルール)</span><span class="sxs-lookup"><span data-stu-id="54ff2-103">FieldUri (Rule)</span></span>

<span data-ttu-id="54ff2-104">**FieldURI**要素は、検証エラーの原因となったルールフィールドへの URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="54ff2-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="54ff2-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="54ff2-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54ff2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="54ff2-106">Attributes and elements</span></span>

<span data-ttu-id="54ff2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54ff2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54ff2-108">属性</span><span class="sxs-lookup"><span data-stu-id="54ff2-108">Attributes</span></span>

<span data-ttu-id="54ff2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="54ff2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54ff2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="54ff2-110">Child elements</span></span>

<span data-ttu-id="54ff2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="54ff2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54ff2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="54ff2-112">Parent elements</span></span>

|<span data-ttu-id="54ff2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="54ff2-113">**Element**</span></span>|<span data-ttu-id="54ff2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="54ff2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54ff2-115">Error</span><span class="sxs-lookup"><span data-stu-id="54ff2-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="54ff2-116">特定のルールプロパティ値、述語プロパティ値、または action プロパティ値に対する1つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="54ff2-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54ff2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="54ff2-117">Text value</span></span>

<span data-ttu-id="54ff2-118">この要素のテキスト値は、次の文字列のいずれかに制限されています。</span><span class="sxs-lookup"><span data-stu-id="54ff2-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="54ff2-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="54ff2-119">RuleId</span></span>
    
- <span data-ttu-id="54ff2-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="54ff2-120">DisplayName</span></span>
    
- <span data-ttu-id="54ff2-121">優先度</span><span class="sxs-lookup"><span data-stu-id="54ff2-121">Priority</span></span>
    
- <span data-ttu-id="54ff2-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="54ff2-122">IsNotSupported</span></span>
    
- <span data-ttu-id="54ff2-123">アクション</span><span class="sxs-lookup"><span data-stu-id="54ff2-123">Actions</span></span>
    
- <span data-ttu-id="54ff2-124">条件: カテゴリ</span><span class="sxs-lookup"><span data-stu-id="54ff2-124">Condition:Categories</span></span>
    
- <span data-ttu-id="54ff2-125">条件: 文字列</span><span class="sxs-lookup"><span data-stu-id="54ff2-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="54ff2-126">条件: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="54ff2-127">条件: 次の文字列を持つ</span><span class="sxs-lookup"><span data-stu-id="54ff2-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="54ff2-128">条件: という文字列</span><span class="sxs-lookup"><span data-stu-id="54ff2-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="54ff2-129">条件: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="54ff2-130">条件: 大き Subjectstrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="54ff2-131">条件: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="54ff2-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="54ff2-132">条件: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="54ff2-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="54ff2-133">条件: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="54ff2-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="54ff2-134">条件: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="54ff2-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="54ff2-135">条件: 重要度</span><span class="sxs-lookup"><span data-stu-id="54ff2-135">Condition:Importance</span></span>
    
- <span data-ttu-id="54ff2-136">条件: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="54ff2-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="54ff2-137">条件: Is自動転送</span><span class="sxs-lookup"><span data-stu-id="54ff2-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="54ff2-138">条件: Is自動応答</span><span class="sxs-lookup"><span data-stu-id="54ff2-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="54ff2-139">条件: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="54ff2-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="54ff2-140">条件: Is会議要求</span><span class="sxs-lookup"><span data-stu-id="54ff2-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="54ff2-141">条件: Is会議応答</span><span class="sxs-lookup"><span data-stu-id="54ff2-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="54ff2-142">条件: IsNDR</span><span class="sxs-lookup"><span data-stu-id="54ff2-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="54ff2-143">条件: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="54ff2-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="54ff2-144">条件: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="54ff2-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="54ff2-145">条件: IsSigned</span><span class="sxs-lookup"><span data-stu-id="54ff2-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="54ff2-146">条件: IsVoicemail メール</span><span class="sxs-lookup"><span data-stu-id="54ff2-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="54ff2-147">条件: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="54ff2-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="54ff2-148">条件: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="54ff2-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="54ff2-149">条件: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="54ff2-150">条件: [Ccme]</span><span class="sxs-lookup"><span data-stu-id="54ff2-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="54ff2-151">条件: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="54ff2-152">条件: 文のアドレス</span><span class="sxs-lookup"><span data-stu-id="54ff2-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="54ff2-153">条件: SentToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="54ff2-154">条件: 説明文</span><span class="sxs-lookup"><span data-stu-id="54ff2-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="54ff2-155">条件: 秘密度</span><span class="sxs-lookup"><span data-stu-id="54ff2-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="54ff2-156">条件: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="54ff2-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="54ff2-157">条件: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="54ff2-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="54ff2-158">例外: カテゴリ</span><span class="sxs-lookup"><span data-stu-id="54ff2-158">Exception:Categories</span></span>
    
- <span data-ttu-id="54ff2-159">例外: 次の文字列があります。</span><span class="sxs-lookup"><span data-stu-id="54ff2-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="54ff2-160">例外: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="54ff2-161">例外: すべての受信者文字列</span><span class="sxs-lookup"><span data-stu-id="54ff2-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="54ff2-162">例外: という文字列</span><span class="sxs-lookup"><span data-stu-id="54ff2-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="54ff2-163">例外: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="54ff2-164">例外: 大き Subjectstrings</span><span class="sxs-lookup"><span data-stu-id="54ff2-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="54ff2-165">例外: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="54ff2-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="54ff2-166">例外: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="54ff2-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="54ff2-167">例外: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="54ff2-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="54ff2-168">例外: HasAttachments</span><span class="sxs-lookup"><span data-stu-id="54ff2-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="54ff2-169">例外: 重要度</span><span class="sxs-lookup"><span data-stu-id="54ff2-169">Exception:Importance</span></span>
    
- <span data-ttu-id="54ff2-170">例外: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="54ff2-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="54ff2-171">例外: Is自動転送</span><span class="sxs-lookup"><span data-stu-id="54ff2-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="54ff2-172">例外: Is自動応答</span><span class="sxs-lookup"><span data-stu-id="54ff2-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="54ff2-173">例外: IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="54ff2-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="54ff2-174">例外: Is会議要求</span><span class="sxs-lookup"><span data-stu-id="54ff2-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="54ff2-175">例外: Is会議応答</span><span class="sxs-lookup"><span data-stu-id="54ff2-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="54ff2-176">例外: IsNDR</span><span class="sxs-lookup"><span data-stu-id="54ff2-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="54ff2-177">例外: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="54ff2-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="54ff2-178">例外: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="54ff2-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="54ff2-179">例外: IsSigned</span><span class="sxs-lookup"><span data-stu-id="54ff2-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="54ff2-180">例外: IsVoicemail メール</span><span class="sxs-lookup"><span data-stu-id="54ff2-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="54ff2-181">例外: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="54ff2-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="54ff2-182">例外: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="54ff2-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="54ff2-183">例外: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="54ff2-184">例外: [Ccme]</span><span class="sxs-lookup"><span data-stu-id="54ff2-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="54ff2-185">例外: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="54ff2-186">例外: アドレスの説明</span><span class="sxs-lookup"><span data-stu-id="54ff2-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="54ff2-187">例外: SentToMe</span><span class="sxs-lookup"><span data-stu-id="54ff2-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="54ff2-188">例外: 文の説明</span><span class="sxs-lookup"><span data-stu-id="54ff2-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="54ff2-189">例外: 秘密度</span><span class="sxs-lookup"><span data-stu-id="54ff2-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="54ff2-190">例外: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="54ff2-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="54ff2-191">例外: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="54ff2-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="54ff2-192">アクション: カテゴリを割り当てる</span><span class="sxs-lookup"><span data-stu-id="54ff2-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="54ff2-193">アクション: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="54ff2-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="54ff2-194">アクション: 削除</span><span class="sxs-lookup"><span data-stu-id="54ff2-194">Action:Delete</span></span>
    
- <span data-ttu-id="54ff2-195">アクション: forwardasattachmenttorattachmentpiattachment</span><span class="sxs-lookup"><span data-stu-id="54ff2-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="54ff2-196">アクション: forwardtorpipipi</span><span class="sxs-lookup"><span data-stu-id="54ff2-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="54ff2-197">アクション: マーク (重要)</span><span class="sxs-lookup"><span data-stu-id="54ff2-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="54ff2-198">アクション: MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="54ff2-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="54ff2-199">アクション: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="54ff2-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="54ff2-200">アクション: PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="54ff2-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="54ff2-201">アクション: Redirecttorの Piん</span><span class="sxs-lookup"><span data-stu-id="54ff2-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="54ff2-202">アクション: SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="54ff2-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="54ff2-203">アクション: ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="54ff2-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="54ff2-204">アクション: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="54ff2-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="54ff2-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="54ff2-205">IsEnabled</span></span>
    
- <span data-ttu-id="54ff2-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="54ff2-206">IsInError</span></span>
    
- <span data-ttu-id="54ff2-207">条件</span><span class="sxs-lookup"><span data-stu-id="54ff2-207">Conditions</span></span>
    
- <span data-ttu-id="54ff2-208">Exceptions</span><span class="sxs-lookup"><span data-stu-id="54ff2-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="54ff2-209">注釈</span><span class="sxs-lookup"><span data-stu-id="54ff2-209">Remarks</span></span>

<span data-ttu-id="54ff2-210">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="54ff2-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54ff2-211">要素の情報</span><span class="sxs-lookup"><span data-stu-id="54ff2-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54ff2-212">Namespace</span><span class="sxs-lookup"><span data-stu-id="54ff2-212">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54ff2-213">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54ff2-213">Schema Name</span></span>  <br/> |<span data-ttu-id="54ff2-214">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="54ff2-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54ff2-215">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54ff2-215">Validation File</span></span>  <br/> |<span data-ttu-id="54ff2-216">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="54ff2-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54ff2-217">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="54ff2-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="54ff2-218">正しくない</span><span class="sxs-lookup"><span data-stu-id="54ff2-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54ff2-219">関連項目</span><span class="sxs-lookup"><span data-stu-id="54ff2-219">See also</span></span>



- [<span data-ttu-id="54ff2-220">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="54ff2-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

