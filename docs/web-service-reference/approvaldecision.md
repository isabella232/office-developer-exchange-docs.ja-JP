---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: ApprovalDecision 要素は、承認要求メッセージに対して行われた決定を指定します。
ms.openlocfilehash: a8dc168edec882ba97cdea764f8d20c71ed85f8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463448"
---
# <a name="approvaldecision"></a><span data-ttu-id="57bcc-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="57bcc-103">ApprovalDecision</span></span>

<span data-ttu-id="57bcc-104">**Approvaldecision**要素は、承認要求メッセージに対して行われた決定を指定します。</span><span class="sxs-lookup"><span data-stu-id="57bcc-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="57bcc-105">**int**</span><span class="sxs-lookup"><span data-stu-id="57bcc-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57bcc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="57bcc-106">Attributes and elements</span></span>

<span data-ttu-id="57bcc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57bcc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57bcc-108">属性</span><span class="sxs-lookup"><span data-stu-id="57bcc-108">Attributes</span></span>

<span data-ttu-id="57bcc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57bcc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57bcc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57bcc-110">Child elements</span></span>

<span data-ttu-id="57bcc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57bcc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57bcc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57bcc-112">Parent elements</span></span>

[<span data-ttu-id="57bcc-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="57bcc-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="57bcc-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57bcc-114">Text value</span></span>

<span data-ttu-id="57bcc-115">**Approvaldecision**要素のテキスト値は、承認された場合は1、拒否した場合は2です。</span><span class="sxs-lookup"><span data-stu-id="57bcc-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="57bcc-116">注釈</span><span class="sxs-lookup"><span data-stu-id="57bcc-116">Remarks</span></span>

<span data-ttu-id="57bcc-117">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57bcc-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="57bcc-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57bcc-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57bcc-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="57bcc-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57bcc-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="57bcc-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57bcc-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57bcc-121">Schema Name</span></span>  <br/> |<span data-ttu-id="57bcc-122">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="57bcc-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="57bcc-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57bcc-123">Validation File</span></span>  <br/> |<span data-ttu-id="57bcc-124">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="57bcc-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57bcc-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57bcc-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="57bcc-126">正しい</span><span class="sxs-lookup"><span data-stu-id="57bcc-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57bcc-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="57bcc-127">See also</span></span>

- [<span data-ttu-id="57bcc-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="57bcc-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="57bcc-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="57bcc-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

