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
description: Server 要素は、イベントが発生した物理サーバーを表します。
ms.openlocfilehash: 1a5d2e223acfc402ae964c619598845e4212b639
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462046"
---
# <a name="server-messagetracking"></a><span data-ttu-id="b2edd-103">サーバー (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="b2edd-103">Server (MessageTracking)</span></span>

<span data-ttu-id="b2edd-104">**Server**要素は、イベントが発生した物理サーバーを表します。</span><span class="sxs-lookup"><span data-stu-id="b2edd-104">The **Server** element represents the physical server where the event occurred.</span></span> 
  
```XML
<Server/>
```

 <span data-ttu-id="b2edd-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="b2edd-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2edd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b2edd-106">Attributes and elements</span></span>

<span data-ttu-id="b2edd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b2edd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2edd-108">属性</span><span class="sxs-lookup"><span data-stu-id="b2edd-108">Attributes</span></span>

<span data-ttu-id="b2edd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b2edd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2edd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b2edd-110">Child elements</span></span>

<span data-ttu-id="b2edd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b2edd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2edd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b2edd-112">Parent elements</span></span>

|<span data-ttu-id="b2edd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b2edd-113">**Element**</span></span>|<span data-ttu-id="b2edd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b2edd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2edd-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="b2edd-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="b2edd-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b2edd-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b2edd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b2edd-117">Text value</span></span>

<span data-ttu-id="b2edd-118">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2edd-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b2edd-119">注釈</span><span class="sxs-lookup"><span data-stu-id="b2edd-119">Remarks</span></span>

<span data-ttu-id="b2edd-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b2edd-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2edd-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b2edd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2edd-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2edd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2edd-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b2edd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b2edd-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b2edd-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2edd-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b2edd-125">Validation File</span></span>  <br/> |<span data-ttu-id="b2edd-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b2edd-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2edd-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b2edd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2edd-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="b2edd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2edd-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2edd-129">See also</span></span>



- [<span data-ttu-id="b2edd-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b2edd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

