---
title: エラー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Errors
api_type:
- schema
ms.assetid: ea37a2b5-e2d1-4089-960f-7014b9535a50
description: エラー要素には、Web サービスから返されるエラーを格納するプロパティ バッグが含まれています。
ms.openlocfilehash: a029492c1e3c11cc31d3501bd4ea0024ef8ecb91
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760333"
---
# <a name="errors"></a><span data-ttu-id="1cf3d-103">エラー</span><span class="sxs-lookup"><span data-stu-id="1cf3d-103">Errors</span></span>

<span data-ttu-id="1cf3d-104">**エラー**要素には、Web サービスから返されるエラーを格納するプロパティ バッグが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-104">The **Errors** element contains a property bag to store errors that are returned through the Web service.</span></span> 
  
[<span data-ttu-id="1cf3d-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="1cf3d-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
[<span data-ttu-id="1cf3d-106">エラー</span><span class="sxs-lookup"><span data-stu-id="1cf3d-106">Errors</span></span>](errors-ex15websvcsotherref.md)
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 <span data-ttu-id="1cf3d-107">**ArrayOfArraysOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="1cf3d-107">**ArrayOfArraysOfTrackingPropertiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cf3d-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1cf3d-108">Attributes and elements</span></span>

<span data-ttu-id="1cf3d-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cf3d-110">属性</span><span class="sxs-lookup"><span data-stu-id="1cf3d-110">Attributes</span></span>

<span data-ttu-id="1cf3d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cf3d-112">子要素</span><span class="sxs-lookup"><span data-stu-id="1cf3d-112">Child elements</span></span>

|<span data-ttu-id="1cf3d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cf3d-113">**Element**</span></span>|<span data-ttu-id="1cf3d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cf3d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cf3d-115">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="1cf3d-115">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="1cf3d-116">1 つまたは複数の追跡のプロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-116">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cf3d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="1cf3d-117">Parent elements</span></span>

|<span data-ttu-id="1cf3d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cf3d-118">**Element**</span></span>|<span data-ttu-id="1cf3d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cf3d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cf3d-120">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="1cf3d-120">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="1cf3d-121">状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-121">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="1cf3d-122">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="1cf3d-122">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="1cf3d-123">1 つの結果が含まれています[GetMessageTrackingReport の操作](getmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-123">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1cf3d-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1cf3d-124">Text value</span></span>

<span data-ttu-id="1cf3d-125">なし。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cf3d-126">備考</span><span class="sxs-lookup"><span data-stu-id="1cf3d-126">Remarks</span></span>

<span data-ttu-id="1cf3d-127">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1cf3d-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cf3d-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="1cf3d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cf3d-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="1cf3d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cf3d-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cf3d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1cf3d-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1cf3d-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1cf3d-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cf3d-132">Validation File</span></span>  <br/> |<span data-ttu-id="1cf3d-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cf3d-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cf3d-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1cf3d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cf3d-135">False</span><span class="sxs-lookup"><span data-stu-id="1cf3d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cf3d-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cf3d-136">See also</span></span>



[<span data-ttu-id="1cf3d-137">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="1cf3d-137">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="1cf3d-138">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="1cf3d-138">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="1cf3d-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1cf3d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

