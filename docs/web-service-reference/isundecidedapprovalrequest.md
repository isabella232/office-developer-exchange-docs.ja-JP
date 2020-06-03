---
title: Is未確認 Dedapprovalrequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: Is未確認の Dedapprovalrequest 要素は、承認要求メッセージが処理されたかどうかを指定します。
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458174"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="29154-103">Is未確認 Dedapprovalrequest</span><span class="sxs-lookup"><span data-stu-id="29154-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="29154-104">**Is未確認の Dedapprovalrequest**要素は、承認要求メッセージが処理されたかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="29154-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="29154-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="29154-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29154-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="29154-106">Attributes and elements</span></span>

<span data-ttu-id="29154-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="29154-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29154-108">属性</span><span class="sxs-lookup"><span data-stu-id="29154-108">Attributes</span></span>

<span data-ttu-id="29154-109">なし。</span><span class="sxs-lookup"><span data-stu-id="29154-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29154-110">子要素</span><span class="sxs-lookup"><span data-stu-id="29154-110">Child elements</span></span>

<span data-ttu-id="29154-111">なし。</span><span class="sxs-lookup"><span data-stu-id="29154-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29154-112">親要素</span><span class="sxs-lookup"><span data-stu-id="29154-112">Parent elements</span></span>

[<span data-ttu-id="29154-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="29154-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="29154-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="29154-114">Text value</span></span>

<span data-ttu-id="29154-115">承認要求メッセージが処理されていない場合は、 **is不明な Dedapprovalrequest**要素のテキスト値は**true**です。</span><span class="sxs-lookup"><span data-stu-id="29154-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="29154-116">値が**false**の場合は、承認要求が決定されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="29154-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="29154-117">注釈</span><span class="sxs-lookup"><span data-stu-id="29154-117">Remarks</span></span>

<span data-ttu-id="29154-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="29154-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="29154-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="29154-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29154-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="29154-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29154-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="29154-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="29154-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="29154-122">Schema Name</span></span>  <br/> |<span data-ttu-id="29154-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="29154-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="29154-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="29154-124">Validation File</span></span>  <br/> |<span data-ttu-id="29154-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="29154-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="29154-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="29154-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="29154-127">正しい</span><span class="sxs-lookup"><span data-stu-id="29154-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29154-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="29154-128">See also</span></span>



[<span data-ttu-id="29154-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="29154-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="29154-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="29154-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

