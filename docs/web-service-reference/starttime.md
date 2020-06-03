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
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458566"
---
# <a name="starttime"></a><span data-ttu-id="ce4b2-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="ce4b2-103">StartTime</span></span>

<span data-ttu-id="ce4b2-104">**StartTime**要素は、時間間隔の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="ce4b2-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="ce4b2-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ce4b2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ce4b2-106">Attributes and elements</span></span>

<span data-ttu-id="ce4b2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce4b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce4b2-108">Attributes</span></span>

<span data-ttu-id="ce4b2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce4b2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ce4b2-110">Child elements</span></span>

<span data-ttu-id="ce4b2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce4b2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ce4b2-112">Parent elements</span></span>

|<span data-ttu-id="ce4b2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ce4b2-113">**Element**</span></span>|<span data-ttu-id="ce4b2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce4b2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce4b2-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="ce4b2-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="ce4b2-116">ユーザーの空き時間情報を照会した期間を識別します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="ce4b2-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="ce4b2-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="ce4b2-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="ce4b2-119">提案された会議時間に関する詳細情報について、クエリされる期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="ce4b2-120">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="ce4b2-121">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="ce4b2-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="ce4b2-122">[Oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、不在時 (OOF) の状態が有効になる期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="ce4b2-123">この要素に使用できる XPath 式は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="ce4b2-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="ce4b2-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="ce4b2-125">一意の予定表アイテムの出現を表します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="ce4b2-126">これは、可用性の照会に使用されます。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="ce4b2-127">**CalendarEvent**要素では、 **StartTime**要素を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="ce4b2-128">**CalendarEvent**要素の**starttime**要素は、 **CalendarEvent**型に対して一意ですが、 **Duration**型の**starttime**要素に含まれているのと同じファセット値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="ce4b2-129">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce4b2-130">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ce4b2-130">Text value</span></span>

<span data-ttu-id="ce4b2-131">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce4b2-132">注釈</span><span class="sxs-lookup"><span data-stu-id="ce4b2-132">Remarks</span></span>

<span data-ttu-id="ce4b2-133">[EndTime](endtime.md)要素は、期間の最後の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="ce4b2-134">スキーマには、いくつかの[StartTime](starttime.md)要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ce4b2-135">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ce4b2-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ce4b2-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ce4b2-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce4b2-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce4b2-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce4b2-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce4b2-138">Schema Name</span></span>  <br/> |<span data-ttu-id="ce4b2-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ce4b2-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce4b2-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce4b2-140">Validation File</span></span>  <br/> |<span data-ttu-id="ce4b2-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ce4b2-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce4b2-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ce4b2-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce4b2-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="ce4b2-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce4b2-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce4b2-144">See also</span></span>

- [<span data-ttu-id="ce4b2-145">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="ce4b2-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="ce4b2-146">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="ce4b2-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

