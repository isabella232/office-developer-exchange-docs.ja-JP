---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: ActionType 要素は、保留のアクションの種類を示します。
ms.openlocfilehash: 8f2796df818dac2bd285b055aa44fbcecd0de5e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457859"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="f8fdf-103">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="f8fdf-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="f8fdf-104">**ActionType**要素は、保留のアクションの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="f8fdf-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="f8fdf-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8fdf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f8fdf-106">Attributes and elements</span></span>

<span data-ttu-id="f8fdf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8fdf-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8fdf-108">Attributes</span></span>

<span data-ttu-id="f8fdf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8fdf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f8fdf-110">Child elements</span></span>

<span data-ttu-id="f8fdf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8fdf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f8fdf-112">Parent elements</span></span>

[<span data-ttu-id="f8fdf-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="f8fdf-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="f8fdf-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f8fdf-114">Text value</span></span>

<span data-ttu-id="f8fdf-115">**ActionType**要素のテキスト値は、メールボックスの保留セットの種類です。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="f8fdf-116">**Create**のテキスト値は、メールボックスの保持が作成されることを示します。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="f8fdf-117">**Update**のテキスト値は、メールボックスの保持が更新されることを示します。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="f8fdf-118">テキスト値**Remove**は、メールボックスの保持が削除されることを示します。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f8fdf-119">注釈</span><span class="sxs-lookup"><span data-stu-id="f8fdf-119">Remarks</span></span>

<span data-ttu-id="f8fdf-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f8fdf-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8fdf-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f8fdf-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8fdf-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8fdf-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8fdf-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f8fdf-124">Schema name</span></span>  <br/> |<span data-ttu-id="f8fdf-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f8fdf-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8fdf-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f8fdf-126">Validation file</span></span>  <br/> |<span data-ttu-id="f8fdf-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f8fdf-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8fdf-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f8fdf-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f8fdf-129">false</span><span class="sxs-lookup"><span data-stu-id="f8fdf-129">false</span></span>  <br/> |
   

