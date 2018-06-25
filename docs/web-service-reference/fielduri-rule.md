---
title: FieldUri (ルール)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: FieldURI 要素は、検証エラーの原因となったルール] フィールドに URI を指定します。
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760469"
---
# <a name="fielduri-rule"></a><span data-ttu-id="6cc6d-103">FieldUri (ルール)</span><span class="sxs-lookup"><span data-stu-id="6cc6d-103">FieldUri (Rule)</span></span>

<span data-ttu-id="6cc6d-104">**FieldURI**要素は、検証エラーの原因となったルール] フィールドに URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="6cc6d-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="6cc6d-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cc6d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6cc6d-106">Attributes and elements</span></span>

<span data-ttu-id="6cc6d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cc6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cc6d-108">Attributes</span></span>

<span data-ttu-id="6cc6d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cc6d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6cc6d-110">Child elements</span></span>

<span data-ttu-id="6cc6d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cc6d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6cc6d-112">Parent elements</span></span>

|<span data-ttu-id="6cc6d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cc6d-113">**Element**</span></span>|<span data-ttu-id="6cc6d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cc6d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cc6d-115">Error</span><span class="sxs-lookup"><span data-stu-id="6cc6d-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="6cc6d-116">特定のルールのプロパティの値、述語プロパティの値、またはアクションのプロパティの値の 1 つの検証エラーを表します。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6cc6d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6cc6d-117">Text value</span></span>

<span data-ttu-id="6cc6d-118">この要素のテキスト値は、次の文字列のいずれかに制限されています。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="6cc6d-119">規則 Id</span><span class="sxs-lookup"><span data-stu-id="6cc6d-119">RuleId</span></span>
    
- <span data-ttu-id="6cc6d-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="6cc6d-120">DisplayName</span></span>
    
- <span data-ttu-id="6cc6d-121">優先度</span><span class="sxs-lookup"><span data-stu-id="6cc6d-121">Priority</span></span>
    
- <span data-ttu-id="6cc6d-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="6cc6d-122">IsNotSupported</span></span>
    
- <span data-ttu-id="6cc6d-123">アクション</span><span class="sxs-lookup"><span data-stu-id="6cc6d-123">Actions</span></span>
    
- <span data-ttu-id="6cc6d-124">条件のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-124">Condition:Categories</span></span>
    
- <span data-ttu-id="6cc6d-125">条件: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="6cc6d-126">条件: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="6cc6d-127">条件: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="6cc6d-128">条件: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="6cc6d-129">条件: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="6cc6d-130">条件: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="6cc6d-131">条件: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="6cc6d-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="6cc6d-132">条件: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="6cc6d-133">条件: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="6cc6d-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="6cc6d-134">条件: 添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="6cc6d-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="6cc6d-135">条件: 重要性</span><span class="sxs-lookup"><span data-stu-id="6cc6d-135">Condition:Importance</span></span>
    
- <span data-ttu-id="6cc6d-136">条件: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="6cc6d-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="6cc6d-137">条件: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="6cc6d-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="6cc6d-138">条件: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="6cc6d-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="6cc6d-139">条件: 暗号化されたチャレンジ</span><span class="sxs-lookup"><span data-stu-id="6cc6d-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="6cc6d-140">条件: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6cc6d-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="6cc6d-141">条件: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6cc6d-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="6cc6d-142">条件: IsNDR</span><span class="sxs-lookup"><span data-stu-id="6cc6d-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="6cc6d-143">条件: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="6cc6d-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="6cc6d-144">条件: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="6cc6d-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="6cc6d-145">条件入手します。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="6cc6d-146">条件: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="6cc6d-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="6cc6d-147">条件: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="6cc6d-148">条件: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="6cc6d-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="6cc6d-149">条件: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="6cc6d-150">条件: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="6cc6d-151">条件: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="6cc6d-152">条件: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="6cc6d-153">条件: SentToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="6cc6d-154">条件: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="6cc6d-155">条件: 感度解析</span><span class="sxs-lookup"><span data-stu-id="6cc6d-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="6cc6d-156">条件: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="6cc6d-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="6cc6d-157">条件: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="6cc6d-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="6cc6d-158">例外のカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-158">Exception:Categories</span></span>
    
