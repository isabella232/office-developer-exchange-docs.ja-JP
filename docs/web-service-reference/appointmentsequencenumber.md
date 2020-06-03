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
ms.openlocfilehash: daeea7a656c59923bcb6f2850539c7869d6eb181
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461661"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="57793-103">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="57793-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="57793-104">**AppointmentSequenceNumber**要素は、予定のバージョンのシーケンス番号を指定します。</span><span class="sxs-lookup"><span data-stu-id="57793-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="57793-105">**int**</span><span class="sxs-lookup"><span data-stu-id="57793-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57793-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="57793-106">Attributes and elements</span></span>

<span data-ttu-id="57793-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57793-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57793-108">属性</span><span class="sxs-lookup"><span data-stu-id="57793-108">Attributes</span></span>

<span data-ttu-id="57793-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57793-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57793-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57793-110">Child elements</span></span>

<span data-ttu-id="57793-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57793-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57793-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57793-112">Parent elements</span></span>

|<span data-ttu-id="57793-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="57793-113">**Element**</span></span>|<span data-ttu-id="57793-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="57793-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57793-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="57793-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="57793-116">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="57793-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="57793-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="57793-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="57793-118">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="57793-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57793-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57793-119">Text value</span></span>

<span data-ttu-id="57793-120">テキスト値は、バージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="57793-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57793-121">注釈</span><span class="sxs-lookup"><span data-stu-id="57793-121">Remarks</span></span>

<span data-ttu-id="57793-122">この値は、予定が新しい情報で更新されたときに更新されます。</span><span class="sxs-lookup"><span data-stu-id="57793-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="57793-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="57793-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57793-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="57793-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57793-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="57793-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57793-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57793-126">Schema Name</span></span>  <br/> |<span data-ttu-id="57793-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="57793-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="57793-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57793-128">Validation File</span></span>  <br/> |<span data-ttu-id="57793-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="57793-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57793-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57793-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="57793-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="57793-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57793-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="57793-132">See also</span></span>

- [<span data-ttu-id="57793-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="57793-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

