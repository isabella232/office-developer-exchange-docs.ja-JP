---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: ApprovalRequestData 要素は、承認要求メッセージの承認の状態を指定します。
ms.openlocfilehash: ed1c1e3db4edd2cf4de032dc61abd73e863d4f1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759425"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="3a0fc-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="3a0fc-103">ApprovalRequestData</span></span>

<span data-ttu-id="3a0fc-104">**ApprovalRequestData**要素は、承認要求メッセージの承認の状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a0fc-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="3a0fc-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="3a0fc-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a0fc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a0fc-106">Attributes and elements</span></span>

<span data-ttu-id="3a0fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a0fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a0fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a0fc-108">Attributes</span></span>

<span data-ttu-id="3a0fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a0fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a0fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a0fc-110">Child elements</span></span>

<span data-ttu-id="3a0fc-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="3a0fc-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a0fc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3a0fc-112">Parent elements</span></span>

[<span data-ttu-id="3a0fc-113">Message</span><span class="sxs-lookup"><span data-stu-id="3a0fc-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="3a0fc-114">Remarks</span><span class="sxs-lookup"><span data-stu-id="3a0fc-114">Remarks</span></span>

<span data-ttu-id="3a0fc-115">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3a0fc-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3a0fc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a0fc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a0fc-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="3a0fc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a0fc-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="3a0fc-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a0fc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a0fc-119">Schema Name</span></span>  <br/> |<span data-ttu-id="3a0fc-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3a0fc-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="3a0fc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a0fc-121">Validation File</span></span>  <br/> |<span data-ttu-id="3a0fc-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3a0fc-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a0fc-123">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3a0fc-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a0fc-124">True</span><span class="sxs-lookup"><span data-stu-id="3a0fc-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a0fc-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a0fc-125">See also</span></span>

- [<span data-ttu-id="3a0fc-126">Message</span><span class="sxs-lookup"><span data-stu-id="3a0fc-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="3a0fc-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3a0fc-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