- <span data-ttu-id="6cc6d-159">例外: ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="6cc6d-160">例外: ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="6cc6d-161">例外: ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="6cc6d-162">例外: ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="6cc6d-163">例外: ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="6cc6d-164">例外: ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="6cc6d-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="6cc6d-165">例外: FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="6cc6d-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="6cc6d-166">例外: FromAddresses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="6cc6d-167">例外: FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="6cc6d-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="6cc6d-168">例外: 添付ファイル付き</span><span class="sxs-lookup"><span data-stu-id="6cc6d-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="6cc6d-169">例外: 重要性</span><span class="sxs-lookup"><span data-stu-id="6cc6d-169">Exception:Importance</span></span>
    
- <span data-ttu-id="6cc6d-170">例外: IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="6cc6d-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="6cc6d-171">例外: IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="6cc6d-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="6cc6d-172">例外: IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="6cc6d-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="6cc6d-173">例外: 暗号化されたチャレンジ</span><span class="sxs-lookup"><span data-stu-id="6cc6d-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="6cc6d-174">例外: IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="6cc6d-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="6cc6d-175">例外: IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="6cc6d-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="6cc6d-176">例外: IsNDR</span><span class="sxs-lookup"><span data-stu-id="6cc6d-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="6cc6d-177">例外: IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="6cc6d-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="6cc6d-178">例外: IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="6cc6d-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="6cc6d-179">例外: 入手</span><span class="sxs-lookup"><span data-stu-id="6cc6d-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="6cc6d-180">例外: IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="6cc6d-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="6cc6d-181">例外: ItemClasses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="6cc6d-182">例外: MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="6cc6d-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="6cc6d-183">例外: NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="6cc6d-184">例外: SentCcMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="6cc6d-185">例外: SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="6cc6d-186">例外: SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="6cc6d-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="6cc6d-187">例外: SentToMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="6cc6d-188">例外: SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="6cc6d-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="6cc6d-189">例外: 感度解析</span><span class="sxs-lookup"><span data-stu-id="6cc6d-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="6cc6d-190">例外: WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="6cc6d-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="6cc6d-191">例外: WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="6cc6d-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="6cc6d-192">アクション: AssignCategories</span><span class="sxs-lookup"><span data-stu-id="6cc6d-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="6cc6d-193">アクション: CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="6cc6d-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="6cc6d-194">アクションの削除:</span><span class="sxs-lookup"><span data-stu-id="6cc6d-194">Action:Delete</span></span>
    
- <span data-ttu-id="6cc6d-195">アクション: ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="6cc6d-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="6cc6d-196">アクション: ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="6cc6d-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="6cc6d-197">アクション: MarkImportance</span><span class="sxs-lookup"><span data-stu-id="6cc6d-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="6cc6d-198">アクション: MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="6cc6d-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="6cc6d-199">アクション: MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="6cc6d-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="6cc6d-200">アクション: PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="6cc6d-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="6cc6d-201">アクション: RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="6cc6d-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="6cc6d-202">アクション: SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="6cc6d-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="6cc6d-203">アクション: ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="6cc6d-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="6cc6d-204">アクション: StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="6cc6d-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="6cc6d-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="6cc6d-205">IsEnabled</span></span>
    
- <span data-ttu-id="6cc6d-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="6cc6d-206">IsInError</span></span>
    
- <span data-ttu-id="6cc6d-207">条件</span><span class="sxs-lookup"><span data-stu-id="6cc6d-207">Conditions</span></span>
    
- <span data-ttu-id="6cc6d-208">例外</span><span class="sxs-lookup"><span data-stu-id="6cc6d-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6cc6d-209">備考</span><span class="sxs-lookup"><span data-stu-id="6cc6d-209">Remarks</span></span>

<span data-ttu-id="6cc6d-210">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6cc6d-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cc6d-211">要素情報</span><span class="sxs-lookup"><span data-stu-id="6cc6d-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cc6d-212">名前空間</span><span class="sxs-lookup"><span data-stu-id="6cc6d-212">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cc6d-213">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cc6d-213">Schema Name</span></span>  <br/> |<span data-ttu-id="6cc6d-214">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6cc6d-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cc6d-215">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cc6d-215">Validation File</span></span>  <br/> |<span data-ttu-id="6cc6d-216">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cc6d-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cc6d-217">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6cc6d-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cc6d-218">False</span><span class="sxs-lookup"><span data-stu-id="6cc6d-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cc6d-219">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cc6d-219">See also</span></span>



- [<span data-ttu-id="6cc6d-220">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cc6d-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

