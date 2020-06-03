---
title: IsCancelled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsCancelled
api_type:
- schema
ms.assetid: 50c1e97f-2913-47a1-8457-60428a3c5b92
description: IsCancelled 要素は、予定または会議がキャンセルされたかどうかを示します。
ms.openlocfilehash: 946c9d956da9cf31e9fa08d4ab6f4950b11214b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455570"
---
# <a name="iscancelled"></a><span data-ttu-id="a5e28-103">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="a5e28-103">IsCancelled</span></span>

<span data-ttu-id="a5e28-104">**Iscancelled**要素は、予定または会議がキャンセルされたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-104">The **IsCancelled** element indicates whether an appointment or meeting has been canceled.</span></span> 
  
```xml
<IsCancelled/>
```

 <span data-ttu-id="a5e28-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a5e28-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5e28-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a5e28-106">Attributes and elements</span></span>

<span data-ttu-id="a5e28-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5e28-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5e28-108">Attributes</span></span>

<span data-ttu-id="a5e28-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a5e28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5e28-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a5e28-110">Child elements</span></span>

<span data-ttu-id="a5e28-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a5e28-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5e28-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a5e28-112">Parent elements</span></span>

|<span data-ttu-id="a5e28-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a5e28-113">**Element**</span></span>|<span data-ttu-id="a5e28-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a5e28-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5e28-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a5e28-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a5e28-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a5e28-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a5e28-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a5e28-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5e28-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a5e28-119">Text value</span></span>

<span data-ttu-id="a5e28-120">この要素が含まれている場合は、ブール値を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5e28-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="a5e28-121">**True**の値は、予定表アイテムが取り消されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-121">A value of **true** indicates that the calendar item has been canceled.</span></span> <span data-ttu-id="a5e28-122">値が**false**の場合、予定表アイテムが取り消されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a5e28-122">A value of **false** indicates that a calendar item has not been canceled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a5e28-123">注釈</span><span class="sxs-lookup"><span data-stu-id="a5e28-123">Remarks</span></span>

<span data-ttu-id="a5e28-124">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a5e28-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5e28-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a5e28-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5e28-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5e28-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5e28-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a5e28-127">Schema name</span></span>  <br/> |<span data-ttu-id="a5e28-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a5e28-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5e28-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a5e28-129">Validation file</span></span>  <br/> |<span data-ttu-id="a5e28-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a5e28-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5e28-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a5e28-131">Can be empty</span></span>  <br/> |<span data-ttu-id="a5e28-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="a5e28-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5e28-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="a5e28-133">See also</span></span>



- [<span data-ttu-id="a5e28-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a5e28-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

