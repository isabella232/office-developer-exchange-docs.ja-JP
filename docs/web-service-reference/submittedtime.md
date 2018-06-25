---
title: SubmittedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmittedTime
api_type:
- schema
ms.assetid: 45c8fa36-c539-42ca-99dc-1ac33cc54afc
description: SubmittedTime 要素は、メッセージがサーバーを入力する時間を表します。
ms.openlocfilehash: 89fc6400914495b8f1bd3994f17421d0ab079460
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833613"
---
# <a name="submittedtime"></a><span data-ttu-id="e16b3-103">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="e16b3-103">SubmittedTime</span></span>

<span data-ttu-id="e16b3-104">**SubmittedTime**要素は、メッセージがサーバーを入力する時間を表します。</span><span class="sxs-lookup"><span data-stu-id="e16b3-104">The **SubmittedTime** element represents the time that the message entered the server.</span></span> 
  
```XML
<SubmittedTime/>
```

 <span data-ttu-id="e16b3-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="e16b3-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e16b3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e16b3-106">Attributes and elements</span></span>

<span data-ttu-id="e16b3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e16b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e16b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="e16b3-108">Attributes</span></span>

<span data-ttu-id="e16b3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e16b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e16b3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e16b3-110">Child elements</span></span>

<span data-ttu-id="e16b3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e16b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e16b3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e16b3-112">Parent elements</span></span>

|<span data-ttu-id="e16b3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e16b3-113">**Element**</span></span>|<span data-ttu-id="e16b3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e16b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e16b3-115">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="e16b3-115">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="e16b3-116">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e16b3-116">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e16b3-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e16b3-117">Text value</span></span>

 <span data-ttu-id="e16b3-118">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="e16b3-118">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e16b3-119">備考</span><span class="sxs-lookup"><span data-stu-id="e16b3-119">Remarks</span></span>

<span data-ttu-id="e16b3-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e16b3-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e16b3-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="e16b3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e16b3-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="e16b3-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e16b3-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e16b3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="e16b3-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e16b3-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="e16b3-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e16b3-125">Validation File</span></span>  <br/> |<span data-ttu-id="e16b3-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e16b3-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e16b3-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e16b3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="e16b3-128">False</span><span class="sxs-lookup"><span data-stu-id="e16b3-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e16b3-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="e16b3-129">See also</span></span>



- [<span data-ttu-id="e16b3-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e16b3-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

