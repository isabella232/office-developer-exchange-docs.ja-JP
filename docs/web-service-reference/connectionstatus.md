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
description: ConnectionStatus 要素は、ストリーミングサブスクリプションの状態に関するテキストの説明を提供します。
ms.openlocfilehash: 928537201041950011ae06444e3c412228d252ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462718"
---
# <a name="connectionstatus"></a><span data-ttu-id="c8c8b-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="c8c8b-103">ConnectionStatus</span></span>

<span data-ttu-id="c8c8b-104">**Connectionstatus**要素は、ストリーミングサブスクリプションの状態に関するテキストの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="c8c8b-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="c8c8b-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8c8b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c8c8b-106">Attributes and elements</span></span>

<span data-ttu-id="c8c8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8c8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8c8b-108">Attributes</span></span>

<span data-ttu-id="c8c8b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8c8b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c8c8b-110">Child elements</span></span>

<span data-ttu-id="c8c8b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8c8b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c8c8b-112">Parent elements</span></span>

|<span data-ttu-id="c8c8b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c8c8b-113">**Element**</span></span>|<span data-ttu-id="c8c8b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c8c8b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8c8b-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c8c8b-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="c8c8b-116">1つの[Getstreamingevents 操作](getstreamingevents-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8c8b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c8c8b-117">Text value</span></span>

<span data-ttu-id="c8c8b-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-118">A text value is required.</span></span> <span data-ttu-id="c8c8b-119">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="c8c8b-120">OK</span><span class="sxs-lookup"><span data-stu-id="c8c8b-120">OK</span></span>
    
- <span data-ttu-id="c8c8b-121">更新不可</span><span class="sxs-lookup"><span data-stu-id="c8c8b-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c8c8b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="c8c8b-122">Remarks</span></span>

<span data-ttu-id="c8c8b-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c8c8b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8c8b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c8c8b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8c8b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8c8b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c8c8b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c8c8b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c8c8b-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c8c8b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c8c8b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c8c8b-128">Validation File</span></span>  <br/> |<span data-ttu-id="c8c8b-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c8c8b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8c8b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c8c8b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8c8b-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="c8c8b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8c8b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="c8c8b-132">See also</span></span>



[<span data-ttu-id="c8c8b-133">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="c8c8b-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="c8c8b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c8c8b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

