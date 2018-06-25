---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: 終了時刻の要素は、時間間隔の終了を表します。
ms.openlocfilehash: 7d3d186618a7bcc05ad82532e13e03d2e67a0e40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760312"
---
# <a name="endtime"></a><span data-ttu-id="d850f-103">EndTime</span><span class="sxs-lookup"><span data-stu-id="d850f-103">EndTime</span></span>

<span data-ttu-id="d850f-104">**終了時刻**の要素は、時間間隔の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="d850f-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="d850f-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d850f-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d850f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d850f-106">Attributes and elements</span></span>

<span data-ttu-id="d850f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d850f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d850f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d850f-108">Attributes</span></span>

<span data-ttu-id="d850f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d850f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d850f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d850f-110">Child elements</span></span>

<span data-ttu-id="d850f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d850f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d850f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d850f-112">Parent elements</span></span>

|<span data-ttu-id="d850f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d850f-113">**Element**</span></span>|<span data-ttu-id="d850f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d850f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d850f-115">時間</span><span class="sxs-lookup"><span data-stu-id="d850f-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="d850f-116">ユーザーの可用性について照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="d850f-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="d850f-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d850f-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="d850f-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="d850f-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="d850f-119">提案された会議の時間についての詳細情報を照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="d850f-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="d850f-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d850f-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="d850f-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="d850f-121"></span></span>  <br/> |
|[<span data-ttu-id="d850f-122">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="d850f-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="d850f-123">Office (OOF) の状態が有効である[OofState](oofstate.md)要素は、 **[スケジュール済]** に設定されている場合、期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="d850f-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="d850f-124">この要素に使用可能な XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="d850f-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="d850f-125">出現</span><span class="sxs-lookup"><span data-stu-id="d850f-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="d850f-126">定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d850f-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d850f-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="d850f-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="d850f-128">独自の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="d850f-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="d850f-129">可用性の照会のために使用します。</span><span class="sxs-lookup"><span data-stu-id="d850f-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="d850f-130">**CalendarEvent**要素では、**終了時刻**の要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="d850f-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="d850f-131">**CalendarEvent**要素の**終了時刻**の要素は、 **CalendarEvent**の種類に固有です。</span><span class="sxs-lookup"><span data-stu-id="d850f-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="d850f-132">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="d850f-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d850f-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d850f-133">Text value</span></span>

<span data-ttu-id="d850f-134">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="d850f-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d850f-135">備考</span><span class="sxs-lookup"><span data-stu-id="d850f-135">Remarks</span></span>

<span data-ttu-id="d850f-136">[StartTime](starttime.md)要素は、時間間隔の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="d850f-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="d850f-137">終了時刻は、クライアントの時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="d850f-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="d850f-138">スキーマには、[終了時刻](endtime.md)の多くの要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d850f-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d850f-139">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d850f-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d850f-140">要素情報</span><span class="sxs-lookup"><span data-stu-id="d850f-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d850f-141">名前空間</span><span class="sxs-lookup"><span data-stu-id="d850f-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d850f-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d850f-142">Schema Name</span></span>  <br/> |<span data-ttu-id="d850f-143">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d850f-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="d850f-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d850f-144">Validation File</span></span>  <br/> |<span data-ttu-id="d850f-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d850f-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d850f-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d850f-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="d850f-147">False</span><span class="sxs-lookup"><span data-stu-id="d850f-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d850f-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="d850f-148">See also</span></span>

- [<span data-ttu-id="d850f-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="d850f-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d850f-150">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="d850f-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

