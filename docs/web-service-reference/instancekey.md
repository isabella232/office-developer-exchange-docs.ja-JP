---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: InstanceKey 要素は、アイテムまたは会話のインスタンス キーを指定します。
ms.openlocfilehash: a0e4f9390d5dc368388b5a20e38796c6c0157a40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831943"
---
# <a name="instancekey"></a><span data-ttu-id="fc8d3-103">InstanceKey</span><span class="sxs-lookup"><span data-stu-id="fc8d3-103">InstanceKey</span></span>

<span data-ttu-id="fc8d3-104">**InstanceKey**要素は、アイテムまたは会話のインスタンス キーを指定します。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-104">The **InstanceKey** element specifies an instance key for an item or conversation.</span></span> 
  
```XML
<InstanceKey></InstanceKey>
```

 <span data-ttu-id="fc8d3-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="fc8d3-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc8d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fc8d3-106">Attributes and elements</span></span>

<span data-ttu-id="fc8d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc8d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc8d3-108">Attributes</span></span>

<span data-ttu-id="fc8d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc8d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fc8d3-110">Child elements</span></span>

<span data-ttu-id="fc8d3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc8d3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fc8d3-112">Parent elements</span></span>

|<span data-ttu-id="fc8d3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fc8d3-113">**Element**</span></span>|<span data-ttu-id="fc8d3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fc8d3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc8d3-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="fc8d3-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="fc8d3-116">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="fc8d3-117">アイテム</span><span class="sxs-lookup"><span data-stu-id="fc8d3-117">Item</span></span>](item.md) <br/> |<span data-ttu-id="fc8d3-118">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-118">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc8d3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fc8d3-119">Text value</span></span>

<span data-ttu-id="fc8d3-120">**InstanceKey**要素のテキスト値は、アイテムまたは会話のインスタンス キーです。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-120">The text value of the **InstanceKey** element is the instance key for an item or conversation.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fc8d3-121">備考</span><span class="sxs-lookup"><span data-stu-id="fc8d3-121">Remarks</span></span>

<span data-ttu-id="fc8d3-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fc8d3-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc8d3-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="fc8d3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc8d3-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="fc8d3-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc8d3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fc8d3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fc8d3-127">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="fc8d3-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="fc8d3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fc8d3-128">Validation File</span></span>  <br/> |<span data-ttu-id="fc8d3-129">types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc8d3-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc8d3-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fc8d3-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fc8d3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc8d3-131">See also</span></span>



- [<span data-ttu-id="fc8d3-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fc8d3-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

