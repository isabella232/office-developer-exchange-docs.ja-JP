---
title: InternalId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalId
api_type:
- schema
ms.assetid: c179db1a-95c9-40da-bd3f-0bed548c0325
description: InternalId 要素は、イベント id の整数値を表します。
ms.openlocfilehash: 66d5852e104de843911b46a225154ebd991e2220
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459939"
---
# <a name="internalid"></a><span data-ttu-id="f67dd-103">InternalId</span><span class="sxs-lookup"><span data-stu-id="f67dd-103">InternalId</span></span>

<span data-ttu-id="f67dd-104">**Internalid**要素は、イベント id の整数値を表します。</span><span class="sxs-lookup"><span data-stu-id="f67dd-104">The **InternalId** element represents an integer value for the event identification.</span></span> 
  
```XML
<InternalId/>
```

 <span data-ttu-id="f67dd-105">**nonNegativeInteger**</span><span class="sxs-lookup"><span data-stu-id="f67dd-105">**nonNegativeInteger**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f67dd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f67dd-106">Attributes and elements</span></span>

<span data-ttu-id="f67dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f67dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f67dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="f67dd-108">Attributes</span></span>

<span data-ttu-id="f67dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f67dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f67dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f67dd-110">Child elements</span></span>

<span data-ttu-id="f67dd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f67dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f67dd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f67dd-112">Parent elements</span></span>

|<span data-ttu-id="f67dd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f67dd-113">**Element**</span></span>|<span data-ttu-id="f67dd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f67dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f67dd-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="f67dd-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="f67dd-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f67dd-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f67dd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f67dd-117">Text value</span></span>

<span data-ttu-id="f67dd-118">この要素を使用する場合は、整数を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="f67dd-118">A text value that represents an integer is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f67dd-119">注釈</span><span class="sxs-lookup"><span data-stu-id="f67dd-119">Remarks</span></span>

<span data-ttu-id="f67dd-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f67dd-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f67dd-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f67dd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f67dd-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="f67dd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f67dd-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f67dd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f67dd-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f67dd-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f67dd-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f67dd-125">Validation File</span></span>  <br/> |<span data-ttu-id="f67dd-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f67dd-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f67dd-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f67dd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f67dd-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="f67dd-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f67dd-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f67dd-129">See also</span></span>



- [<span data-ttu-id="f67dd-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f67dd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

