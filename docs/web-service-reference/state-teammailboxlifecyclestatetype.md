---
title: 状態 (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: State 要素には、サイトのメールボックスに設定されているライフ サイクル状態が含まれています。
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833571"
---
# <a name="state-teammailboxlifecyclestatetype"></a><span data-ttu-id="39d3f-103">状態 (TeamMailboxLifecycleStateType)</span><span class="sxs-lookup"><span data-stu-id="39d3f-103">State (TeamMailboxLifecycleStateType)</span></span>

<span data-ttu-id="39d3f-104">**State**要素には、サイトのメールボックスに設定されているライフ サイクル状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39d3f-104">The **State** element contains the lifecycle state that is set on a site mailbox.</span></span> 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

<span data-ttu-id="39d3f-105">**TeamMailboxLifecycleStateType**</span><span class="sxs-lookup"><span data-stu-id="39d3f-105">**TeamMailboxLifecycleStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="39d3f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="39d3f-106">Attributes and elements</span></span>

<span data-ttu-id="39d3f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="39d3f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39d3f-108">属性</span><span class="sxs-lookup"><span data-stu-id="39d3f-108">Attributes</span></span>

<span data-ttu-id="39d3f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="39d3f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39d3f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="39d3f-110">Child elements</span></span>

<span data-ttu-id="39d3f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="39d3f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="39d3f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="39d3f-112">Parent elements</span></span>

[<span data-ttu-id="39d3f-113">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="39d3f-113">SetTeamMailbox</span></span>](setteammailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="39d3f-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="39d3f-114">Text value</span></span>

<span data-ttu-id="39d3f-115">**状態**の要素のテキスト値は、サイトのメールボックスに設定されているライフ サイクル状態です。</span><span class="sxs-lookup"><span data-stu-id="39d3f-115">The text value of the **State** element is the lifecycle state that is set on a site mailbox.</span></span> <span data-ttu-id="39d3f-116">**作業中**のテキスト値は、サイトのメールボックスが使用中でことを示します。</span><span class="sxs-lookup"><span data-stu-id="39d3f-116">A text value of **Active** indicates that a site mailbox is in active use.</span></span> <span data-ttu-id="39d3f-117">**終了**のテキスト値は、サイトのメールボックスが閉じられたアクティブな使用されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="39d3f-117">A text value of **Closed** indicates that a site mailbox has been closed and is not in active use.</span></span> <span data-ttu-id="39d3f-118">**リンクのない**のテキスト値は、サイトのメールボックスが、web ベースのコラボレーション環境にリンクされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="39d3f-118">A text value of **Unlinked** indicates that a site mailbox is not linked to a web-based collaboration environment.</span></span> <span data-ttu-id="39d3f-119">**アクティブ**、**終了**、および**PendingDelete**の値は、相互に排他的ですが、**リンクのない**値は互いに他の値を除く。</span><span class="sxs-lookup"><span data-stu-id="39d3f-119">The **Active**, **Closed**, and **PendingDelete** values are mutually exclusive, but the **Unlinked** value is not mutually exclusive of the other values.</span></span> <span data-ttu-id="39d3f-120">**PendingDelete**のテキスト値は、サイトのメールボックスが削除は保留されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="39d3f-120">A text value of **PendingDelete** indicates that a site mailbox is pending deletion.</span></span> <span data-ttu-id="39d3f-121">サイトのメールボックスには**PendingDelete**に設定することができます前に閉じる。</span><span class="sxs-lookup"><span data-stu-id="39d3f-121">A site mailbox has to be closed before it can be set as **PendingDelete**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39d3f-122">備考</span><span class="sxs-lookup"><span data-stu-id="39d3f-122">Remarks</span></span>

<span data-ttu-id="39d3f-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="39d3f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="39d3f-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="39d3f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39d3f-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="39d3f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39d3f-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="39d3f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39d3f-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="39d3f-127">Schema name</span></span>  <br/> |<span data-ttu-id="39d3f-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="39d3f-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39d3f-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="39d3f-129">Validation file</span></span>  <br/> |<span data-ttu-id="39d3f-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="39d3f-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39d3f-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="39d3f-131">Can be empty</span></span>  <br/> ||
   

