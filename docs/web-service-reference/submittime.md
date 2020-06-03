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
description: SubmitTime 要素は、メッセージがサーバーに送信された時刻を表します。
ms.openlocfilehash: e4409d962988ee308e0c0b461f9448ef68067fe8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467054"
---
# <a name="submittime"></a><span data-ttu-id="780dc-103">SubmitTime</span><span class="sxs-lookup"><span data-stu-id="780dc-103">SubmitTime</span></span>

<span data-ttu-id="780dc-104">**Submittime**要素は、メッセージがサーバーに送信された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="780dc-104">The **SubmitTime** element represents the time at which the message was sent to the server.</span></span> 
  
```XML
<SubmitTime/>
```

 <span data-ttu-id="780dc-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="780dc-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="780dc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="780dc-106">Attributes and elements</span></span>

<span data-ttu-id="780dc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="780dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="780dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="780dc-108">Attributes</span></span>

<span data-ttu-id="780dc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="780dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="780dc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="780dc-110">Child elements</span></span>

<span data-ttu-id="780dc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="780dc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="780dc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="780dc-112">Parent elements</span></span>

|<span data-ttu-id="780dc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="780dc-113">**Element**</span></span>|<span data-ttu-id="780dc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="780dc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="780dc-115">および search-messagetrackingreport</span><span class="sxs-lookup"><span data-stu-id="780dc-115">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="780dc-116">[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。</span><span class="sxs-lookup"><span data-stu-id="780dc-116">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="780dc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="780dc-117">Text value</span></span>

<span data-ttu-id="780dc-118">この要素を使用する場合は、日付/時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="780dc-118">A text value that represents a date/time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="780dc-119">注釈</span><span class="sxs-lookup"><span data-stu-id="780dc-119">Remarks</span></span>

<span data-ttu-id="780dc-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="780dc-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="780dc-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="780dc-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="780dc-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="780dc-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="780dc-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="780dc-123">Schema Name</span></span>  <br/> |<span data-ttu-id="780dc-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="780dc-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="780dc-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="780dc-125">Validation File</span></span>  <br/> |<span data-ttu-id="780dc-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="780dc-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="780dc-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="780dc-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="780dc-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="780dc-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="780dc-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="780dc-129">See also</span></span>



[<span data-ttu-id="780dc-130">GetMessageTrackingReport 操作</span><span class="sxs-lookup"><span data-stu-id="780dc-130">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="780dc-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="780dc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

