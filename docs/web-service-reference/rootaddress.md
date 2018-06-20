---
title: RootAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootAddress
api_type:
- schema
ms.assetid: 1dbb130a-e4eb-4baf-ae07-2568a8375bff
description: RootAddress 要素は、RecipientTrackingEvent イベントのイベントを開始する最初のアドレスを表します。
ms.openlocfilehash: afe544d6ee8dea4cb416ad033ed2cd68976ec087
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833250"
---
# <a name="rootaddress"></a><span data-ttu-id="4393f-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="4393f-103">RootAddress</span></span>

<span data-ttu-id="4393f-104">**RootAddress**要素は、 [RecipientTrackingEvent](recipienttrackingevent.md)イベントのイベントを開始する最初のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="4393f-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="4393f-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="4393f-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4393f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4393f-106">Attributes and elements</span></span>

<span data-ttu-id="4393f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4393f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4393f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4393f-108">Attributes</span></span>

<span data-ttu-id="4393f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4393f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4393f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4393f-110">Child elements</span></span>

<span data-ttu-id="4393f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4393f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4393f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4393f-112">Parent elements</span></span>

|<span data-ttu-id="4393f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4393f-113">**Element**</span></span>|<span data-ttu-id="4393f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4393f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4393f-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="4393f-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="4393f-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4393f-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4393f-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4393f-117">Text value</span></span>

<span data-ttu-id="4393f-118">テキスト値は、追跡イベントを開始するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="4393f-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4393f-119">備考</span><span class="sxs-lookup"><span data-stu-id="4393f-119">Remarks</span></span>

<span data-ttu-id="4393f-120">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="4393f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4393f-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="4393f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4393f-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="4393f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4393f-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4393f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="4393f-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4393f-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="4393f-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4393f-125">Validation File</span></span>  <br/> |<span data-ttu-id="4393f-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4393f-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4393f-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4393f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="4393f-128">False</span><span class="sxs-lookup"><span data-stu-id="4393f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4393f-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4393f-129">See also</span></span>



[<span data-ttu-id="4393f-130">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="4393f-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="4393f-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4393f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

