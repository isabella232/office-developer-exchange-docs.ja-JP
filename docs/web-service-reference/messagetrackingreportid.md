---
title: MessageTrackingReportId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: MessageTrackingReportId 要素は、メッセージ ID、組織でメッセージが発見された、メッセージが送信されたサーバーとメッセージを一意に識別するための内部 ID でメッセージを表します。
ms.openlocfilehash: 8e0d85b203b8a34acedb5f6b9fe46359d5e0b97c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832456"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="cae4c-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="cae4c-103">MessageTrackingReportId</span></span>

<span data-ttu-id="cae4c-104">**MessageTrackingReportId**要素は、メッセージ ID、組織でメッセージが発見された、メッセージが送信されたサーバーとメッセージを一意に識別するための内部 ID でメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="cae4c-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="cae4c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="cae4c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cae4c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cae4c-106">Attributes and elements</span></span>

<span data-ttu-id="cae4c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cae4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cae4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="cae4c-108">Attributes</span></span>

<span data-ttu-id="cae4c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cae4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cae4c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cae4c-110">Child elements</span></span>

<span data-ttu-id="cae4c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cae4c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cae4c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cae4c-112">Parent elements</span></span>

|<span data-ttu-id="cae4c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cae4c-113">**Element**</span></span>|<span data-ttu-id="cae4c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cae4c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cae4c-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cae4c-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="cae4c-116">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="cae4c-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="cae4c-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="cae4c-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="cae4c-118">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cae4c-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cae4c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cae4c-119">Text value</span></span>

<span data-ttu-id="cae4c-120">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="cae4c-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cae4c-121">備考</span><span class="sxs-lookup"><span data-stu-id="cae4c-121">Remarks</span></span>

<span data-ttu-id="cae4c-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cae4c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cae4c-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="cae4c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cae4c-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="cae4c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cae4c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cae4c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cae4c-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cae4c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="cae4c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cae4c-127">Validation File</span></span>  <br/> |<span data-ttu-id="cae4c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cae4c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cae4c-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cae4c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cae4c-130">False</span><span class="sxs-lookup"><span data-stu-id="cae4c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cae4c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="cae4c-131">See also</span></span>



[<span data-ttu-id="cae4c-132">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="cae4c-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="cae4c-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cae4c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

