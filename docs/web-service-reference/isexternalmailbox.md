---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: IsExternalMailbox 要素は、メールボックスが組織の外部にあるかどうかを示します。
ms.openlocfilehash: cf9f71e9b955cffd1bebefd5f23acba66ba1b894
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832010"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="6faa3-103">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="6faa3-103">IsExternalMailbox</span></span>

<span data-ttu-id="6faa3-104">**IsExternalMailbox**要素は、メールボックスが組織の外部にあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6faa3-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="6faa3-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="6faa3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6faa3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6faa3-106">Attributes and elements</span></span>

<span data-ttu-id="6faa3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6faa3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6faa3-108">属性</span><span class="sxs-lookup"><span data-stu-id="6faa3-108">Attributes</span></span>

<span data-ttu-id="6faa3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6faa3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6faa3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6faa3-110">Child elements</span></span>

<span data-ttu-id="6faa3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6faa3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6faa3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6faa3-112">Parent elements</span></span>

[<span data-ttu-id="6faa3-113">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="6faa3-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="6faa3-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6faa3-114">Text value</span></span>

<span data-ttu-id="6faa3-115">の**場合は true** 、 **IsExternalMailbox**要素のテキスト値は、外部の組織内にメールボックスがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="6faa3-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="6faa3-116">**False**の値は、組織内にメールボックスがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="6faa3-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6faa3-117">備考</span><span class="sxs-lookup"><span data-stu-id="6faa3-117">Remarks</span></span>

<span data-ttu-id="6faa3-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6faa3-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6faa3-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6faa3-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6faa3-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="6faa3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6faa3-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="6faa3-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6faa3-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6faa3-122">Schema name</span></span>  <br/> |<span data-ttu-id="6faa3-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6faa3-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="6faa3-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6faa3-124">Validation file</span></span>  <br/> |<span data-ttu-id="6faa3-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6faa3-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6faa3-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6faa3-126">Can be empty</span></span>  <br/> |<span data-ttu-id="6faa3-127">False</span><span class="sxs-lookup"><span data-stu-id="6faa3-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6faa3-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="6faa3-128">See also</span></span>



- [<span data-ttu-id="6faa3-129">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6faa3-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

