---
title: UnknownAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownAttendeeConflictData
api_type:
- schema
ms.assetid: 70e41268-c231-4587-9d23-e46927fe5272
description: UnknownAttendeeConflictData 要素は、ユーザー、配布リスト、または連絡先ではない、未解決の出席者または出席者を表します。
ms.openlocfilehash: b4362e0117e3939c21342a1ab8079d95512aec79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459869"
---
# <a name="unknownattendeeconflictdata"></a><span data-ttu-id="4ef16-103">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="4ef16-103">UnknownAttendeeConflictData</span></span>

<span data-ttu-id="4ef16-104">**UnknownAttendeeConflictData**要素は、ユーザー、配布リスト、または連絡先ではない、未解決の出席者または出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="4ef16-104">The **UnknownAttendeeConflictData** element represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span> 
  
[<span data-ttu-id="4ef16-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4ef16-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4ef16-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4ef16-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="4ef16-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4ef16-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="4ef16-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="4ef16-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="4ef16-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="4ef16-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="4ef16-110">提案</span><span class="sxs-lookup"><span data-stu-id="4ef16-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="4ef16-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="4ef16-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="4ef16-112">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="4ef16-112">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md)
  
```xml
<UnknownAttendeeConflictData/>
```

 <span data-ttu-id="4ef16-113">**UnknownAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="4ef16-113">**UnknownAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ef16-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4ef16-114">Attributes and elements</span></span>

<span data-ttu-id="4ef16-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ef16-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ef16-116">属性</span><span class="sxs-lookup"><span data-stu-id="4ef16-116">Attributes</span></span>

<span data-ttu-id="4ef16-117">なし。</span><span class="sxs-lookup"><span data-stu-id="4ef16-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ef16-118">子要素</span><span class="sxs-lookup"><span data-stu-id="4ef16-118">Child elements</span></span>

<span data-ttu-id="4ef16-119">なし。</span><span class="sxs-lookup"><span data-stu-id="4ef16-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ef16-120">親要素</span><span class="sxs-lookup"><span data-stu-id="4ef16-120">Parent elements</span></span>

|<span data-ttu-id="4ef16-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ef16-121">**Element**</span></span>|<span data-ttu-id="4ef16-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ef16-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ef16-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="4ef16-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="4ef16-124">[Getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="4ef16-124">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="4ef16-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4ef16-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ef16-126">注釈</span><span class="sxs-lookup"><span data-stu-id="4ef16-126">Remarks</span></span>

<span data-ttu-id="4ef16-127">Active Directory ディレクトリサービスオブジェクトに対して解決できない場合、出席者は不明です。</span><span class="sxs-lookup"><span data-stu-id="4ef16-127">An attendee is unknown if it cannot be resolved against an Active Directory directory service object.</span></span> <span data-ttu-id="4ef16-128">ユーザー、グループ、または連絡先であると判断できない場合、出席者は未解決になります。</span><span class="sxs-lookup"><span data-stu-id="4ef16-128">An attendee is unresolved if it cannot be determined to be a user, group, or contact.</span></span> <span data-ttu-id="4ef16-129">たとえば、メールが有効なパブリックフォルダーである場合、出席者は解決されません。</span><span class="sxs-lookup"><span data-stu-id="4ef16-129">For example, an attendee will not be resolved if it is a mail-enabled public folder.</span></span>
  
<span data-ttu-id="4ef16-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4ef16-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ef16-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4ef16-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ef16-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ef16-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ef16-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ef16-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4ef16-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="4ef16-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ef16-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ef16-135">Validation File</span></span>  <br/> |<span data-ttu-id="4ef16-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="4ef16-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ef16-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4ef16-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="4ef16-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="4ef16-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ef16-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ef16-139">See also</span></span>



[<span data-ttu-id="4ef16-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="4ef16-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4ef16-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4ef16-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4ef16-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="4ef16-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

