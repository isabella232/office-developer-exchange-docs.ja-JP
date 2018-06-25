---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: DetailedSuggestionsWindow 要素は、提案された会議の時間についての詳細情報を照会する期間を指定します。
ms.openlocfilehash: 8a3af0178d0c96b50f4dd641716a9f7a7be8f7a2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760024"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="db38c-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="db38c-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="db38c-104">**DetailedSuggestionsWindow**要素は、提案された会議の時間についての詳細情報を照会する期間を指定します。</span><span class="sxs-lookup"><span data-stu-id="db38c-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="db38c-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="db38c-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="db38c-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="db38c-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="db38c-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="db38c-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="db38c-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="db38c-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db38c-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="db38c-109">Attributes and elements</span></span>

<span data-ttu-id="db38c-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db38c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db38c-111">属性</span><span class="sxs-lookup"><span data-stu-id="db38c-111">Attributes</span></span>

<span data-ttu-id="db38c-112">なし。</span><span class="sxs-lookup"><span data-stu-id="db38c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db38c-113">子要素</span><span class="sxs-lookup"><span data-stu-id="db38c-113">Child elements</span></span>

|<span data-ttu-id="db38c-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="db38c-114">**Element**</span></span>|<span data-ttu-id="db38c-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="db38c-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db38c-116">開始時刻</span><span class="sxs-lookup"><span data-stu-id="db38c-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="db38c-117">提案された会議の時間についての詳細なクエリを実行する期間の開始を表します。</span><span class="sxs-lookup"><span data-stu-id="db38c-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="db38c-118">終了時刻</span><span class="sxs-lookup"><span data-stu-id="db38c-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="db38c-119">提案された会議の時間についての詳細なクエリを実行する、時間の終了を表します。</span><span class="sxs-lookup"><span data-stu-id="db38c-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db38c-120">親要素</span><span class="sxs-lookup"><span data-stu-id="db38c-120">Parent elements</span></span>

|<span data-ttu-id="db38c-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="db38c-121">**Element**</span></span>|<span data-ttu-id="db38c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="db38c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db38c-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="db38c-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="db38c-124">取得するためのオプションが含まれています会議の情報を提案します。</span><span class="sxs-lookup"><span data-stu-id="db38c-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="db38c-125">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="db38c-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="db38c-126">備考</span><span class="sxs-lookup"><span data-stu-id="db38c-126">Remarks</span></span>

<span data-ttu-id="db38c-127">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="db38c-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="db38c-128">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ MicrosoftExchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="db38c-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="db38c-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="db38c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db38c-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="db38c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db38c-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db38c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="db38c-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="db38c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="db38c-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db38c-133">Validation File</span></span>  <br/> |<span data-ttu-id="db38c-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db38c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db38c-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db38c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="db38c-136">False</span><span class="sxs-lookup"><span data-stu-id="db38c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db38c-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="db38c-137">See also</span></span>

- [<span data-ttu-id="db38c-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="db38c-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="db38c-139">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="db38c-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

