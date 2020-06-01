---
title: IntendedFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IntendedFreeBusyStatus
api_type:
- schema
ms.assetid: 0e0fa898-69a4-4c57-8bb2-52f716b5b478
description: IntendedFreeBusyStatus 要素は、会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。
ms.openlocfilehash: c5502bcfb308aa2f02a9575ab43f80261b5fa4ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465619"
---
# <a name="intendedfreebusystatus"></a><span data-ttu-id="5a53f-103">IntendedFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5a53f-103">IntendedFreeBusyStatus</span></span>

<span data-ttu-id="5a53f-104">**IntendedFreeBusyStatus**要素は、会議出席依頼に関連付けられている予定表アイテムの目的の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5a53f-104">The **IntendedFreeBusyStatus** element represents the intended status for the calendar item that is associated with the meeting request.</span></span> 
  
```xml
<IntendedFreeBusyStatus/>
```

 <span data-ttu-id="5a53f-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="5a53f-105">**LegacyFreeBusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a53f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5a53f-106">Attributes and elements</span></span>

<span data-ttu-id="5a53f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a53f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a53f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a53f-108">Attributes</span></span>

<span data-ttu-id="5a53f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a53f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a53f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a53f-110">Child elements</span></span>

<span data-ttu-id="5a53f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a53f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a53f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a53f-112">Parent elements</span></span>

|<span data-ttu-id="5a53f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a53f-113">**Element**</span></span>|<span data-ttu-id="5a53f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a53f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a53f-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5a53f-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5a53f-116">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="5a53f-116">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a53f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a53f-117">Text value</span></span>

<span data-ttu-id="5a53f-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="5a53f-118">A text value is required.</span></span> <span data-ttu-id="5a53f-119">この要素に使用できる値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5a53f-119">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="5a53f-120">空き</span><span class="sxs-lookup"><span data-stu-id="5a53f-120">Free</span></span>
    
- <span data-ttu-id="5a53f-121">仮の予定</span><span class="sxs-lookup"><span data-stu-id="5a53f-121">Tentative</span></span>
    
- <span data-ttu-id="5a53f-122">多忙</span><span class="sxs-lookup"><span data-stu-id="5a53f-122">Busy</span></span>
    
- <span data-ttu-id="5a53f-123">OOF</span><span class="sxs-lookup"><span data-stu-id="5a53f-123">OOF</span></span>
    
- <span data-ttu-id="5a53f-124">NoData</span><span class="sxs-lookup"><span data-stu-id="5a53f-124">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="5a53f-125">注釈</span><span class="sxs-lookup"><span data-stu-id="5a53f-125">Remarks</span></span>

<span data-ttu-id="5a53f-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5a53f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a53f-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5a53f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a53f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a53f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a53f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a53f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="5a53f-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5a53f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a53f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a53f-131">Validation File</span></span>  <br/> |<span data-ttu-id="5a53f-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5a53f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a53f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a53f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a53f-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="5a53f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a53f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a53f-135">See also</span></span>



- [<span data-ttu-id="5a53f-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a53f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

