---
title: GetStreamingEventsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponse
api_type:
- schema
ms.assetid: ea1e7e7e-1b19-4e07-ba42-5dbd888c6db2
description: GetStreamingEvents Response 要素は、GetStreamingEvents 要素要求への応答を表します。
ms.openlocfilehash: 84cd4f0099ab0fda1c1fe771dca0d9ef932b132b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457726"
---
# <a name="getstreamingeventsresponse"></a><span data-ttu-id="96da8-103">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="96da8-103">GetStreamingEventsResponse</span></span>

<span data-ttu-id="96da8-104">**Getstreamingevents response**要素は、 [getstreamingevents](getstreamingevents.md)要素要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="96da8-104">The **GetStreamingEventsResponse** element represents a response to a [GetStreamingEvents](getstreamingevents.md) element request.</span></span> 
  
```xml
<GetStreamingEventsResponse>
   <ResponseMessages/>
</GetStreamingEventsResponse>
```

 <span data-ttu-id="96da8-105">**Getstreamingイベント Responsetype**</span><span class="sxs-lookup"><span data-stu-id="96da8-105">**GetStreamingEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96da8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="96da8-106">Attributes and elements</span></span>

<span data-ttu-id="96da8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="96da8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96da8-108">属性</span><span class="sxs-lookup"><span data-stu-id="96da8-108">Attributes</span></span>

<span data-ttu-id="96da8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="96da8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96da8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="96da8-110">Child elements</span></span>

|<span data-ttu-id="96da8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="96da8-111">**Element**</span></span>|<span data-ttu-id="96da8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="96da8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96da8-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="96da8-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="96da8-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="96da8-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96da8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="96da8-115">Parent elements</span></span>

<span data-ttu-id="96da8-116">なし。</span><span class="sxs-lookup"><span data-stu-id="96da8-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="96da8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="96da8-117">Text value</span></span>

<span data-ttu-id="96da8-118">なし。</span><span class="sxs-lookup"><span data-stu-id="96da8-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96da8-119">注釈</span><span class="sxs-lookup"><span data-stu-id="96da8-119">Remarks</span></span>

<span data-ttu-id="96da8-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="96da8-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96da8-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="96da8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96da8-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="96da8-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96da8-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="96da8-123">Schema name</span></span>  <br/> |<span data-ttu-id="96da8-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="96da8-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96da8-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="96da8-125">Validation file</span></span>  <br/> |<span data-ttu-id="96da8-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="96da8-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96da8-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="96da8-127">Can be empty</span></span>  <br/> |<span data-ttu-id="96da8-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="96da8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96da8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="96da8-129">See also</span></span>



[<span data-ttu-id="96da8-130">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="96da8-130">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="96da8-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="96da8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

