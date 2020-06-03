---
title: 状態 (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Status 要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459988"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="0835f-103">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="0835f-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="0835f-104">**Status**要素は、メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="0835f-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="0835f-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="0835f-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0835f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0835f-106">Attributes and elements</span></span>

<span data-ttu-id="0835f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0835f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0835f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0835f-108">Attributes</span></span>

<span data-ttu-id="0835f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0835f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0835f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0835f-110">Child elements</span></span>

<span data-ttu-id="0835f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0835f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0835f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0835f-112">Parent elements</span></span>

[<span data-ttu-id="0835f-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="0835f-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="0835f-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0835f-114">Text value</span></span>

<span data-ttu-id="0835f-115">**Status**要素のテキスト値は、メールボックスの保持状態です。</span><span class="sxs-lookup"><span data-stu-id="0835f-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="0835f-116">**Status**要素には、次のリストの値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="0835f-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="0835f-117">NotOnHold-メールボックスは保持されていません。</span><span class="sxs-lookup"><span data-stu-id="0835f-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="0835f-118">保留中-メールボックスは保留中または保留中のどちらかが保留中です。</span><span class="sxs-lookup"><span data-stu-id="0835f-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="0835f-119">OnHold-メールボックスに保留が正常に適用されました。</span><span class="sxs-lookup"><span data-stu-id="0835f-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="0835f-120">PartialHold-一部のメールボックスに対して保留が正常に適用されましたが、すべてのメールボックスに適用されていません。</span><span class="sxs-lookup"><span data-stu-id="0835f-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="0835f-121">Failed-保留リストをメールボックスに適用できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0835f-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0835f-122">注釈</span><span class="sxs-lookup"><span data-stu-id="0835f-122">Remarks</span></span>

<span data-ttu-id="0835f-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0835f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0835f-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0835f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0835f-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0835f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0835f-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0835f-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0835f-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0835f-127">Schema name</span></span>  <br/> |<span data-ttu-id="0835f-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0835f-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0835f-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0835f-129">Validation file</span></span>  <br/> |<span data-ttu-id="0835f-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0835f-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0835f-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0835f-131">Can be empty</span></span>  <br/> ||
   

