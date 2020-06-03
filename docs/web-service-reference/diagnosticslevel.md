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
ms.openlocfilehash: 3060d4f1b8449a5870d964bdfcdbf0d503905abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467831"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="bb56c-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="bb56c-103">DiagnosticsLevel</span></span>

<span data-ttu-id="bb56c-104">**DiagnosticsLevel**要素は、レポートを派生させるために使用されるタイミングとパフォーマンスの情報を表します。</span><span class="sxs-lookup"><span data-stu-id="bb56c-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="bb56c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="bb56c-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb56c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bb56c-106">Attributes and elements</span></span>

<span data-ttu-id="bb56c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb56c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb56c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb56c-108">Attributes</span></span>

<span data-ttu-id="bb56c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bb56c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb56c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bb56c-110">Child elements</span></span>

<span data-ttu-id="bb56c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="bb56c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bb56c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="bb56c-112">Parent elements</span></span>

|<span data-ttu-id="bb56c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="bb56c-113">**Element**</span></span>|<span data-ttu-id="bb56c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb56c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb56c-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="bb56c-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="bb56c-116">検索するメッセージの種類に関する条件を含みます。</span><span class="sxs-lookup"><span data-stu-id="bb56c-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="bb56c-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="bb56c-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="bb56c-118">指定された ID の完全なメッセージ追跡レポートを取得する[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)の要求を含みます。</span><span class="sxs-lookup"><span data-stu-id="bb56c-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb56c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bb56c-119">Text value</span></span>

<span data-ttu-id="bb56c-120">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb56c-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb56c-121">注釈</span><span class="sxs-lookup"><span data-stu-id="bb56c-121">Remarks</span></span>

<span data-ttu-id="bb56c-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bb56c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb56c-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bb56c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb56c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="bb56c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb56c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bb56c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bb56c-126">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bb56c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb56c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bb56c-127">Validation File</span></span>  <br/> |<span data-ttu-id="bb56c-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bb56c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb56c-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bb56c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb56c-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="bb56c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb56c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb56c-131">See also</span></span>

- [<span data-ttu-id="bb56c-132">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="bb56c-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="bb56c-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bb56c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

