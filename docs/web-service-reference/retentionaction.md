---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: RetentionAction 要素は、保持タグを持つアイテムに対して実行されるアクションを指定します。
ms.openlocfilehash: c16988413e732ddc3cd6ebc355cb73c4d96550c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465234"
---
# <a name="retentionaction"></a><span data-ttu-id="9259c-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="9259c-103">RetentionAction</span></span>

<span data-ttu-id="9259c-104">**Retentionaction**要素は、保持タグを持つアイテムに対して実行されるアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="9259c-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="9259c-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="9259c-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9259c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9259c-106">Attributes and elements</span></span>

<span data-ttu-id="9259c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9259c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9259c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9259c-108">Attributes</span></span>

<span data-ttu-id="9259c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9259c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9259c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9259c-110">Child elements</span></span>

<span data-ttu-id="9259c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9259c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9259c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9259c-112">Parent elements</span></span>

[<span data-ttu-id="9259c-113">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="9259c-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="9259c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9259c-114">Text value</span></span>

<span data-ttu-id="9259c-115">**Retentionaction**要素のテキスト値は、アイテムに対して実行されるアクションです。</span><span class="sxs-lookup"><span data-stu-id="9259c-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="9259c-116">次の一覧に、 **Retentionaction**要素のテキスト値を示します。</span><span class="sxs-lookup"><span data-stu-id="9259c-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="9259c-117">**None** -アイテムに対してアクションは実行されません。</span><span class="sxs-lookup"><span data-stu-id="9259c-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="9259c-118">**MoveToDeletedItems** -アイテムは既定の削除済みアイテムフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="9259c-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="9259c-119">**Movetofolder** -アイテムは指定されたフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="9259c-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="9259c-120">**Deleteandallowrecovery** -アイテムが削除され、[収集] に入ります。</span><span class="sxs-lookup"><span data-stu-id="9259c-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="9259c-121">**PermanentlyDelete** -アイテムはメールボックスから完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="9259c-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="9259c-122">**MarkAsPastRetentionLimit** -アイテムは、保持時間制限を超えたとしてマークされています。</span><span class="sxs-lookup"><span data-stu-id="9259c-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="9259c-123">**Movetoarchive** -アイテムはアーカイブメールボックスに移動されます。</span><span class="sxs-lookup"><span data-stu-id="9259c-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="9259c-124">注釈</span><span class="sxs-lookup"><span data-stu-id="9259c-124">Remarks</span></span>

<span data-ttu-id="9259c-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9259c-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9259c-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9259c-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9259c-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9259c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9259c-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="9259c-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9259c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9259c-129">Schema name</span></span>  <br/> |<span data-ttu-id="9259c-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9259c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9259c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9259c-131">Validation file</span></span>  <br/> |<span data-ttu-id="9259c-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9259c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9259c-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9259c-133">Can be empty</span></span>  <br/> ||
   

