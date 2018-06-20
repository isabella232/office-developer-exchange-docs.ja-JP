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
description: UnknownAttendeeConflictData 要素は、解決できない出席者または出席者は、ユーザー、配布リスト、または取引先担当者を表します。
ms.openlocfilehash: 2363e243a833f580b4b5701b7d39d9ba9420f35a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839800"
---
# <a name="unknownattendeeconflictdata"></a><span data-ttu-id="1ad3c-103">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="1ad3c-103">UnknownAttendeeConflictData</span></span>

<span data-ttu-id="1ad3c-104">**UnknownAttendeeConflictData**要素は、解決できない出席者または出席者は、ユーザー、配布リスト、または取引先担当者を表します。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-104">The **UnknownAttendeeConflictData** element represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span> 
  
[<span data-ttu-id="1ad3c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ad3c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1ad3c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="1ad3c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="1ad3c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="1ad3c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="1ad3c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="1ad3c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="1ad3c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="1ad3c-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="1ad3c-110">提案</span><span class="sxs-lookup"><span data-stu-id="1ad3c-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="1ad3c-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="1ad3c-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="1ad3c-112">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="1ad3c-112">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md)
  
```xml
<UnknownAttendeeConflictData/>
```

 <span data-ttu-id="1ad3c-113">**UnknownAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="1ad3c-113">**UnknownAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ad3c-114">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1ad3c-114">Attributes and elements</span></span>

<span data-ttu-id="1ad3c-115">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ad3c-116">属性</span><span class="sxs-lookup"><span data-stu-id="1ad3c-116">Attributes</span></span>

<span data-ttu-id="1ad3c-117">なし。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ad3c-118">子要素</span><span class="sxs-lookup"><span data-stu-id="1ad3c-118">Child elements</span></span>

<span data-ttu-id="1ad3c-119">なし。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ad3c-120">親要素</span><span class="sxs-lookup"><span data-stu-id="1ad3c-120">Parent elements</span></span>

|<span data-ttu-id="1ad3c-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ad3c-121">**Element**</span></span>|<span data-ttu-id="1ad3c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ad3c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ad3c-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="1ad3c-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="1ad3c-124">[GetUserAvailability 操作](getuseravailability-operation.md)で指定されたクエリを実行した出席者のために競合データの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-124">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="1ad3c-125">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ad3c-126">備考</span><span class="sxs-lookup"><span data-stu-id="1ad3c-126">Remarks</span></span>

<span data-ttu-id="1ad3c-127">Active Directory ディレクトリ サービス オブジェクトに対する、解決できない場合、出席者は不明です。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-127">An attendee is unknown if it cannot be resolved against an Active Directory directory service object.</span></span> <span data-ttu-id="1ad3c-128">ユーザー、グループ、または連絡先を指定できない場合、出席者は解決ではありません。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-128">An attendee is unresolved if it cannot be determined to be a user, group, or contact.</span></span> <span data-ttu-id="1ad3c-129">たとえば、出席者は解決できませんがメールが有効なパブリック フォルダーにある場合。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-129">For example, an attendee will not be resolved if it is a mail-enabled public folder.</span></span>
  
<span data-ttu-id="1ad3c-130">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ad3c-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="1ad3c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ad3c-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="1ad3c-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ad3c-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ad3c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1ad3c-134">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1ad3c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ad3c-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ad3c-135">Validation File</span></span>  <br/> |<span data-ttu-id="1ad3c-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1ad3c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ad3c-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ad3c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ad3c-138">False</span><span class="sxs-lookup"><span data-stu-id="1ad3c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ad3c-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ad3c-139">See also</span></span>



[<span data-ttu-id="1ad3c-140">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="1ad3c-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1ad3c-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1ad3c-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1ad3c-142">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="1ad3c-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

