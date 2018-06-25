---
title: プロパティ (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: プロパティ要素には、1 つまたは複数の追跡のプロパティの一覧が含まれています。
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="b4aa2-103">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="b4aa2-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="b4aa2-104">**プロパティ**要素には、1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="b4aa2-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b4aa2-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="b4aa2-106">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="b4aa2-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="b4aa2-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="b4aa2-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b4aa2-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b4aa2-108">Attributes and elements</span></span>

<span data-ttu-id="b4aa2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4aa2-110">属性</span><span class="sxs-lookup"><span data-stu-id="b4aa2-110">Attributes</span></span>

<span data-ttu-id="b4aa2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4aa2-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b4aa2-112">Child elements</span></span>

|<span data-ttu-id="b4aa2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4aa2-113">**Element**</span></span>|<span data-ttu-id="b4aa2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4aa2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4aa2-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="b4aa2-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="b4aa2-116">名前と値文字列のペアを使用してレポートを追跡するメッセージのプロパティを作成するを表します。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4aa2-117">親要素</span><span class="sxs-lookup"><span data-stu-id="b4aa2-117">Parent elements</span></span>

|<span data-ttu-id="b4aa2-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="b4aa2-118">**Element**</span></span>|<span data-ttu-id="b4aa2-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b4aa2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4aa2-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b4aa2-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b4aa2-121">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="b4aa2-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="b4aa2-123">状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b4aa2-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="b4aa2-125">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="b4aa2-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="b4aa2-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="b4aa2-127">1 つの結果が含まれています[GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-128">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="b4aa2-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="b4aa2-129">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-130">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b4aa2-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="b4aa2-131">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b4aa2-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="b4aa2-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="b4aa2-133">[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md)要素の 1 つのメッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b4aa2-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b4aa2-134">Text value</span></span>

<span data-ttu-id="b4aa2-135">なし。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b4aa2-136">備考</span><span class="sxs-lookup"><span data-stu-id="b4aa2-136">Remarks</span></span>

<span data-ttu-id="b4aa2-137">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b4aa2-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4aa2-138">要素情報</span><span class="sxs-lookup"><span data-stu-id="b4aa2-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4aa2-139">名前空間</span><span class="sxs-lookup"><span data-stu-id="b4aa2-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b4aa2-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b4aa2-140">Schema Name</span></span>  <br/> |<span data-ttu-id="b4aa2-141">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b4aa2-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b4aa2-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b4aa2-142">Validation File</span></span>  <br/> |<span data-ttu-id="b4aa2-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b4aa2-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b4aa2-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b4aa2-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4aa2-145">False</span><span class="sxs-lookup"><span data-stu-id="b4aa2-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4aa2-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="b4aa2-146">See also</span></span>

- [<span data-ttu-id="b4aa2-147">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="b4aa2-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="b4aa2-148">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="b4aa2-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="b4aa2-149">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b4aa2-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

