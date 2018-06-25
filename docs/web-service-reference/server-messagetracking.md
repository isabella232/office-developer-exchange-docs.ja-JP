---
title: サーバー (MessageTracking)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Server
api_type:
- schema
ms.assetid: eb5408bd-6fa5-4415-9224-24d5e07ec5b3
description: サーバー要素は、イベントが発生した物理サーバーを表します。
ms.openlocfilehash: 95117eb2b5d195bc8b7ff90098e4138b67722f28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833372"
---
# <a name="server-messagetracking"></a><span data-ttu-id="9cbeb-103">サーバー (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="9cbeb-103">Server (MessageTracking)</span></span>

<span data-ttu-id="9cbeb-104">**サーバー**要素は、イベントが発生した物理サーバーを表します。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-104">The **Server** element represents the physical server where the event occurred.</span></span> 
  
```XML
<Server/>
```

 <span data-ttu-id="9cbeb-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="9cbeb-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cbeb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9cbeb-106">Attributes and elements</span></span>

<span data-ttu-id="9cbeb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cbeb-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cbeb-108">Attributes</span></span>

<span data-ttu-id="9cbeb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cbeb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9cbeb-110">Child elements</span></span>

<span data-ttu-id="9cbeb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cbeb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9cbeb-112">Parent elements</span></span>

|<span data-ttu-id="9cbeb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9cbeb-113">**Element**</span></span>|<span data-ttu-id="9cbeb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cbeb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cbeb-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="9cbeb-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="9cbeb-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cbeb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9cbeb-117">Text value</span></span>

<span data-ttu-id="9cbeb-118">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9cbeb-119">備考</span><span class="sxs-lookup"><span data-stu-id="9cbeb-119">Remarks</span></span>

<span data-ttu-id="9cbeb-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9cbeb-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cbeb-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="9cbeb-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cbeb-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="9cbeb-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cbeb-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9cbeb-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9cbeb-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9cbeb-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9cbeb-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9cbeb-125">Validation File</span></span>  <br/> |<span data-ttu-id="9cbeb-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9cbeb-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cbeb-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9cbeb-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cbeb-128">False</span><span class="sxs-lookup"><span data-stu-id="9cbeb-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cbeb-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9cbeb-129">See also</span></span>



- [<span data-ttu-id="9cbeb-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9cbeb-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

