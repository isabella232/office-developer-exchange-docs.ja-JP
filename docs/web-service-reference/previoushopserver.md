---
title: PreviousHopServer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousHopServer
api_type:
- schema
ms.assetid: 74456709-1250-4943-bae0-11a3db44a684
description: PreviousHopServer 要素は、メッセージを承諾する前のサーバー名を表します。
ms.openlocfilehash: d9641fdba3b7ef5b487139074c8e475edec9e74c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832879"
---
# <a name="previoushopserver"></a><span data-ttu-id="66b2c-103">PreviousHopServer</span><span class="sxs-lookup"><span data-stu-id="66b2c-103">PreviousHopServer</span></span>

<span data-ttu-id="66b2c-104">**PreviousHopServer**要素は、メッセージを承諾する前のサーバー名を表します。</span><span class="sxs-lookup"><span data-stu-id="66b2c-104">The **PreviousHopServer** element represents the previous server name that accepted the message.</span></span> 
  
```XML
<PreviousHopServer/>
```

 <span data-ttu-id="66b2c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="66b2c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66b2c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="66b2c-106">Attributes and elements</span></span>

<span data-ttu-id="66b2c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="66b2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66b2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="66b2c-108">Attributes</span></span>

<span data-ttu-id="66b2c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="66b2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66b2c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="66b2c-110">Child elements</span></span>

<span data-ttu-id="66b2c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="66b2c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66b2c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="66b2c-112">Parent elements</span></span>

|<span data-ttu-id="66b2c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="66b2c-113">**Element**</span></span>|<span data-ttu-id="66b2c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="66b2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66b2c-115">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="66b2c-115">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="66b2c-116">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66b2c-116">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66b2c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="66b2c-117">Text value</span></span>

<span data-ttu-id="66b2c-118">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="66b2c-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66b2c-119">備考</span><span class="sxs-lookup"><span data-stu-id="66b2c-119">Remarks</span></span>

<span data-ttu-id="66b2c-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="66b2c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66b2c-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="66b2c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66b2c-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="66b2c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66b2c-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="66b2c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="66b2c-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="66b2c-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="66b2c-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="66b2c-125">Validation File</span></span>  <br/> |<span data-ttu-id="66b2c-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66b2c-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66b2c-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="66b2c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="66b2c-128">False</span><span class="sxs-lookup"><span data-stu-id="66b2c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66b2c-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="66b2c-129">See also</span></span>



- [<span data-ttu-id="66b2c-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="66b2c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

