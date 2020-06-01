---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: State 要素には、サイトメールボックスに設定されているライフサイクル状態が含まれます。
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465164"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="15618-103">State (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="15618-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="15618-104">**State**要素には、サイトメールボックスに設定されているライフサイクル状態が含まれます。</span><span class="sxs-lookup"><span data-stu-id="15618-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="15618-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="15618-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15618-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="15618-106">Attributes and elements</span></span>

<span data-ttu-id="15618-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15618-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15618-108">属性</span><span class="sxs-lookup"><span data-stu-id="15618-108">Attributes</span></span>

<span data-ttu-id="15618-109">なし。</span><span class="sxs-lookup"><span data-stu-id="15618-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15618-110">子要素</span><span class="sxs-lookup"><span data-stu-id="15618-110">Child elements</span></span>

<span data-ttu-id="15618-111">なし。</span><span class="sxs-lookup"><span data-stu-id="15618-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15618-112">親要素</span><span class="sxs-lookup"><span data-stu-id="15618-112">Parent elements</span></span>

[<span data-ttu-id="15618-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="15618-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="15618-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="15618-114">Text value</span></span>

<span data-ttu-id="15618-115">**State**要素のテキスト値は、サイトメールボックスに設定されているライフサイクル状態です。</span><span class="sxs-lookup"><span data-stu-id="15618-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="15618-116">**Active**のテキスト値は、サイトメールボックスがアクティブに使用されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="15618-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="15618-117">テキスト値**closed**は、サイトメールボックスが閉じられていて、使用中ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="15618-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="15618-118">**リンク**のないテキスト値は、サイトメールボックスが web ベースのグループ作業環境にリンクされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="15618-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="15618-119">**アクティブ**、**クローズ**、および**PendingDelete**の値は相互に排他的ですが、**リンク**されていない値は他の値を相互排他的にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="15618-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="15618-120">テキスト値の**PendingDelete**は、サイトメールボックスが削除を保留していることを示します。</span><span class="sxs-lookup"><span data-stu-id="15618-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="15618-121">サイトメールボックスは、 **PendingDelete**として設定する前に閉じる必要があります。</span><span class="sxs-lookup"><span data-stu-id="15618-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15618-122">注釈</span><span class="sxs-lookup"><span data-stu-id="15618-122">Remarks</span></span>

<span data-ttu-id="15618-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="15618-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="15618-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="15618-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15618-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="15618-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15618-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="15618-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15618-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15618-127">Schema name</span></span>  <br/> |<span data-ttu-id="15618-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="15618-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="15618-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15618-129">Validation file</span></span>  <br/> |<span data-ttu-id="15618-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="15618-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15618-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="15618-131">Can be empty</span></span>  <br/> ||
   

