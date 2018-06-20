---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: StartTime 要素は、時間間隔の開始を表します。
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833560"
---
# <a name="starttime"></a><span data-ttu-id="4e400-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="4e400-103">StartTime</span></span>

<span data-ttu-id="4e400-104">**StartTime**要素は、時間間隔の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="4e400-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="4e400-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="4e400-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4e400-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e400-106">Attributes and elements</span></span>

<span data-ttu-id="4e400-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e400-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e400-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e400-108">Attributes</span></span>

<span data-ttu-id="4e400-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4e400-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e400-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4e400-110">Child elements</span></span>

<span data-ttu-id="4e400-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4e400-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e400-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4e400-112">Parent elements</span></span>

|<span data-ttu-id="4e400-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e400-113">**Element**</span></span>|<span data-ttu-id="4e400-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e400-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e400-115">時間</span><span class="sxs-lookup"><span data-stu-id="4e400-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="4e400-116">ユーザーの可用性について照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e400-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="4e400-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e400-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="4e400-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="4e400-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="4e400-119">提案された会議の時間についての詳細情報を照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e400-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="4e400-120">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e400-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="4e400-121">期間 (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="4e400-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="4e400-122">Office (OOF) の状態が有効である[OofState](oofstate.md)要素は、 **[スケジュール済]** に設定されている場合、期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e400-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="4e400-123">この要素に使用可能な XPath 式は、次のように。</span><span class="sxs-lookup"><span data-stu-id="4e400-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="4e400-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="4e400-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="4e400-125">独自の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="4e400-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="4e400-126">可用性の照会のために使用します。</span><span class="sxs-lookup"><span data-stu-id="4e400-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="4e400-127">**CalendarEvent**要素の**開始**要素が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e400-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="4e400-128">**CalendarEvent**要素の**開始時刻**の要素は、**期間**の種類の**開始時刻**の要素が含まれているのと同じファセット値が含まれていますが**CalendarEvent**の種類に固有です。</span><span class="sxs-lookup"><span data-stu-id="4e400-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="4e400-129">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4e400-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e400-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4e400-130">Text value</span></span>

<span data-ttu-id="4e400-131">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="4e400-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e400-132">備考</span><span class="sxs-lookup"><span data-stu-id="4e400-132">Remarks</span></span>

<span data-ttu-id="4e400-133">[終了時刻](endtime.md)の要素では、期間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="4e400-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="4e400-134">スキーマには、[開始時刻](starttime.md)の多くの要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e400-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4e400-135">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4e400-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4e400-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="4e400-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e400-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="4e400-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e400-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e400-138">Schema Name</span></span>  <br/> |<span data-ttu-id="4e400-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4e400-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="4e400-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e400-140">Validation File</span></span>  <br/> |<span data-ttu-id="4e400-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4e400-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e400-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4e400-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e400-143">False</span><span class="sxs-lookup"><span data-stu-id="4e400-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e400-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e400-144">See also</span></span>

- [<span data-ttu-id="4e400-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="4e400-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="4e400-146">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="4e400-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

