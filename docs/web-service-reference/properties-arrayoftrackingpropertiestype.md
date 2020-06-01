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
description: Properties 要素には、1つ以上の追跡プロパティの一覧が含まれています。
ms.openlocfilehash: 007a4dc14c84c47ea7af8ccacc554c134d563e44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465633"
---
# <a name="properties-arrayoftrackingpropertiestype"></a><span data-ttu-id="7e445-103">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="7e445-103">Properties (ArrayOfTrackingPropertiesType)</span></span>

<span data-ttu-id="7e445-104">**Properties**要素には、1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e445-104">The **Properties** element contains a list of one or more tracking properties.</span></span> 
  
- [<span data-ttu-id="7e445-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7e445-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
- [<span data-ttu-id="7e445-106">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="7e445-106">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

<span data-ttu-id="7e445-107">**ArrayOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="7e445-107">**ArrayOfTrackingPropertiesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e445-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e445-108">Attributes and elements</span></span>

<span data-ttu-id="7e445-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e445-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e445-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e445-110">Attributes</span></span>

<span data-ttu-id="7e445-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e445-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e445-112">子要素</span><span class="sxs-lookup"><span data-stu-id="7e445-112">Child elements</span></span>

|<span data-ttu-id="7e445-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="7e445-113">**Element**</span></span>|<span data-ttu-id="7e445-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e445-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e445-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="7e445-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="7e445-116">メッセージ追跡レポートのプロパティを作成するために使用される文字列の名前と値のペアを表します。</span><span class="sxs-lookup"><span data-stu-id="7e445-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e445-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7e445-117">Parent elements</span></span>

|<span data-ttu-id="7e445-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e445-118">**Element**</span></span>|<span data-ttu-id="7e445-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e445-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e445-120">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7e445-120">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="7e445-121">検索するメッセージの種類の条件を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e445-121">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="7e445-122">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="7e445-122">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7e445-123">単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7e445-123">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7e445-124">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="7e445-124">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="7e445-125">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="7e445-125">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="7e445-126">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="7e445-126">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="7e445-127">1つの[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e445-127">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7e445-128">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="7e445-128">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="7e445-129">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e445-129">Contains information for a single event for a recipient.</span></span>  <br/> |
|[<span data-ttu-id="7e445-130">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="7e445-130">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="7e445-131">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="7e445-131">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7e445-132">MessageTrackingSearchResult</span><span class="sxs-lookup"><span data-stu-id="7e445-132">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="7e445-133">[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="7e445-133">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e445-134">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e445-134">Text value</span></span>

<span data-ttu-id="7e445-135">なし。</span><span class="sxs-lookup"><span data-stu-id="7e445-135">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e445-136">注釈</span><span class="sxs-lookup"><span data-stu-id="7e445-136">Remarks</span></span>

<span data-ttu-id="7e445-137">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e445-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e445-138">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e445-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e445-139">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e445-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e445-140">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e445-140">Schema Name</span></span>  <br/> |<span data-ttu-id="7e445-141">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e445-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e445-142">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e445-142">Validation File</span></span>  <br/> |<span data-ttu-id="7e445-143">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7e445-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e445-144">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e445-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e445-145">正しくない</span><span class="sxs-lookup"><span data-stu-id="7e445-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e445-146">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e445-146">See also</span></span>

- [<span data-ttu-id="7e445-147">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="7e445-147">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="7e445-148">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="7e445-148">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="7e445-149">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e445-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

