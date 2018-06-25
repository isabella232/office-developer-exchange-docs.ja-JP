---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: IncludeNonIndexableItems 要素には、インデックスを作成できないアイテムを含めるかどうかを示すブール値が含まれています。
ms.openlocfilehash: ae91a3c6db82aea1d45940603d0ff2064d29f43f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831904"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="b6b43-103">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="b6b43-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="b6b43-104">**IncludeNonIndexableItems**要素には、インデックスを作成できないアイテムを含めるかどうかを示す**ブール**値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6b43-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="b6b43-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="b6b43-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6b43-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b6b43-106">Attributes and elements</span></span>

<span data-ttu-id="b6b43-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6b43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6b43-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6b43-108">Attributes</span></span>

<span data-ttu-id="b6b43-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b6b43-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6b43-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b6b43-110">Child elements</span></span>

<span data-ttu-id="b6b43-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b6b43-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6b43-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b6b43-112">Parent elements</span></span>

[<span data-ttu-id="b6b43-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="b6b43-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="b6b43-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b6b43-114">Text value</span></span>

<span data-ttu-id="b6b43-115">の**場合は true** 、 **IncludeNonIndexableItems**要素のテキスト値は、インデックスを作成できないアイテムはメールボックスの保留リストに含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="b6b43-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="b6b43-116">**False**の値は、メールボックスの保留リストにインデックスを作成できない項目が含まれていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b6b43-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b6b43-117">備考</span><span class="sxs-lookup"><span data-stu-id="b6b43-117">Remarks</span></span>

<span data-ttu-id="b6b43-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b6b43-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6b43-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b6b43-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6b43-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="b6b43-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6b43-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="b6b43-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b6b43-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6b43-122">Schema name</span></span>  <br/> |<span data-ttu-id="b6b43-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6b43-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b6b43-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6b43-124">Validation file</span></span>  <br/> |<span data-ttu-id="b6b43-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b6b43-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b6b43-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b6b43-126">Can be empty</span></span>  <br/> |<span data-ttu-id="b6b43-127">false</span><span class="sxs-lookup"><span data-stu-id="b6b43-127">false</span></span>  <br/> |
   

