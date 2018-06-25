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
description: GetStreamingEventsResponse 要素は、GetStreamingEvents 要素の要求に対する応答を表します。
ms.openlocfilehash: 46e606c6093c0e9853668bea10cbdb006191f762
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831681"
---
# <a name="getstreamingeventsresponse"></a><span data-ttu-id="f64ad-103">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="f64ad-103">GetStreamingEventsResponse</span></span>

<span data-ttu-id="f64ad-104">**GetStreamingEventsResponse**要素は、 [GetStreamingEvents](getstreamingevents.md)要素の要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="f64ad-104">The **GetStreamingEventsResponse** element represents a response to a [GetStreamingEvents](getstreamingevents.md) element request.</span></span> 
  
```xml
<GetStreamingEventsResponse>
   <ResponseMessages/>
</GetStreamingEventsResponse>
```

 <span data-ttu-id="f64ad-105">**GetStreamingEventsResponseType**</span><span class="sxs-lookup"><span data-stu-id="f64ad-105">**GetStreamingEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f64ad-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f64ad-106">Attributes and elements</span></span>

<span data-ttu-id="f64ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f64ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f64ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="f64ad-108">Attributes</span></span>

<span data-ttu-id="f64ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f64ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f64ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f64ad-110">Child elements</span></span>

|<span data-ttu-id="f64ad-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f64ad-111">**Element**</span></span>|<span data-ttu-id="f64ad-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f64ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f64ad-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f64ad-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f64ad-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f64ad-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f64ad-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f64ad-115">Parent elements</span></span>

<span data-ttu-id="f64ad-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f64ad-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f64ad-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f64ad-117">Text value</span></span>

<span data-ttu-id="f64ad-118">なし。</span><span class="sxs-lookup"><span data-stu-id="f64ad-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f64ad-119">備考</span><span class="sxs-lookup"><span data-stu-id="f64ad-119">Remarks</span></span>

<span data-ttu-id="f64ad-120">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f64ad-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f64ad-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="f64ad-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f64ad-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="f64ad-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f64ad-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f64ad-123">Schema name</span></span>  <br/> |<span data-ttu-id="f64ad-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f64ad-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f64ad-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f64ad-125">Validation file</span></span>  <br/> |<span data-ttu-id="f64ad-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f64ad-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f64ad-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f64ad-127">Can be empty</span></span>  <br/> |<span data-ttu-id="f64ad-128">False</span><span class="sxs-lookup"><span data-stu-id="f64ad-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f64ad-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f64ad-129">See also</span></span>



[<span data-ttu-id="f64ad-130">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="f64ad-130">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="f64ad-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f64ad-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

