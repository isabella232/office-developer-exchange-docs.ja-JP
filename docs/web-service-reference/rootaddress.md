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
description: RootAddress 要素は、受信者 Trackingevent イベントのイベントを開始する最初のアドレスを表します。
ms.openlocfilehash: e020ff07f271bdde6c2a4172141097dcba66f64e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465094"
---
# <a name="rootaddress"></a><span data-ttu-id="09bd9-103">RootAddress</span><span class="sxs-lookup"><span data-stu-id="09bd9-103">RootAddress</span></span>

<span data-ttu-id="09bd9-104">**Rootaddress**要素は、[受信者 trackingevent](recipienttrackingevent.md)イベントのイベントを開始する最初のアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="09bd9-104">The **RootAddress** element represents the first address that starts the event for a [RecipientTrackingEvent](recipienttrackingevent.md) event.</span></span> 
  
```xml
<RootAddress/>
```

 <span data-ttu-id="09bd9-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="09bd9-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09bd9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="09bd9-106">Attributes and elements</span></span>

<span data-ttu-id="09bd9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="09bd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09bd9-108">属性</span><span class="sxs-lookup"><span data-stu-id="09bd9-108">Attributes</span></span>

<span data-ttu-id="09bd9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="09bd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09bd9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="09bd9-110">Child elements</span></span>

<span data-ttu-id="09bd9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="09bd9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09bd9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="09bd9-112">Parent elements</span></span>

|<span data-ttu-id="09bd9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="09bd9-113">**Element**</span></span>|<span data-ttu-id="09bd9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="09bd9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09bd9-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="09bd9-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="09bd9-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="09bd9-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09bd9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="09bd9-117">Text value</span></span>

<span data-ttu-id="09bd9-118">テキスト値は、追跡イベントを開始するアドレスです。</span><span class="sxs-lookup"><span data-stu-id="09bd9-118">The text value is the address that starts the tracking event.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09bd9-119">注釈</span><span class="sxs-lookup"><span data-stu-id="09bd9-119">Remarks</span></span>

<span data-ttu-id="09bd9-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="09bd9-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09bd9-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="09bd9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09bd9-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="09bd9-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09bd9-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="09bd9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="09bd9-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="09bd9-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="09bd9-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="09bd9-125">Validation File</span></span>  <br/> |<span data-ttu-id="09bd9-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="09bd9-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09bd9-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="09bd9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="09bd9-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="09bd9-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09bd9-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="09bd9-129">See also</span></span>



[<span data-ttu-id="09bd9-130">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="09bd9-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="09bd9-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="09bd9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

