---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: ApprovalRequestData 要素は、承認要求メッセージの承認状態を指定します。
ms.openlocfilehash: decbd4d646a56b9810387adcdb6a9049da89bc38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462305"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="17ea5-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="17ea5-103">ApprovalRequestData</span></span>

<span data-ttu-id="17ea5-104">**Approvalrequestdata**要素は、承認要求メッセージの承認状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="17ea5-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="17ea5-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="17ea5-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17ea5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17ea5-106">Attributes and elements</span></span>

<span data-ttu-id="17ea5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17ea5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17ea5-108">属性</span><span class="sxs-lookup"><span data-stu-id="17ea5-108">Attributes</span></span>

<span data-ttu-id="17ea5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="17ea5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17ea5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="17ea5-110">Child elements</span></span>

<span data-ttu-id="17ea5-111">[Is未確認 Dedapprovalrequest](isundecidedapprovalrequest.md)  | [Approvaldecision](approvaldecision.md)  | [ApprovalDecisionMaker](approvaldecisionmaker.md)  | [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="17ea5-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17ea5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="17ea5-112">Parent elements</span></span>

[<span data-ttu-id="17ea5-113">Message</span><span class="sxs-lookup"><span data-stu-id="17ea5-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="17ea5-114">注釈</span><span class="sxs-lookup"><span data-stu-id="17ea5-114">Remarks</span></span>

<span data-ttu-id="17ea5-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="17ea5-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="17ea5-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="17ea5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17ea5-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="17ea5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17ea5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="17ea5-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17ea5-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17ea5-119">Schema Name</span></span>  <br/> |<span data-ttu-id="17ea5-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="17ea5-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="17ea5-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17ea5-121">Validation File</span></span>  <br/> |<span data-ttu-id="17ea5-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="17ea5-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17ea5-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="17ea5-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="17ea5-124">正しい</span><span class="sxs-lookup"><span data-stu-id="17ea5-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17ea5-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="17ea5-125">See also</span></span>

- [<span data-ttu-id="17ea5-126">Message</span><span class="sxs-lookup"><span data-stu-id="17ea5-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="17ea5-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="17ea5-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

