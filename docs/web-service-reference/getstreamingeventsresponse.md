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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831681"
---
# <a name="getstreamingeventsresponse"></a><span data-ttu-id="ea606-103">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="ea606-103">GetStreamingEventsResponse</span></span>

<span data-ttu-id="ea606-104">**GetStreamingEventsResponse**要素は、 [GetStreamingEvents](getstreamingevents.md)要素の要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="ea606-104">The **GetStreamingEventsResponse** element represents a response to a [GetStreamingEvents](getstreamingevents.md) element request.</span></span> 
  
```xml
<GetStreamingEventsResponse>
   <ResponseMessages/>
</GetStreamingEventsResponse>
```

 <span data-ttu-id="ea606-105">**GetStreamingEventsResponseType**</span><span class="sxs-lookup"><span data-stu-id="ea606-105">**GetStreamingEventsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea606-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea606-106">Attributes and elements</span></span>

<span data-ttu-id="ea606-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea606-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea606-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea606-108">Attributes</span></span>

<span data-ttu-id="ea606-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ea606-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea606-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ea606-110">Child elements</span></span>

|<span data-ttu-id="ea606-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea606-111">**Element**</span></span>|<span data-ttu-id="ea606-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea606-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea606-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ea606-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ea606-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea606-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea606-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ea606-115">Parent elements</span></span>

<span data-ttu-id="ea606-116">なし。</span><span class="sxs-lookup"><span data-stu-id="ea606-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ea606-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ea606-117">Text value</span></span>

<span data-ttu-id="ea606-118">なし。</span><span class="sxs-lookup"><span data-stu-id="ea606-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea606-119">備考</span><span class="sxs-lookup"><span data-stu-id="ea606-119">Remarks</span></span>

<span data-ttu-id="ea606-120">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="ea606-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea606-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea606-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea606-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea606-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea606-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea606-123">Schema name</span></span>  <br/> |<span data-ttu-id="ea606-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="ea606-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea606-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea606-125">Validation file</span></span>  <br/> |<span data-ttu-id="ea606-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ea606-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea606-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ea606-127">Can be empty</span></span>  <br/> |<span data-ttu-id="ea606-128">False</span><span class="sxs-lookup"><span data-stu-id="ea606-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea606-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea606-129">See also</span></span>



[<span data-ttu-id="ea606-130">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="ea606-130">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="ea606-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ea606-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

