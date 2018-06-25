---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: ConnectionStatus 要素は、ストリーミングのサブスクリプションの状態の説明を提供します。
ms.openlocfilehash: 567308d79eaccba24230deddf5d78a724b8746af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759660"
---
# <a name="connectionstatus"></a><span data-ttu-id="7f97b-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="7f97b-103">ConnectionStatus</span></span>

<span data-ttu-id="7f97b-104">**ConnectionStatus**要素は、ストリーミングのサブスクリプションの状態の説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="7f97b-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="7f97b-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="7f97b-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f97b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f97b-106">Attributes and elements</span></span>

<span data-ttu-id="7f97b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f97b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f97b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f97b-108">Attributes</span></span>

<span data-ttu-id="7f97b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7f97b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f97b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7f97b-110">Child elements</span></span>

<span data-ttu-id="7f97b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7f97b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f97b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7f97b-112">Parent elements</span></span>

|<span data-ttu-id="7f97b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f97b-113">**Element**</span></span>|<span data-ttu-id="7f97b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f97b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f97b-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f97b-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="7f97b-116">状態および 1 つの結果が含まれています[GetStreamingEvents の操作](getstreamingevents-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="7f97b-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7f97b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7f97b-117">Text value</span></span>

<span data-ttu-id="7f97b-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="7f97b-118">A text value is required.</span></span> <span data-ttu-id="7f97b-119">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="7f97b-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="7f97b-120">OK</span><span class="sxs-lookup"><span data-stu-id="7f97b-120">OK</span></span>
    
- <span data-ttu-id="7f97b-121">更新不可</span><span class="sxs-lookup"><span data-stu-id="7f97b-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7f97b-122">備考</span><span class="sxs-lookup"><span data-stu-id="7f97b-122">Remarks</span></span>

<span data-ttu-id="7f97b-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7f97b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f97b-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f97b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f97b-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f97b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f97b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f97b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7f97b-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f97b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f97b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f97b-128">Validation File</span></span>  <br/> |<span data-ttu-id="7f97b-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f97b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f97b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7f97b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f97b-131">False</span><span class="sxs-lookup"><span data-stu-id="7f97b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f97b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f97b-132">See also</span></span>



[<span data-ttu-id="7f97b-133">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="7f97b-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="7f97b-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7f97b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

