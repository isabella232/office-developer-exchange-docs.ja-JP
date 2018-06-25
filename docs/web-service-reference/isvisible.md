---
title: IsVisible
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 403acdd5-3b79-46f4-9894-ba57e10085e4
description: IsVisible 要素では、リテンション ・ ポリシーがユーザーに表示するかどうかを示します。
ms.openlocfilehash: c08b8a3d537c062d3a1a8ed59823bc0f74eea426
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832133"
---
# <a name="isvisible"></a><span data-ttu-id="9ffe7-103">IsVisible</span><span class="sxs-lookup"><span data-stu-id="9ffe7-103">IsVisible</span></span>

<span data-ttu-id="9ffe7-104">**IsVisible**要素では、リテンション ・ ポリシーがユーザーに表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-104">The **IsVisible** element indicates whether the retention policy is visible to users.</span></span> 
  
```XML
<IsVisible> true | false</IsVisible>
```

 <span data-ttu-id="9ffe7-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9ffe7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ffe7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ffe7-106">Attributes and elements</span></span>

<span data-ttu-id="9ffe7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ffe7-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ffe7-108">Attributes</span></span>

<span data-ttu-id="9ffe7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ffe7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9ffe7-110">Child elements</span></span>

<span data-ttu-id="9ffe7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ffe7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9ffe7-112">Parent elements</span></span>

[<span data-ttu-id="9ffe7-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="9ffe7-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="9ffe7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9ffe7-114">Text value</span></span>

<span data-ttu-id="9ffe7-115">の場合**は true。** **IsVisible**要素のテキスト値では、リテンション ・ ポリシーは、ユーザーに表示されることを示します。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-115">A text value of **true** for the **IsVisible** element indicates that the retention policy is visible to a user.</span></span> <span data-ttu-id="9ffe7-116">**False**の値では、リテンション ・ ポリシーがユーザーに表示されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-116">A value of **false** indicates the retention policy is not visible to users.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9ffe7-117">備考</span><span class="sxs-lookup"><span data-stu-id="9ffe7-117">Remarks</span></span>

<span data-ttu-id="9ffe7-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9ffe7-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9ffe7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

