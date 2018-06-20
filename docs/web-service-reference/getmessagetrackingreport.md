---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: GetMessageTrackingReport 要素には、指定した ID のレポートを追跡する、完全なメッセージを取得するために GetMessageTrackingReport 操作の要求が含まれています。
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760796"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="89f9d-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="89f9d-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="89f9d-104">**GetMessageTrackingReport**要素には、指定した ID のレポートを追跡する、完全なメッセージを取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="89f9d-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 <span data-ttu-id="89f9d-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="89f9d-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89f9d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="89f9d-106">Attributes and elements</span></span>

<span data-ttu-id="89f9d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89f9d-108">属性</span><span class="sxs-lookup"><span data-stu-id="89f9d-108">Attributes</span></span>

<span data-ttu-id="89f9d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="89f9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89f9d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="89f9d-110">Child elements</span></span>

|<span data-ttu-id="89f9d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="89f9d-111">**Element**</span></span>|<span data-ttu-id="89f9d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="89f9d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89f9d-113">スコープ (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="89f9d-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="89f9d-114">検索を実行する場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-114">Specifies where to perform the search.</span></span> <span data-ttu-id="89f9d-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="89f9d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-116">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="89f9d-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="89f9d-117">追跡を取得するレポートの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="89f9d-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="89f9d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="89f9d-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="89f9d-120">指定した追跡レポートで使用する受信者のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="89f9d-121">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="89f9d-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="89f9d-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="89f9d-123">**FindMessageTrackingReport**操作から取得された id 文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="89f9d-124">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="89f9d-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="89f9d-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="89f9d-126">タスクを実行している人が特権を持つ役割を持っているかを指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="89f9d-127">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="89f9d-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="89f9d-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="89f9d-129">追跡レポートを派生させるために使用されるタイミングとパフォーマンスの情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="89f9d-130">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="89f9d-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="89f9d-131">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="89f9d-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="89f9d-132">1 つまたは複数の追跡のプロパティの一覧を指定します。</span><span class="sxs-lookup"><span data-stu-id="89f9d-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="89f9d-133">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="89f9d-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89f9d-134">親要素</span><span class="sxs-lookup"><span data-stu-id="89f9d-134">Parent elements</span></span>

<span data-ttu-id="89f9d-135">なし。</span><span class="sxs-lookup"><span data-stu-id="89f9d-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89f9d-136">備考</span><span class="sxs-lookup"><span data-stu-id="89f9d-136">Remarks</span></span>

<span data-ttu-id="89f9d-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="89f9d-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89f9d-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="89f9d-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89f9d-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="89f9d-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89f9d-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="89f9d-140">Schema Name</span></span>  <br/> |<span data-ttu-id="89f9d-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="89f9d-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89f9d-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="89f9d-142">Validation File</span></span>  <br/> |<span data-ttu-id="89f9d-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89f9d-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89f9d-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="89f9d-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="89f9d-145">False</span><span class="sxs-lookup"><span data-stu-id="89f9d-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89f9d-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="89f9d-146">See also</span></span>



[<span data-ttu-id="89f9d-147">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="89f9d-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="89f9d-148">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="89f9d-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

