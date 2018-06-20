---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: IsUndecidedApprovalRequest 要素は、承認要求メッセージが処理済みであるかどうかを指定します。
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832127"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="a4dee-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="a4dee-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="a4dee-104">**IsUndecidedApprovalRequest**要素は、承認要求メッセージが処理済みであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="a4dee-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="a4dee-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="a4dee-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4dee-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a4dee-106">Attributes and elements</span></span>

<span data-ttu-id="a4dee-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4dee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4dee-108">属性</span><span class="sxs-lookup"><span data-stu-id="a4dee-108">Attributes</span></span>

<span data-ttu-id="a4dee-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a4dee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4dee-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a4dee-110">Child elements</span></span>

<span data-ttu-id="a4dee-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a4dee-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4dee-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a4dee-112">Parent elements</span></span>

[<span data-ttu-id="a4dee-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="a4dee-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="a4dee-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4dee-114">Text value</span></span>

<span data-ttu-id="a4dee-115">**承認要求メッセージが処理済みいない場合、 **IsUndecidedApprovalRequest**要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="a4dee-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="a4dee-116">**False**の値は、承認要求が決定されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="a4dee-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4dee-117">備考</span><span class="sxs-lookup"><span data-stu-id="a4dee-117">Remarks</span></span>

<span data-ttu-id="a4dee-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a4dee-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="a4dee-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a4dee-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4dee-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="a4dee-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4dee-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="a4dee-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4dee-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4dee-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a4dee-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a4dee-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4dee-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4dee-124">Validation File</span></span>  <br/> |<span data-ttu-id="a4dee-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4dee-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4dee-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a4dee-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4dee-127">True</span><span class="sxs-lookup"><span data-stu-id="a4dee-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4dee-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4dee-128">See also</span></span>



[<span data-ttu-id="a4dee-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="a4dee-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="a4dee-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4dee-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

