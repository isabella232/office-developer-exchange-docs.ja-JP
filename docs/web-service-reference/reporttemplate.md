---
title: ReportTemplate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: ReportTemplate 要素を取得するレポートの種類を表します。
ms.openlocfilehash: 70aab69f4d20ad9fd7e878c7fccd16e261c9b94c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833118"
---
# <a name="reporttemplate"></a><span data-ttu-id="ce0a9-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="ce0a9-103">ReportTemplate</span></span>

<span data-ttu-id="ce0a9-104">**ReportTemplate**要素を取得するレポートの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="ce0a9-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce0a9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ce0a9-106">Attributes and elements</span></span>

<span data-ttu-id="ce0a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce0a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce0a9-108">Attributes</span></span>

<span data-ttu-id="ce0a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce0a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ce0a9-110">Child elements</span></span>

<span data-ttu-id="ce0a9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce0a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ce0a9-112">Parent elements</span></span>

|<span data-ttu-id="ce0a9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-113">**Element**</span></span>|<span data-ttu-id="ce0a9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce0a9-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="ce0a9-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="ce0a9-116">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="ce0a9-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce0a9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ce0a9-117">Text value</span></span>

<span data-ttu-id="ce0a9-118">**ReportTemplate**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="ce0a9-119">**ReportTemplate 要素の値**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="ce0a9-120">**値**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-120">**Value**</span></span>|<span data-ttu-id="ce0a9-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="ce0a9-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ce0a9-122">概要</span><span class="sxs-lookup"><span data-stu-id="ce0a9-122">Summary</span></span>  <br/> |<span data-ttu-id="ce0a9-123">レポートを表示するメッセージのすべての受信者、メッセージの配信状態の各受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="ce0a9-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="ce0a9-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="ce0a9-125">1 人の受信者を指定するレポートでは発生したイベントの完全な履歴が表示されます。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce0a9-126">備考</span><span class="sxs-lookup"><span data-stu-id="ce0a9-126">Remarks</span></span>

<span data-ttu-id="ce0a9-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ce0a9-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce0a9-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="ce0a9-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce0a9-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="ce0a9-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce0a9-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ce0a9-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ce0a9-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ce0a9-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ce0a9-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ce0a9-132">Validation File</span></span>  <br/> |<span data-ttu-id="ce0a9-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce0a9-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce0a9-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ce0a9-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce0a9-135">False</span><span class="sxs-lookup"><span data-stu-id="ce0a9-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce0a9-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ce0a9-136">See also</span></span>



- [<span data-ttu-id="ce0a9-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ce0a9-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

