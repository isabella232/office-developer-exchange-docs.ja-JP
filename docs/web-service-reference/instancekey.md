---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: InstanceKey 要素は、アイテムまたはスレッドのインスタンスキーを指定します。
ms.openlocfilehash: a6b55b9021fe63be7f678f0a1bcb24e88aeba005
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459974"
---
# <a name="instancekey"></a><span data-ttu-id="1a980-103">InstanceKey</span><span class="sxs-lookup"><span data-stu-id="1a980-103">InstanceKey</span></span>

<span data-ttu-id="1a980-104">**InstanceKey**要素は、アイテムまたはスレッドのインスタンスキーを指定します。</span><span class="sxs-lookup"><span data-stu-id="1a980-104">The **InstanceKey** element specifies an instance key for an item or conversation.</span></span> 
  
```XML
<InstanceKey></InstanceKey>
```

 <span data-ttu-id="1a980-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="1a980-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a980-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1a980-106">Attributes and elements</span></span>

<span data-ttu-id="1a980-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a980-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a980-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a980-108">Attributes</span></span>

<span data-ttu-id="1a980-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a980-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a980-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a980-110">Child elements</span></span>

<span data-ttu-id="1a980-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1a980-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a980-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1a980-112">Parent elements</span></span>

|<span data-ttu-id="1a980-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a980-113">**Element**</span></span>|<span data-ttu-id="1a980-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a980-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a980-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="1a980-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="1a980-116">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="1a980-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="1a980-117">Item</span><span class="sxs-lookup"><span data-stu-id="1a980-117">Item</span></span>](item.md) <br/> |<span data-ttu-id="1a980-118">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1a980-118">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a980-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1a980-119">Text value</span></span>

<span data-ttu-id="1a980-120">**InstanceKey**要素のテキスト値は、アイテムまたはスレッドのインスタンスキーです。</span><span class="sxs-lookup"><span data-stu-id="1a980-120">The text value of the **InstanceKey** element is the instance key for an item or conversation.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1a980-121">注釈</span><span class="sxs-lookup"><span data-stu-id="1a980-121">Remarks</span></span>

<span data-ttu-id="1a980-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1a980-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1a980-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1a980-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a980-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1a980-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a980-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a980-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a980-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a980-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1a980-127">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="1a980-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="1a980-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a980-128">Validation File</span></span>  <br/> |<span data-ttu-id="1a980-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1a980-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a980-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1a980-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1a980-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a980-131">See also</span></span>



- [<span data-ttu-id="1a980-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a980-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

