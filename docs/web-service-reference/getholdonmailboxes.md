---
title: GetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4c94cfb7-42e2-42e4-9c6d-a1b0f4747f83
description: GetHoldOnMailboxes 要素は、GetHoldOnMailboxes 要求の先頭を示します。
ms.openlocfilehash: 844fe18e983223a014fed2043452c18b1e5ac465
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760745"
---
# <a name="getholdonmailboxes"></a><span data-ttu-id="7e2e2-103">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="7e2e2-103">GetHoldOnMailboxes</span></span>

<span data-ttu-id="7e2e2-104">**GetHoldOnMailboxes**要素は、 **GetHoldOnMailboxes**要求の先頭を示します。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-104">The **GetHoldOnMailboxes** element indicates the beginning of the **GetHoldOnMailboxes** request.</span></span> 
  
```XML
<GetHoldOnMailboxes>
   <HoldId/>
</GetHoldOnMailboxes>
```

 <span data-ttu-id="7e2e2-105">**GetHoldOnMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="7e2e2-105">**GetHoldOnMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e2e2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e2e2-106">Attributes and elements</span></span>

<span data-ttu-id="7e2e2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e2e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e2e2-108">Attributes</span></span>

<span data-ttu-id="7e2e2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e2e2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e2e2-110">Child elements</span></span>

[<span data-ttu-id="7e2e2-111">HoldId</span><span class="sxs-lookup"><span data-stu-id="7e2e2-111">HoldId</span></span>](holdid.md)
  
### <a name="parent-elements"></a><span data-ttu-id="7e2e2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e2e2-112">Parent elements</span></span>

<span data-ttu-id="7e2e2-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e2e2-114">解説</span><span class="sxs-lookup"><span data-stu-id="7e2e2-114">Remarks</span></span>

<span data-ttu-id="7e2e2-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e2e2-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e2e2-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e2e2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e2e2-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e2e2-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e2e2-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e2e2-119">Schema name</span></span>  <br/> |<span data-ttu-id="7e2e2-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7e2e2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e2e2-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e2e2-121">Validation file</span></span>  <br/> |<span data-ttu-id="7e2e2-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e2e2-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e2e2-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e2e2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="7e2e2-124">false</span><span class="sxs-lookup"><span data-stu-id="7e2e2-124">false</span></span>  <br/> |
   

