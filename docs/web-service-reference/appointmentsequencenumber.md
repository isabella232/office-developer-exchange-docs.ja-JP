---
title: AppointmentSequenceNumber
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentSequenceNumber
api_type:
- schema
ms.assetid: eb4c48bd-f905-48dc-ae16-53a080b9b025
description: AppointmentSequenceNumber 要素は、予定のバージョンのシーケンス番号を指定します。
ms.openlocfilehash: bc186170ccca06669ea7d20cea06c542f9ce274a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759420"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="49a70-103">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="49a70-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="49a70-104">**AppointmentSequenceNumber**要素は、予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="49a70-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="49a70-105">**int**</span><span class="sxs-lookup"><span data-stu-id="49a70-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49a70-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="49a70-106">Attributes and elements</span></span>

<span data-ttu-id="49a70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49a70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49a70-108">属性</span><span class="sxs-lookup"><span data-stu-id="49a70-108">Attributes</span></span>

<span data-ttu-id="49a70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="49a70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49a70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="49a70-110">Child elements</span></span>

<span data-ttu-id="49a70-111">なし。</span><span class="sxs-lookup"><span data-stu-id="49a70-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49a70-112">親要素</span><span class="sxs-lookup"><span data-stu-id="49a70-112">Parent elements</span></span>

|<span data-ttu-id="49a70-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="49a70-113">**Element**</span></span>|<span data-ttu-id="49a70-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="49a70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49a70-115">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="49a70-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="49a70-116">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="49a70-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="49a70-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="49a70-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="49a70-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="49a70-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49a70-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="49a70-119">Text value</span></span>

<span data-ttu-id="49a70-120">テキスト値は、バージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="49a70-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49a70-121">備考</span><span class="sxs-lookup"><span data-stu-id="49a70-121">Remarks</span></span>

<span data-ttu-id="49a70-122">予定が新しい情報で更新されたとき、この値が更新されます。</span><span class="sxs-lookup"><span data-stu-id="49a70-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="49a70-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="49a70-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49a70-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="49a70-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49a70-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="49a70-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49a70-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49a70-126">Schema Name</span></span>  <br/> |<span data-ttu-id="49a70-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="49a70-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="49a70-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49a70-128">Validation File</span></span>  <br/> |<span data-ttu-id="49a70-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49a70-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49a70-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49a70-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="49a70-131">False</span><span class="sxs-lookup"><span data-stu-id="49a70-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49a70-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="49a70-132">See also</span></span>

- [<span data-ttu-id="49a70-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="49a70-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

