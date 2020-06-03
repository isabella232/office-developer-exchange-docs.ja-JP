---
title: ConnectionTimeout
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
description: ConnectionTimeout 要素は、接続を開いたままにする時間を分単位で指定します。
ms.openlocfilehash: 671e3cf5466ee8b3543036811708bd7f54afdcce
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463854"
---
# <a name="connectiontimeout"></a><span data-ttu-id="17cc1-103">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="17cc1-103">ConnectionTimeout</span></span>

<span data-ttu-id="17cc1-104">**ConnectionTimeout**要素は、接続を開いたままにする時間を分単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="17cc1-104">The **ConnectionTimeout** element specifies the number of minutes to keep a connection open.</span></span> 
  
[<span data-ttu-id="17cc1-105">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="17cc1-105">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="17cc1-106">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="17cc1-106">ConnectionTimeout</span></span>](connectiontimeout.md)
  
```xml
<ConnectionTimeout/>
```

 <span data-ttu-id="17cc1-107">**int**</span><span class="sxs-lookup"><span data-stu-id="17cc1-107">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17cc1-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17cc1-108">Attributes and elements</span></span>

<span data-ttu-id="17cc1-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17cc1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17cc1-110">属性</span><span class="sxs-lookup"><span data-stu-id="17cc1-110">Attributes</span></span>

<span data-ttu-id="17cc1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="17cc1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17cc1-112">子要素</span><span class="sxs-lookup"><span data-stu-id="17cc1-112">Child elements</span></span>

<span data-ttu-id="17cc1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="17cc1-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17cc1-114">親要素</span><span class="sxs-lookup"><span data-stu-id="17cc1-114">Parent elements</span></span>

|<span data-ttu-id="17cc1-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="17cc1-115">**Element**</span></span>|<span data-ttu-id="17cc1-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="17cc1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17cc1-117">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="17cc1-117">GetStreamingEvents</span></span>](getstreamingevents.md) <br/> |<span data-ttu-id="17cc1-118">ストリーミング接続からイベント通知を取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="17cc1-118">Defines a request to get event notifications from a streaming connection.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17cc1-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="17cc1-119">Text value</span></span>

<span data-ttu-id="17cc1-120">テキスト値は、ストリーミング接続を開いたままにしておく最大時間 (分単位) を示す整数を表します。</span><span class="sxs-lookup"><span data-stu-id="17cc1-120">The text value represents an integer that describes the maximum number of minutes to keep a streaming connection open.</span></span> <span data-ttu-id="17cc1-121">この値は、1 ~ 30 の範囲である必要があります。</span><span class="sxs-lookup"><span data-stu-id="17cc1-121">The value must be between 1 and 30, inclusive.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17cc1-122">注釈</span><span class="sxs-lookup"><span data-stu-id="17cc1-122">Remarks</span></span>

<span data-ttu-id="17cc1-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="17cc1-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17cc1-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="17cc1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17cc1-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="17cc1-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17cc1-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="17cc1-126">Schema name</span></span>  <br/> |<span data-ttu-id="17cc1-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="17cc1-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="17cc1-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="17cc1-128">Validation file</span></span>  <br/> |<span data-ttu-id="17cc1-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="17cc1-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17cc1-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="17cc1-130">Can be empty</span></span>  <br/> |<span data-ttu-id="17cc1-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="17cc1-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17cc1-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="17cc1-132">See also</span></span>



[<span data-ttu-id="17cc1-133">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="17cc1-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="17cc1-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="17cc1-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

