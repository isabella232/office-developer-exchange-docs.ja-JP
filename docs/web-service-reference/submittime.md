---
title: SubmitTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubmitTime
api_type:
- schema
ms.assetid: 97e4b71e-f45c-4bdb-80f9-805934916c0f
description: SubmitTime 要素は、サーバーにあるメッセージが送信された時刻を表します。
ms.openlocfilehash: 3f19e2ac14b412ef8d1ab59eb069f0223cf782ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833617"
---
# <a name="submittime"></a><span data-ttu-id="f1cb7-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="f1cb7-103">SubmitTime</span></span>

<span data-ttu-id="f1cb7-104">**SubmitTime**要素は、サーバーにあるメッセージが送信された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="f1cb7-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f1cb7-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1cb7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f1cb7-106">Attributes and elements</span></span>

<span data-ttu-id="f1cb7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1cb7-108">属性</span><span class="sxs-lookup"><span data-stu-id="f1cb7-108">Attributes</span></span>

<span data-ttu-id="f1cb7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1cb7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f1cb7-110">Child elements</span></span>

<span data-ttu-id="f1cb7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1cb7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f1cb7-112">Parent elements</span></span>

|<span data-ttu-id="f1cb7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f1cb7-113">**Element**</span></span>|<span data-ttu-id="f1cb7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f1cb7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1cb7-115">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="f1cb7-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="f1cb7-116">[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)で返される 1 つのメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f1cb7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f1cb7-117">Text value</span></span>

<span data-ttu-id="f1cb7-118">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1cb7-119">備考</span><span class="sxs-lookup"><span data-stu-id="f1cb7-119">Remarks</span></span>

<span data-ttu-id="f1cb7-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f1cb7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1cb7-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="f1cb7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1cb7-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="f1cb7-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1cb7-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f1cb7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f1cb7-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f1cb7-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1cb7-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f1cb7-125">Validation File</span></span>  <br/> |<span data-ttu-id="f1cb7-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1cb7-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1cb7-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f1cb7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1cb7-128">False</span><span class="sxs-lookup"><span data-stu-id="f1cb7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1cb7-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f1cb7-129">See also</span></span>



[<span data-ttu-id="f1cb7-130">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="f1cb7-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="f1cb7-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f1cb7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

