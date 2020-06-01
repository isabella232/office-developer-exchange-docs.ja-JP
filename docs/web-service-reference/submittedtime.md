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
description: SubmittedTime 要素は、メッセージがサーバーに入力した時刻を表します。
ms.openlocfilehash: bf9495aa700d2887d199eccb38289e0ebd2e8636
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465409"
---
# <a name="submittedtime"></a><span data-ttu-id="df60a-103">SubmittedTime</span><span class="sxs-lookup"><span data-stu-id="df60a-103">SubmittedTime</span></span>

<span data-ttu-id="df60a-104">**Submittedtime**要素は、メッセージがサーバーに入力した時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="df60a-104">The **SubmittedTime** element represents the time that the message entered the server.</span></span> 
  
```XML
<SubmittedTime/>
```

 <span data-ttu-id="df60a-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="df60a-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df60a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="df60a-106">Attributes and elements</span></span>

<span data-ttu-id="df60a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df60a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df60a-108">属性</span><span class="sxs-lookup"><span data-stu-id="df60a-108">Attributes</span></span>

<span data-ttu-id="df60a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="df60a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df60a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="df60a-110">Child elements</span></span>

<span data-ttu-id="df60a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="df60a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df60a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="df60a-112">Parent elements</span></span>

|<span data-ttu-id="df60a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="df60a-113">**Element**</span></span>|<span data-ttu-id="df60a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="df60a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df60a-115">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="df60a-115">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="df60a-116">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="df60a-116">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df60a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="df60a-117">Text value</span></span>

 <span data-ttu-id="df60a-118">この要素を使用する場合は、日付/時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="df60a-118">A text value that represents a date/time is required if this element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="df60a-119">注釈</span><span class="sxs-lookup"><span data-stu-id="df60a-119">Remarks</span></span>

<span data-ttu-id="df60a-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="df60a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df60a-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="df60a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df60a-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="df60a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df60a-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df60a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="df60a-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="df60a-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="df60a-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df60a-125">Validation File</span></span>  <br/> |<span data-ttu-id="df60a-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="df60a-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df60a-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="df60a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="df60a-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="df60a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df60a-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="df60a-129">See also</span></span>



- [<span data-ttu-id="df60a-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="df60a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

