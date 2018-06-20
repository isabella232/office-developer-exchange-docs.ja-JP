---
title: 状態 (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: 状態の要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833579"
---
# <a name="status-holdstatustype"></a><span data-ttu-id="7f37a-103">状態 (HoldStatusType)</span><span class="sxs-lookup"><span data-stu-id="7f37a-103">Status (HoldStatusType)</span></span>

<span data-ttu-id="7f37a-104">**状態**の要素は、メールボックスの保留状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f37a-104">The **Status** element specifies the hold status for a mailbox.</span></span> 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 <span data-ttu-id="7f37a-105">**HoldStatusType**</span><span class="sxs-lookup"><span data-stu-id="7f37a-105">**HoldStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f37a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f37a-106">Attributes and elements</span></span>

<span data-ttu-id="7f37a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f37a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f37a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f37a-108">Attributes</span></span>

<span data-ttu-id="7f37a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f37a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f37a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f37a-110">Child elements</span></span>

<span data-ttu-id="7f37a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7f37a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f37a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7f37a-112">Parent elements</span></span>

[<span data-ttu-id="7f37a-113">MailboxHoldStatus</span><span class="sxs-lookup"><span data-stu-id="7f37a-113">MailboxHoldStatus</span></span>](mailboxholdstatus.md)
  
## <a name="text-value"></a><span data-ttu-id="7f37a-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f37a-114">Text value</span></span>

<span data-ttu-id="7f37a-115">**状態**の要素のテキスト値は、メールボックスの保留状態です。</span><span class="sxs-lookup"><span data-stu-id="7f37a-115">The text value of the **Status** element is the hold status of a mailbox.</span></span> <span data-ttu-id="7f37a-116">**状態**の要素は、次の一覧に値を持つことができます。</span><span class="sxs-lookup"><span data-stu-id="7f37a-116">The **Status** element can have the values in the following list.</span></span> 
  
> <span data-ttu-id="7f37a-117">NotOnHold - メールボックスは保留状態にします。</span><span class="sxs-lookup"><span data-stu-id="7f37a-117">NotOnHold - The mailbox is not on hold.</span></span>
    
> <span data-ttu-id="7f37a-118">保留中のメールボックスは、保留中のいずれかが配置または保留中のリリースです。</span><span class="sxs-lookup"><span data-stu-id="7f37a-118">Pending - The mailbox is pending either being placed or released on hold.</span></span> 
    
> <span data-ttu-id="7f37a-119">OnHold - 保留リストは、メールボックスに正常に適用されました。</span><span class="sxs-lookup"><span data-stu-id="7f37a-119">OnHold - The hold was successfully applied to the mailbox.</span></span> 
    
> <span data-ttu-id="7f37a-120">PartialHold - 保留リストには、すべてのメールボックスではなく、一部のメールボックスに正しく適用されました。</span><span class="sxs-lookup"><span data-stu-id="7f37a-120">PartialHold - The hold was successfully applied to some mailboxes but not to all mailboxes.</span></span>
    
> <span data-ttu-id="7f37a-121">保留に失敗しました - メールボックスに適用できませんでした。</span><span class="sxs-lookup"><span data-stu-id="7f37a-121">Failed - The hold failed to apply to the mailbox.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7f37a-122">備考</span><span class="sxs-lookup"><span data-stu-id="7f37a-122">Remarks</span></span>

<span data-ttu-id="7f37a-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7f37a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f37a-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7f37a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f37a-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f37a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f37a-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f37a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f37a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f37a-127">Schema name</span></span>  <br/> |<span data-ttu-id="7f37a-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7f37a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f37a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f37a-129">Validation file</span></span>  <br/> |<span data-ttu-id="7f37a-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7f37a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f37a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7f37a-131">Can be empty</span></span>  <br/> ||
   

