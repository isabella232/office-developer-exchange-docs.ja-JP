---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: RetentionAction 要素では、保持タグを持つアイテムに対して実行するアクションを指定します。
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833215"
---
# <a name="retentionaction"></a><span data-ttu-id="f058c-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="f058c-103">RetentionAction</span></span>

<span data-ttu-id="f058c-104">**RetentionAction**要素では、保持タグを持つアイテムに対して実行するアクションを指定します。</span><span class="sxs-lookup"><span data-stu-id="f058c-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="f058c-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="f058c-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f058c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f058c-106">Attributes and elements</span></span>

<span data-ttu-id="f058c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f058c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f058c-108">属性</span><span class="sxs-lookup"><span data-stu-id="f058c-108">Attributes</span></span>

<span data-ttu-id="f058c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f058c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f058c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f058c-110">Child elements</span></span>

<span data-ttu-id="f058c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f058c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f058c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f058c-112">Parent elements</span></span>

[<span data-ttu-id="f058c-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="f058c-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="f058c-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f058c-114">Text value</span></span>

<span data-ttu-id="f058c-115">**RetentionAction**要素のテキスト値は、項目に対して実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="f058c-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="f058c-116">次の一覧には、 **RetentionAction**要素のテキスト値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f058c-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="f058c-117">**なし**- 操作は必要ありませんが、項目に実行されます。</span><span class="sxs-lookup"><span data-stu-id="f058c-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="f058c-118">**MoveToDeletedItems**の項目は、既定の削除済みアイテム フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="f058c-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="f058c-119">**MoveToFolder**の項目は、指定したフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="f058c-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="f058c-120">**DeleteAndAllowRecovery**の項目が削除され、大型こみ容器に入れます。</span><span class="sxs-lookup"><span data-stu-id="f058c-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="f058c-121">**PermanentlyDelete**のアイテムはメールボックスから完全に削除します。</span><span class="sxs-lookup"><span data-stu-id="f058c-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="f058c-122">**MarkAsPastRetentionLimit**の項目は、保存期間の制限時間を超過することとしてマークされます。</span><span class="sxs-lookup"><span data-stu-id="f058c-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="f058c-123">**アーカイブに移動**- アイテムは、アーカイブ メールボックスに移動されます。</span><span class="sxs-lookup"><span data-stu-id="f058c-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="f058c-124">備考</span><span class="sxs-lookup"><span data-stu-id="f058c-124">Remarks</span></span>

<span data-ttu-id="f058c-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f058c-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f058c-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f058c-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f058c-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="f058c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f058c-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="f058c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f058c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f058c-129">Schema name</span></span>  <br/> |<span data-ttu-id="f058c-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f058c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f058c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f058c-131">Validation file</span></span>  <br/> |<span data-ttu-id="f058c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f058c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f058c-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f058c-133">Can be empty</span></span>  <br/> ||
   

