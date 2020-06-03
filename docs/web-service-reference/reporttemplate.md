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
description: ReportTemplate 要素は、取得するレポートの種類を表します。
ms.openlocfilehash: 22f14d326032a30e5cb4c2c9e1aff390d98e95e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528700"
---
# <a name="reporttemplate"></a><span data-ttu-id="da13b-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="da13b-103">ReportTemplate</span></span>

<span data-ttu-id="da13b-104">**Reporttemplate**要素は、取得するレポートの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="da13b-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="da13b-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="da13b-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da13b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="da13b-106">Attributes and elements</span></span>

<span data-ttu-id="da13b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="da13b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da13b-108">属性</span><span class="sxs-lookup"><span data-stu-id="da13b-108">Attributes</span></span>

<span data-ttu-id="da13b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="da13b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da13b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="da13b-110">Child elements</span></span>

<span data-ttu-id="da13b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="da13b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da13b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="da13b-112">Parent elements</span></span>

|<span data-ttu-id="da13b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="da13b-113">**Element**</span></span>|<span data-ttu-id="da13b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="da13b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da13b-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="da13b-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="da13b-116">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="da13b-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da13b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="da13b-117">Text value</span></span>

<span data-ttu-id="da13b-118">次の表に、 **Reporttemplate**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="da13b-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="da13b-119">**ReportTemplate 要素の値**</span><span class="sxs-lookup"><span data-stu-id="da13b-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="da13b-120">**値**</span><span class="sxs-lookup"><span data-stu-id="da13b-120">**Value**</span></span>|<span data-ttu-id="da13b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="da13b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da13b-122">概要</span><span class="sxs-lookup"><span data-stu-id="da13b-122">Summary</span></span>  <br/> |<span data-ttu-id="da13b-123">レポートがメッセージのすべての受信者を表示し、各受信者へのメッセージの配信状態を表示するように指定します。</span><span class="sxs-lookup"><span data-stu-id="da13b-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="da13b-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="da13b-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="da13b-125">単一の受信者に対して、発生したイベントの完全な履歴がレポートに表示されることを指定します。</span><span class="sxs-lookup"><span data-stu-id="da13b-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da13b-126">注釈</span><span class="sxs-lookup"><span data-stu-id="da13b-126">Remarks</span></span>

<span data-ttu-id="da13b-127">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="da13b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da13b-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="da13b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da13b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="da13b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="da13b-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="da13b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="da13b-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="da13b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="da13b-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="da13b-132">Validation File</span></span>  <br/> |<span data-ttu-id="da13b-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="da13b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="da13b-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="da13b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="da13b-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="da13b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da13b-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="da13b-136">See also</span></span>



- [<span data-ttu-id="da13b-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="da13b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

