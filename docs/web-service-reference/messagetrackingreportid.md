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
description: MessageTrackingReportId 要素は、メッセージ ID、メッセージが検出された組織、メッセージが送信されたサーバー、メッセージを一意に識別する内部 ID によってメッセージを表します。
ms.openlocfilehash: d6e92593d55608e260634602c2aab694804d716d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460597"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="f45c3-103">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="f45c3-103">MessageTrackingReportId</span></span>

<span data-ttu-id="f45c3-104">**Messagetrackingreportid**要素は、メッセージ ID、メッセージが検出された組織、メッセージが送信されたサーバー、メッセージを一意に識別する内部 ID によってメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f45c3-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="f45c3-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="f45c3-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f45c3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f45c3-106">Attributes and elements</span></span>

<span data-ttu-id="f45c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f45c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f45c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="f45c3-108">Attributes</span></span>

<span data-ttu-id="f45c3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f45c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f45c3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f45c3-110">Child elements</span></span>

<span data-ttu-id="f45c3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f45c3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f45c3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f45c3-112">Parent elements</span></span>

|<span data-ttu-id="f45c3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f45c3-113">**Element**</span></span>|<span data-ttu-id="f45c3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f45c3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f45c3-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f45c3-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="f45c3-116">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="f45c3-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="f45c3-117">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="f45c3-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="f45c3-118">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="f45c3-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f45c3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f45c3-119">Text value</span></span>

<span data-ttu-id="f45c3-120">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="f45c3-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f45c3-121">注釈</span><span class="sxs-lookup"><span data-stu-id="f45c3-121">Remarks</span></span>

<span data-ttu-id="f45c3-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f45c3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f45c3-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f45c3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f45c3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f45c3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f45c3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f45c3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f45c3-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f45c3-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f45c3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f45c3-127">Validation File</span></span>  <br/> |<span data-ttu-id="f45c3-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f45c3-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f45c3-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f45c3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f45c3-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="f45c3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f45c3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f45c3-131">See also</span></span>



[<span data-ttu-id="f45c3-132">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="f45c3-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f45c3-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f45c3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

