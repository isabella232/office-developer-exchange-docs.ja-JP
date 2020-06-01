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
description: DetailedSuggestionsWindow 要素は、提案された会議の時間に関する詳細情報に対してクエリを実行する時間間隔を指定します。
ms.openlocfilehash: 45d582f2642c0e3d8f6330b09946230c8842618d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467845"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="5c416-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="5c416-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="5c416-104">**DetailedSuggestionsWindow**要素は、提案された会議の時間に関する詳細情報に対してクエリを実行する時間間隔を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c416-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="5c416-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="5c416-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="5c416-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="5c416-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="5c416-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="5c416-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="5c416-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="5c416-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c416-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5c416-109">Attributes and elements</span></span>

<span data-ttu-id="5c416-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c416-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c416-111">属性</span><span class="sxs-lookup"><span data-stu-id="5c416-111">Attributes</span></span>

<span data-ttu-id="5c416-112">なし。</span><span class="sxs-lookup"><span data-stu-id="5c416-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c416-113">子要素</span><span class="sxs-lookup"><span data-stu-id="5c416-113">Child elements</span></span>

|<span data-ttu-id="5c416-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="5c416-114">**Element**</span></span>|<span data-ttu-id="5c416-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c416-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c416-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="5c416-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="5c416-117">提案された会議時間に関する詳細情報を照会した期間の開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="5c416-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="5c416-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="5c416-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="5c416-119">提案された会議時間に関する詳細情報を照会した期間の終わりを表します。</span><span class="sxs-lookup"><span data-stu-id="5c416-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c416-120">親要素</span><span class="sxs-lookup"><span data-stu-id="5c416-120">Parent elements</span></span>

|<span data-ttu-id="5c416-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c416-121">**Element**</span></span>|<span data-ttu-id="5c416-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c416-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c416-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="5c416-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="5c416-124">会議提案情報を取得するためのオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c416-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="5c416-125">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c416-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c416-126">注釈</span><span class="sxs-lookup"><span data-stu-id="5c416-126">Remarks</span></span>

<span data-ttu-id="5c416-127">この要素は必須ではありません。</span><span class="sxs-lookup"><span data-stu-id="5c416-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5c416-128">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの/EWS/ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5c416-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5c416-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5c416-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c416-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c416-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c416-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c416-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5c416-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5c416-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c416-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c416-133">Validation File</span></span>  <br/> |<span data-ttu-id="5c416-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5c416-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c416-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c416-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c416-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="5c416-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c416-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c416-137">See also</span></span>

- [<span data-ttu-id="5c416-138">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="5c416-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="5c416-139">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="5c416-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

