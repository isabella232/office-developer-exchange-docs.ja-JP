---
title: GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4c94cfb7-42e2-42e4-9c6d-a1b0f4747f83
description: GetHoldOnMailboxes 要素は、GetHoldOnMailboxes 要求の開始を示します。
ms.openlocfilehash: f3f2cb5a83a662fc83c0a861f740571f089c10d8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458353"
---
# <a name="getholdonmailboxes"></a><span data-ttu-id="1e20d-103">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="1e20d-103">GetHoldOnMailboxes</span></span>

<span data-ttu-id="1e20d-104">**GetHoldOnMailboxes**要素は、 **GetHoldOnMailboxes**要求の開始を示します。</span><span class="sxs-lookup"><span data-stu-id="1e20d-104">The **GetHoldOnMailboxes** element indicates the beginning of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxes>
   <HoldId/>
</GetHoldOnMailboxes>
```

 <span data-ttu-id="1e20d-105">**GetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="1e20d-105">**GetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e20d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1e20d-106">Attributes and elements</span></span>

<span data-ttu-id="1e20d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1e20d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e20d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e20d-108">Attributes</span></span>

<span data-ttu-id="1e20d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1e20d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e20d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1e20d-110">Child elements</span></span>

[<span data-ttu-id="1e20d-111">HoldId</span><span class="sxs-lookup"><span data-stu-id="1e20d-111">HoldId</span></span>](holdid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="1e20d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1e20d-112">Parent elements</span></span>

<span data-ttu-id="1e20d-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1e20d-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e20d-114">注釈</span><span class="sxs-lookup"><span data-stu-id="1e20d-114">Remarks</span></span>

<span data-ttu-id="1e20d-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1e20d-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1e20d-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1e20d-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e20d-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1e20d-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e20d-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="1e20d-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e20d-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1e20d-119">Schema name</span></span>  <br/> |<span data-ttu-id="1e20d-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1e20d-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1e20d-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1e20d-121">Validation file</span></span>  <br/> |<span data-ttu-id="1e20d-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1e20d-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e20d-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1e20d-123">Can be empty</span></span>  <br/> |<span data-ttu-id="1e20d-124">false</span><span class="sxs-lookup"><span data-stu-id="1e20d-124">false</span></span>  <br/> |
   

