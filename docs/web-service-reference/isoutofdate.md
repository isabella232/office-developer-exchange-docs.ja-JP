---
title: IsOutOfDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOutOfDate
api_type:
- schema
ms.assetid: 2b6005a6-56a9-4848-b998-32908c13e2e2
description: IsOutOfDate 要素は、会議出席依頼、要求、応答、またはキャンセルのどちらが古いかどうかを示します。
ms.openlocfilehash: 0a6b2670cc3eb260002821bab31d652177902de1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832110"
---
# <a name="isoutofdate"></a><span data-ttu-id="0e88f-103">IsOutOfDate</span><span class="sxs-lookup"><span data-stu-id="0e88f-103">IsOutOfDate</span></span>

<span data-ttu-id="0e88f-104">**IsOutOfDate**要素は、会議出席依頼、要求、応答、またはキャンセルのどちらが古いかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-104">The **IsOutOfDate** element indicates whether a meeting message, request, response, or cancellation is out-of-date.</span></span> 
  
```xml
<IsOutOfDate/>
```

 <span data-ttu-id="0e88f-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="0e88f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e88f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0e88f-106">Attributes and elements</span></span>

<span data-ttu-id="0e88f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e88f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e88f-108">Attributes</span></span>

<span data-ttu-id="0e88f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e88f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e88f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e88f-110">Child elements</span></span>

<span data-ttu-id="0e88f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0e88f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e88f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0e88f-112">Parent elements</span></span>

|<span data-ttu-id="0e88f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e88f-113">**Element**</span></span>|<span data-ttu-id="0e88f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e88f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e88f-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0e88f-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0e88f-116">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0e88f-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0e88f-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0e88f-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0e88f-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0e88f-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0e88f-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0e88f-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0e88f-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0e88f-122">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e88f-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0e88f-123">Text value</span></span>

<span data-ttu-id="0e88f-124">**True**の場合、テキスト値は、会議アイテムが古いことを示します。</span><span class="sxs-lookup"><span data-stu-id="0e88f-124">A text value of **true** indicates that the meeting item is out-of-date.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e88f-125">備考</span><span class="sxs-lookup"><span data-stu-id="0e88f-125">Remarks</span></span>

<span data-ttu-id="0e88f-126">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0e88f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e88f-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="0e88f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e88f-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="0e88f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e88f-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e88f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0e88f-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0e88f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e88f-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e88f-131">Validation File</span></span>  <br/> |<span data-ttu-id="0e88f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0e88f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e88f-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0e88f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e88f-134">False</span><span class="sxs-lookup"><span data-stu-id="0e88f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e88f-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e88f-135">See also</span></span>



- [<span data-ttu-id="0e88f-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e88f-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

