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
description: GetMessageTrackingReport 要素には、指定された ID の完全なメッセージ追跡レポートを取得するための GetMessageTrackingReport 操作の要求が含まれています。
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44466578"
---
# <a name="getmessagetrackingreport"></a><span data-ttu-id="adad3-103">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="adad3-103">GetMessageTrackingReport</span></span>

<span data-ttu-id="adad3-104">**Getmessagetrackingreport**要素には、指定された ID の完全なメッセージ追跡レポートを取得するための[getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求が含まれています。</span><span class="sxs-lookup"><span data-stu-id="adad3-104">The **GetMessageTrackingReport** element contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span> 
  
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

 <span data-ttu-id="adad3-105">**GetMessageTrackingReportRequestType**</span><span class="sxs-lookup"><span data-stu-id="adad3-105">**GetMessageTrackingReportRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="adad3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="adad3-106">Attributes and elements</span></span>

<span data-ttu-id="adad3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="adad3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="adad3-108">属性</span><span class="sxs-lookup"><span data-stu-id="adad3-108">Attributes</span></span>

<span data-ttu-id="adad3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="adad3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="adad3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="adad3-110">Child elements</span></span>

|<span data-ttu-id="adad3-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="adad3-111">**Element**</span></span>|<span data-ttu-id="adad3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="adad3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="adad3-113">範囲 (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="adad3-113">Scope (NonEmptyStringType)</span></span>](scope-nonemptystringtype.md) <br/> |<span data-ttu-id="adad3-114">検索を実行する場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-114">Specifies where to perform the search.</span></span> <span data-ttu-id="adad3-115">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="adad3-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="adad3-116">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="adad3-116">ReportTemplate</span></span>](reporttemplate.md) <br/> |<span data-ttu-id="adad3-117">取得する追跡レポートの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-117">Specifies the type of tracking report to retrieve.</span></span> <span data-ttu-id="adad3-118">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="adad3-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="adad3-119">RecipientFilter</span><span class="sxs-lookup"><span data-stu-id="adad3-119">RecipientFilter</span></span>](recipientfilter.md) <br/> |<span data-ttu-id="adad3-120">指定した追跡レポートで使用する受信者のアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-120">Specifies a recipient address to use with the specified tracking report.</span></span> <span data-ttu-id="adad3-121">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="adad3-121">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="adad3-122">MessageTrackingReportId</span><span class="sxs-lookup"><span data-stu-id="adad3-122">MessageTrackingReportId</span></span>](messagetrackingreportid.md) <br/> |<span data-ttu-id="adad3-123">**Findmessagetrackingreport**操作から取得した id 文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-123">Specifies an identity string that was obtained from the **FindMessageTrackingReport** operation.</span></span> <span data-ttu-id="adad3-124">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="adad3-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="adad3-125">ReturnQueueEvents</span><span class="sxs-lookup"><span data-stu-id="adad3-125">ReturnQueueEvents</span></span>](returnqueueevents.md) <br/> |<span data-ttu-id="adad3-126">タスクを実行しているユーザーに特権ロールがあることを指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-126">Specifies that the person who is running the task has a privileged role.</span></span> <span data-ttu-id="adad3-127">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="adad3-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="adad3-128">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="adad3-128">DiagnosticsLevel</span></span>](diagnosticslevel.md) <br/> |<span data-ttu-id="adad3-129">追跡レポートを派生させるために使用されるタイミングとパフォーマンスの情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-129">Specifies timing and performance information that will be used to derive the tracking report.</span></span> <span data-ttu-id="adad3-130">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="adad3-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="adad3-131">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="adad3-131">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="adad3-132">1つまたは複数の追跡プロパティのリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="adad3-132">Specifies a list of one or more tracking properties.</span></span> <span data-ttu-id="adad3-133">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="adad3-133">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="adad3-134">親要素</span><span class="sxs-lookup"><span data-stu-id="adad3-134">Parent elements</span></span>

<span data-ttu-id="adad3-135">なし。</span><span class="sxs-lookup"><span data-stu-id="adad3-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="adad3-136">注釈</span><span class="sxs-lookup"><span data-stu-id="adad3-136">Remarks</span></span>

<span data-ttu-id="adad3-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="adad3-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="adad3-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="adad3-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="adad3-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="adad3-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="adad3-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="adad3-140">Schema Name</span></span>  <br/> |<span data-ttu-id="adad3-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="adad3-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="adad3-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="adad3-142">Validation File</span></span>  <br/> |<span data-ttu-id="adad3-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="adad3-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="adad3-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="adad3-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="adad3-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="adad3-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="adad3-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="adad3-146">See also</span></span>



[<span data-ttu-id="adad3-147">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="adad3-147">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="adad3-148">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="adad3-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

