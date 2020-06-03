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
description: MyResponseType 要素には、予定表アイテムの状態または応答が含まれます。
ms.openlocfilehash: 640b0595ac039cc3c119aa52aa6e791e5b695e87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466627"
---
# <a name="myresponsetype"></a><span data-ttu-id="afd5d-103">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="afd5d-103">MyResponseType</span></span>

<span data-ttu-id="afd5d-104">**Myresponsetype**要素には、予定表アイテムの状態または応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="afd5d-104">The **MyResponseType** element contains the status of or response to a calendar item.</span></span> 
  
```xml
<MyResponseType/>
```

 <span data-ttu-id="afd5d-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="afd5d-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afd5d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="afd5d-106">Attributes and elements</span></span>

<span data-ttu-id="afd5d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="afd5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afd5d-108">属性</span><span class="sxs-lookup"><span data-stu-id="afd5d-108">Attributes</span></span>

<span data-ttu-id="afd5d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="afd5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afd5d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="afd5d-110">Child elements</span></span>

<span data-ttu-id="afd5d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="afd5d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afd5d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="afd5d-112">Parent elements</span></span>

|<span data-ttu-id="afd5d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="afd5d-113">**Element**</span></span>|<span data-ttu-id="afd5d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="afd5d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afd5d-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="afd5d-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="afd5d-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="afd5d-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="afd5d-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="afd5d-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="afd5d-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="afd5d-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afd5d-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="afd5d-119">Text value</span></span>

<span data-ttu-id="afd5d-120">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="afd5d-120">A text value is required.</span></span> <span data-ttu-id="afd5d-121">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="afd5d-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="afd5d-122">不明</span><span class="sxs-lookup"><span data-stu-id="afd5d-122">Unknown</span></span>
    
- <span data-ttu-id="afd5d-123">開催者</span><span class="sxs-lookup"><span data-stu-id="afd5d-123">Organizer</span></span>
    
- <span data-ttu-id="afd5d-124">仮の予定</span><span class="sxs-lookup"><span data-stu-id="afd5d-124">Tentative</span></span>
    
- <span data-ttu-id="afd5d-125">承諾</span><span class="sxs-lookup"><span data-stu-id="afd5d-125">Accept</span></span>
    
- <span data-ttu-id="afd5d-126">同意</span><span class="sxs-lookup"><span data-stu-id="afd5d-126">Decline</span></span>
    
- <span data-ttu-id="afd5d-127">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="afd5d-127">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="afd5d-128">注釈</span><span class="sxs-lookup"><span data-stu-id="afd5d-128">Remarks</span></span>

<span data-ttu-id="afd5d-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="afd5d-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afd5d-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="afd5d-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afd5d-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="afd5d-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afd5d-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="afd5d-132">Schema name</span></span>  <br/> |<span data-ttu-id="afd5d-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="afd5d-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="afd5d-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="afd5d-134">Validation file</span></span>  <br/> |<span data-ttu-id="afd5d-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="afd5d-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afd5d-136">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="afd5d-136">Can be empty</span></span>  <br/> |<span data-ttu-id="afd5d-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="afd5d-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afd5d-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="afd5d-138">See also</span></span>



- [<span data-ttu-id="afd5d-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="afd5d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

