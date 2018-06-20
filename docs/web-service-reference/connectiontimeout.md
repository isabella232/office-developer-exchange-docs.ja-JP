---
title: タイムアウト
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionTimeout
api_type:
- schema
ms.assetid: 14da68a0-bcca-4281-a774-47644baa4ee9
description: タイムアウト要素は、接続を開いたままにしておく秒数を指定します。
ms.openlocfilehash: 2bb40ba502853c70ef107c4c740fdfe7073abe31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759659"
---
# <a name="connectiontimeout"></a><span data-ttu-id="fb939-103">タイムアウト</span><span class="sxs-lookup"><span data-stu-id="fb939-103">ConnectionTimeout</span></span>

<span data-ttu-id="fb939-104">**タイムアウト**要素は、接続を開いたままにしておく秒数を指定します。</span><span class="sxs-lookup"><span data-stu-id="fb939-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="fb939-105">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="fb939-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="fb939-106">タイムアウト</span><span class="sxs-lookup"><span data-stu-id="fb939-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="fb939-107">**int**</span><span class="sxs-lookup"><span data-stu-id="fb939-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb939-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fb939-108">Attributes and elements</span></span>

<span data-ttu-id="fb939-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb939-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb939-110">属性</span><span class="sxs-lookup"><span data-stu-id="fb939-110">Attributes</span></span>

<span data-ttu-id="fb939-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fb939-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb939-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fb939-112">Child elements</span></span>

<span data-ttu-id="fb939-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fb939-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb939-114">親要素</span><span class="sxs-lookup"><span data-stu-id="fb939-114">Parent elements</span></span>

|<span data-ttu-id="fb939-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="fb939-115">**Element**</span></span>|<span data-ttu-id="fb939-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="fb939-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb939-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="fb939-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="fb939-118">ストリーミング接続からイベント通知を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="fb939-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb939-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fb939-119">Text value</span></span>

<span data-ttu-id="fb939-120">テキスト値では、ストリーミング接続を開いたままにする時間 (分) の最大数を示す整数を表します。</span><span class="sxs-lookup"><span data-stu-id="fb939-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="fb939-121">値は、1 から 30 日までの間でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="fb939-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb939-122">備考</span><span class="sxs-lookup"><span data-stu-id="fb939-122">Remarks</span></span>

<span data-ttu-id="fb939-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="fb939-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb939-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="fb939-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb939-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="fb939-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb939-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb939-126">Schema name</span></span>  <br/> |<span data-ttu-id="fb939-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fb939-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb939-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb939-128">Validation file</span></span>  <br/> |<span data-ttu-id="fb939-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb939-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb939-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb939-130">Can be empty</span></span>  <br/> |<span data-ttu-id="fb939-131">False</span><span class="sxs-lookup"><span data-stu-id="fb939-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb939-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="fb939-132">See also</span></span>



[<span data-ttu-id="fb939-133">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="fb939-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="fb939-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fb939-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

