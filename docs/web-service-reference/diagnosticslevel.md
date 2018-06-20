---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: DiagnosticsLevel 要素は、レポートを派生させるために使用されるタイミングとパフォーマンスの情報を表します。
ms.openlocfilehash: 9205625bb6cf38e370e29d96770eb293ed9277f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760030"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="54330-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="54330-103">DiagnosticsLevel</span></span>

<span data-ttu-id="54330-104">**DiagnosticsLevel**要素は、レポートを派生させるために使用されるタイミングとパフォーマンスの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="54330-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="54330-105">**string**</span><span class="sxs-lookup"><span data-stu-id="54330-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54330-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="54330-106">Attributes and elements</span></span>

<span data-ttu-id="54330-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="54330-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54330-108">属性</span><span class="sxs-lookup"><span data-stu-id="54330-108">Attributes</span></span>

<span data-ttu-id="54330-109">なし。</span><span class="sxs-lookup"><span data-stu-id="54330-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54330-110">子要素</span><span class="sxs-lookup"><span data-stu-id="54330-110">Child elements</span></span>

<span data-ttu-id="54330-111">なし。</span><span class="sxs-lookup"><span data-stu-id="54330-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54330-112">親要素</span><span class="sxs-lookup"><span data-stu-id="54330-112">Parent elements</span></span>

|<span data-ttu-id="54330-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="54330-113">**Element**</span></span>|<span data-ttu-id="54330-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="54330-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54330-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="54330-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="54330-116">検索するメッセージの種類の条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54330-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="54330-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="54330-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="54330-118">レポートを指定した ID の追跡を取得するために[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)の要求が含まれています</span><span class="sxs-lookup"><span data-stu-id="54330-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54330-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="54330-119">Text value</span></span>

<span data-ttu-id="54330-120">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="54330-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54330-121">備考</span><span class="sxs-lookup"><span data-stu-id="54330-121">Remarks</span></span>

<span data-ttu-id="54330-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="54330-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54330-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="54330-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54330-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="54330-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54330-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="54330-125">Schema Name</span></span>  <br/> |<span data-ttu-id="54330-126">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="54330-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54330-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="54330-127">Validation File</span></span>  <br/> |<span data-ttu-id="54330-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54330-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54330-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="54330-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="54330-130">False</span><span class="sxs-lookup"><span data-stu-id="54330-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54330-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="54330-131">See also</span></span>

- [<span data-ttu-id="54330-132">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="54330-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="54330-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="54330-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

