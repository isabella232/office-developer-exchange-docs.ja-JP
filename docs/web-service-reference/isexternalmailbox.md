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
ms.openlocfilehash: 9be702b05e89857913023a8ec34b78ea4c309274
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455290"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="821c9-103">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="821c9-103">IsExternalMailbox</span></span>

<span data-ttu-id="821c9-104">**IsExternalMailbox**要素は、メールボックスが組織の外部にあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="821c9-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="821c9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="821c9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="821c9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="821c9-106">Attributes and elements</span></span>

<span data-ttu-id="821c9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="821c9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="821c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="821c9-108">Attributes</span></span>

<span data-ttu-id="821c9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="821c9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="821c9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="821c9-110">Child elements</span></span>

<span data-ttu-id="821c9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="821c9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="821c9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="821c9-112">Parent elements</span></span>

[<span data-ttu-id="821c9-113">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="821c9-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="821c9-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="821c9-114">Text value</span></span>

<span data-ttu-id="821c9-115">**IsExternalMailbox**要素のテキスト値が**true の場合**は、メールボックスが外部組織にあることを示します。</span><span class="sxs-lookup"><span data-stu-id="821c9-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="821c9-116">値が**false**の場合は、メールボックスが組織内にあることを示します。</span><span class="sxs-lookup"><span data-stu-id="821c9-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="821c9-117">注釈</span><span class="sxs-lookup"><span data-stu-id="821c9-117">Remarks</span></span>

<span data-ttu-id="821c9-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="821c9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="821c9-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="821c9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="821c9-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="821c9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="821c9-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="821c9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="821c9-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="821c9-122">Schema name</span></span>  <br/> |<span data-ttu-id="821c9-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="821c9-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="821c9-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="821c9-124">Validation file</span></span>  <br/> |<span data-ttu-id="821c9-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="821c9-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="821c9-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="821c9-126">Can be empty</span></span>  <br/> |<span data-ttu-id="821c9-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="821c9-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="821c9-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="821c9-128">See also</span></span>



- [<span data-ttu-id="821c9-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="821c9-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

