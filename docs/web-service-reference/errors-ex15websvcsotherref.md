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
description: Errors 要素には、Web サービスによって返されるエラーを格納するためのプロパティバッグが含まれています。
ms.openlocfilehash: a2f888a81791fe0b57eee6123c4b0f5f609f3e75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465906"
---
# <a name="errors"></a><span data-ttu-id="885bb-103">エラー</span><span class="sxs-lookup"><span data-stu-id="885bb-103">Errors</span></span>

<span data-ttu-id="885bb-104">**Errors**要素には、Web サービスによって返されるエラーを格納するためのプロパティバッグが含まれています。</span><span class="sxs-lookup"><span data-stu-id="885bb-104">The **Errors** element contains a property bag to store errors that are returned through the Web service.</span></span> 
  
[<span data-ttu-id="885bb-105">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="885bb-105">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md)
  
[<span data-ttu-id="885bb-106">エラー</span><span class="sxs-lookup"><span data-stu-id="885bb-106">Errors</span></span>](errors-ex15websvcsotherref.md)
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 <span data-ttu-id="885bb-107">**ArrayOfArraysOfTrackingPropertiesType**</span><span class="sxs-lookup"><span data-stu-id="885bb-107">**ArrayOfArraysOfTrackingPropertiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="885bb-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="885bb-108">Attributes and elements</span></span>

<span data-ttu-id="885bb-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="885bb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="885bb-110">属性</span><span class="sxs-lookup"><span data-stu-id="885bb-110">Attributes</span></span>

<span data-ttu-id="885bb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="885bb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="885bb-112">子要素</span><span class="sxs-lookup"><span data-stu-id="885bb-112">Child elements</span></span>

|<span data-ttu-id="885bb-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="885bb-113">**Element**</span></span>|<span data-ttu-id="885bb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="885bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="885bb-115">プロパティ (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="885bb-115">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="885bb-116">1つ以上の追跡プロパティの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="885bb-116">Contains a list of one or more tracking properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="885bb-117">親要素</span><span class="sxs-lookup"><span data-stu-id="885bb-117">Parent elements</span></span>

|<span data-ttu-id="885bb-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="885bb-118">**Element**</span></span>|<span data-ttu-id="885bb-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="885bb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="885bb-120">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="885bb-120">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="885bb-121">単一の[Findmessagetrackingreport 操作](findmessagetrackingreport-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="885bb-121">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="885bb-122">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="885bb-122">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="885bb-123">1つの[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="885bb-123">Contains the result of a single [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="885bb-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="885bb-124">Text value</span></span>

<span data-ttu-id="885bb-125">なし。</span><span class="sxs-lookup"><span data-stu-id="885bb-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="885bb-126">注釈</span><span class="sxs-lookup"><span data-stu-id="885bb-126">Remarks</span></span>

<span data-ttu-id="885bb-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="885bb-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="885bb-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="885bb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="885bb-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="885bb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="885bb-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="885bb-130">Schema Name</span></span>  <br/> |<span data-ttu-id="885bb-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="885bb-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="885bb-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="885bb-132">Validation File</span></span>  <br/> |<span data-ttu-id="885bb-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="885bb-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="885bb-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="885bb-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="885bb-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="885bb-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="885bb-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="885bb-136">See also</span></span>



[<span data-ttu-id="885bb-137">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="885bb-137">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
  
[<span data-ttu-id="885bb-138">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="885bb-138">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="885bb-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="885bb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

