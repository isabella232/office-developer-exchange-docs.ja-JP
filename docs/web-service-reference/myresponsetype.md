---
title: MyResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MyResponseType
api_type:
- schema
ms.assetid: 9741b71d-a310-4520-81d5-3787a1ee630f
description: MyResponseType 要素には、または予定表アイテムへの応答の状態が含まれています。
ms.openlocfilehash: 3be900ed6d2932699e3e83a0bca2918c016eb689
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832497"
---
# <a name="myresponsetype"></a><span data-ttu-id="576f4-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="576f4-103">MyResponseType</span></span>

<span data-ttu-id="576f4-104">**MyResponseType**要素には、または予定表アイテムへの応答の状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="576f4-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="576f4-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="576f4-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="576f4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="576f4-106">Attributes and elements</span></span>

<span data-ttu-id="576f4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="576f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="576f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="576f4-108">Attributes</span></span>

<span data-ttu-id="576f4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="576f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="576f4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="576f4-110">Child elements</span></span>

<span data-ttu-id="576f4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="576f4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="576f4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="576f4-112">Parent elements</span></span>

|<span data-ttu-id="576f4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="576f4-113">**Element**</span></span>|<span data-ttu-id="576f4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="576f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="576f4-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="576f4-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="576f4-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="576f4-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="576f4-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="576f4-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="576f4-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="576f4-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="576f4-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="576f4-119">Text value</span></span>

<span data-ttu-id="576f4-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="576f4-120">A text value is required.</span></span> <span data-ttu-id="576f4-121">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="576f4-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="576f4-122">Unknown</span><span class="sxs-lookup"><span data-stu-id="576f4-122">Unknown</span></span>
    
- <span data-ttu-id="576f4-123">Organizer</span><span class="sxs-lookup"><span data-stu-id="576f4-123">Organizer</span></span>
    
- <span data-ttu-id="576f4-124">Tentative</span><span class="sxs-lookup"><span data-stu-id="576f4-124">Tentative</span></span>
    
- <span data-ttu-id="576f4-125">承諾</span><span class="sxs-lookup"><span data-stu-id="576f4-125">Accept</span></span>
    
- <span data-ttu-id="576f4-126">辞退</span><span class="sxs-lookup"><span data-stu-id="576f4-126">Decline</span></span>
    
- <span data-ttu-id="576f4-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="576f4-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="576f4-128">備考</span><span class="sxs-lookup"><span data-stu-id="576f4-128">Remarks</span></span>

<span data-ttu-id="576f4-129">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="576f4-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="576f4-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="576f4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="576f4-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="576f4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="576f4-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="576f4-132">Schema name</span></span>  <br/> |<span data-ttu-id="576f4-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="576f4-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="576f4-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="576f4-134">Validation file</span></span>  <br/> |<span data-ttu-id="576f4-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="576f4-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="576f4-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="576f4-136">Can be empty</span></span>  <br/> |<span data-ttu-id="576f4-137">False</span><span class="sxs-lookup"><span data-stu-id="576f4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="576f4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="576f4-138">See also</span></span>



- [<span data-ttu-id="576f4-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="576f4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

