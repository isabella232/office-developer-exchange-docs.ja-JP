---
title: Diagnostics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: 診断の要素は、データ ・ センターのレポートに使用されるタイミングとパフォーマンスの情報を提供します。
ms.openlocfilehash: 2b9cac54a683967ec274b8681fb9a0c8a844205e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760028"
---
# <a name="diagnostics"></a><span data-ttu-id="106ad-103">Diagnostics</span><span class="sxs-lookup"><span data-stu-id="106ad-103">Diagnostics</span></span>

<span data-ttu-id="106ad-104">**診断**の要素は、データ ・ センターのレポートに使用されるタイミングとパフォーマンスの情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="106ad-104">The **Diagnostics** element provides timing and performance information that is used for reporting in a DataCenter.</span></span> 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 <span data-ttu-id="106ad-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="106ad-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="106ad-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="106ad-106">Attributes and elements</span></span>

<span data-ttu-id="106ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="106ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="106ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="106ad-108">Attributes</span></span>

<span data-ttu-id="106ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="106ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="106ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="106ad-110">Child elements</span></span>

|<span data-ttu-id="106ad-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="106ad-111">**Element**</span></span>|<span data-ttu-id="106ad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="106ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="106ad-113">String</span><span class="sxs-lookup"><span data-stu-id="106ad-113">String</span></span>](string.md) <br/> |<span data-ttu-id="106ad-114">アイテム、連絡先、タスク、および会話で使用される文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="106ad-114">Contains a string that is used by items, contacts, tasks, and conversations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="106ad-115">親要素</span><span class="sxs-lookup"><span data-stu-id="106ad-115">Parent elements</span></span>

|<span data-ttu-id="106ad-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="106ad-116">**Element**</span></span>|<span data-ttu-id="106ad-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="106ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="106ad-118">FindMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="106ad-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="106ad-119">状態および 1 つの結果が含まれています[FindMessageTrackingReport の操作](findmessagetrackingreport-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="106ad-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="106ad-120">GetMessageTrackingReportResponse</span><span class="sxs-lookup"><span data-stu-id="106ad-120">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="106ad-121">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="106ad-121">Contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="106ad-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="106ad-122">Text value</span></span>

<span data-ttu-id="106ad-123">なし。</span><span class="sxs-lookup"><span data-stu-id="106ad-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="106ad-124">備考</span><span class="sxs-lookup"><span data-stu-id="106ad-124">Remarks</span></span>

<span data-ttu-id="106ad-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="106ad-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="106ad-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="106ad-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="106ad-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="106ad-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="106ad-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="106ad-128">Schema Name</span></span>  <br/> |<span data-ttu-id="106ad-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="106ad-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="106ad-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="106ad-130">Validation File</span></span>  <br/> |<span data-ttu-id="106ad-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="106ad-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="106ad-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="106ad-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="106ad-133">False</span><span class="sxs-lookup"><span data-stu-id="106ad-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="106ad-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="106ad-134">See also</span></span>

- [<span data-ttu-id="106ad-135">FindMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="106ad-135">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="106ad-136">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="106ad-136">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="106ad-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="106ad-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

