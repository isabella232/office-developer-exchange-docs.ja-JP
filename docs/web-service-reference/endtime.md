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
description: EndTime 要素は、期間の最後の部分を表します。
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462993"
---
# <a name="endtime"></a><span data-ttu-id="691f1-103">EndTime</span><span class="sxs-lookup"><span data-stu-id="691f1-103">EndTime</span></span>

<span data-ttu-id="691f1-104">**EndTime**要素は、期間の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="691f1-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="691f1-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="691f1-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="691f1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="691f1-106">Attributes and elements</span></span>

<span data-ttu-id="691f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="691f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="691f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="691f1-108">Attributes</span></span>

<span data-ttu-id="691f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="691f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="691f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="691f1-110">Child elements</span></span>

<span data-ttu-id="691f1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="691f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="691f1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="691f1-112">Parent elements</span></span>

|<span data-ttu-id="691f1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="691f1-113">**Element**</span></span>|<span data-ttu-id="691f1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="691f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="691f1-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="691f1-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="691f1-116">ユーザーの空き時間情報を照会した期間を識別します。</span><span class="sxs-lookup"><span data-stu-id="691f1-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="691f1-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="691f1-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="691f1-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="691f1-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="691f1-119">提案された会議時間に関する詳細情報について、クエリされる期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="691f1-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="691f1-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="691f1-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="691f1-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="691f1-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span></span>  <br/> |
|[<span data-ttu-id="691f1-122">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="691f1-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="691f1-123">[Oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、不在時 (OOF) の状態が有効になる期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="691f1-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="691f1-124">この要素に使用できる XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="691f1-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="691f1-125">発生</span><span class="sxs-lookup"><span data-stu-id="691f1-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="691f1-126">定期的な予定表アイテムの1つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="691f1-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="691f1-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="691f1-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="691f1-128">一意の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="691f1-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="691f1-129">これは、可用性の照会に使用されます。</span><span class="sxs-lookup"><span data-stu-id="691f1-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="691f1-130">**CalendarEvent**要素では、 **EndTime**要素を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="691f1-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="691f1-131">**CalendarEvent**要素の**EndTime**要素は、 **CalendarEvent**型に対して一意です。</span><span class="sxs-lookup"><span data-stu-id="691f1-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="691f1-132">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="691f1-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="691f1-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="691f1-133">Text value</span></span>

<span data-ttu-id="691f1-134">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="691f1-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="691f1-135">注釈</span><span class="sxs-lookup"><span data-stu-id="691f1-135">Remarks</span></span>

<span data-ttu-id="691f1-136">[StartTime](starttime.md)要素は、時間間隔の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="691f1-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="691f1-137">終了時刻はクライアントの時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="691f1-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="691f1-138">スキーマには、多くの[EndTime](endtime.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="691f1-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="691f1-139">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="691f1-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="691f1-140">要素の情報</span><span class="sxs-lookup"><span data-stu-id="691f1-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="691f1-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="691f1-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="691f1-142">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="691f1-142">Schema Name</span></span>  <br/> |<span data-ttu-id="691f1-143">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="691f1-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="691f1-144">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="691f1-144">Validation File</span></span>  <br/> |<span data-ttu-id="691f1-145">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="691f1-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="691f1-146">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="691f1-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="691f1-147">正しくない</span><span class="sxs-lookup"><span data-stu-id="691f1-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="691f1-148">関連項目</span><span class="sxs-lookup"><span data-stu-id="691f1-148">See also</span></span>

- [<span data-ttu-id="691f1-149">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="691f1-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="691f1-150">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="691f1-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

