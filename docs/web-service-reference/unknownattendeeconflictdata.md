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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459869"
---
# <a name="unknownattendeeconflictdata"></a><span data-ttu-id="9c7c1-103">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="9c7c1-103">UnknownAttendeeConflictData</span></span>

<span data-ttu-id="9c7c1-104">**UnknownAttendeeConflictData**要素は、ユーザー、配布リスト、または連絡先ではない、未解決の出席者または出席者を表します。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-104">The **UnknownAttendeeConflictData** element represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span> 
  
[<span data-ttu-id="9c7c1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="9c7c1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="9c7c1-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="9c7c1-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="9c7c1-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="9c7c1-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="9c7c1-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="9c7c1-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="9c7c1-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="9c7c1-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="9c7c1-110">提案</span><span class="sxs-lookup"><span data-stu-id="9c7c1-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="9c7c1-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="9c7c1-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="9c7c1-112">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="9c7c1-112">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md)
  
```xml
<UnknownAttendeeConflictData/>
```

 <span data-ttu-id="9c7c1-113">**UnknownAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="9c7c1-113">**UnknownAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c7c1-114">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9c7c1-114">Attributes and elements</span></span>

<span data-ttu-id="9c7c1-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c7c1-116">属性</span><span class="sxs-lookup"><span data-stu-id="9c7c1-116">Attributes</span></span>

<span data-ttu-id="9c7c1-117">なし。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c7c1-118">子要素</span><span class="sxs-lookup"><span data-stu-id="9c7c1-118">Child elements</span></span>

<span data-ttu-id="9c7c1-119">なし。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c7c1-120">親要素</span><span class="sxs-lookup"><span data-stu-id="9c7c1-120">Parent elements</span></span>

|<span data-ttu-id="9c7c1-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c7c1-121">**Element**</span></span>|<span data-ttu-id="9c7c1-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c7c1-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c7c1-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="9c7c1-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="9c7c1-124">[Getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-124">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="9c7c1-125">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c7c1-126">注釈</span><span class="sxs-lookup"><span data-stu-id="9c7c1-126">Remarks</span></span>

<span data-ttu-id="9c7c1-127">Active Directory ディレクトリサービスオブジェクトに対して解決できない場合、出席者は不明です。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-127">An attendee is unknown if it cannot be resolved against an Active Directory directory service object.</span></span> <span data-ttu-id="9c7c1-128">ユーザー、グループ、または連絡先であると判断できない場合、出席者は未解決になります。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-128">An attendee is unresolved if it cannot be determined to be a user, group, or contact.</span></span> <span data-ttu-id="9c7c1-129">たとえば、メールが有効なパブリックフォルダーである場合、出席者は解決されません。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-129">For example, an attendee will not be resolved if it is a mail-enabled public folder.</span></span>
  
<span data-ttu-id="9c7c1-130">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9c7c1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c7c1-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9c7c1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c7c1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="9c7c1-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c7c1-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c7c1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="9c7c1-134">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9c7c1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="9c7c1-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c7c1-135">Validation File</span></span>  <br/> |<span data-ttu-id="9c7c1-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9c7c1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c7c1-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9c7c1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c7c1-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="9c7c1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c7c1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c7c1-139">See also</span></span>



[<span data-ttu-id="9c7c1-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="9c7c1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="9c7c1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="9c7c1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="9c7c1-142">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="9c7c1-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

