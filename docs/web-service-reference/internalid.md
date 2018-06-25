---
title: Internalid など
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalId
api_type:
- schema
ms.assetid: c179db1a-95c9-40da-bd3f-0bed548c0325
description: Internalid などの要素は、イベント id の整数値を表します。
ms.openlocfilehash: db547b05268d5ae2dc11be1f80a51f59b9d8e396
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831941"
---
# <a name="internalid"></a><span data-ttu-id="a22ae-103">Internalid など</span><span class="sxs-lookup"><span data-stu-id="a22ae-103">InternalId</span></span>

<span data-ttu-id="a22ae-104">**Internalid など**の要素は、イベント id の整数値を表します。</span><span class="sxs-lookup"><span data-stu-id="a22ae-104">The **InternalId** element represents an integer value for the event identification.</span></span> 
  
```XML
<InternalId/>
```

 <span data-ttu-id="a22ae-105">**nonNegativeInteger**</span><span class="sxs-lookup"><span data-stu-id="a22ae-105">**nonNegativeInteger**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a22ae-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a22ae-106">Attributes and elements</span></span>

<span data-ttu-id="a22ae-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a22ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a22ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="a22ae-108">Attributes</span></span>

<span data-ttu-id="a22ae-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a22ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a22ae-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a22ae-110">Child elements</span></span>

<span data-ttu-id="a22ae-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a22ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a22ae-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a22ae-112">Parent elements</span></span>

|<span data-ttu-id="a22ae-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a22ae-113">**Element**</span></span>|<span data-ttu-id="a22ae-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a22ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a22ae-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="a22ae-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="a22ae-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a22ae-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a22ae-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a22ae-117">Text value</span></span>

<span data-ttu-id="a22ae-118">整数値を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="a22ae-118">A text value that represents an integer is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a22ae-119">備考</span><span class="sxs-lookup"><span data-stu-id="a22ae-119">Remarks</span></span>

<span data-ttu-id="a22ae-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a22ae-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a22ae-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="a22ae-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a22ae-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="a22ae-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a22ae-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a22ae-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a22ae-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a22ae-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="a22ae-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a22ae-125">Validation File</span></span>  <br/> |<span data-ttu-id="a22ae-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a22ae-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a22ae-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a22ae-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a22ae-128">False</span><span class="sxs-lookup"><span data-stu-id="a22ae-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a22ae-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a22ae-129">See also</span></span>



- [<span data-ttu-id="a22ae-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a22ae-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

