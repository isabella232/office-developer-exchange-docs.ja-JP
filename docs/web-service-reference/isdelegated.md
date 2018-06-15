---
title: IsDelegated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: IsDelegated 要素は、会議は、代理人アクセス権限を持つアカウントによって処理されたかどうかを示します。
ms.openlocfilehash: a6f42a57b2d0fdb760e4c36d3211ba57289a3c7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832005"
---
# <a name="isdelegated"></a><span data-ttu-id="d9d06-103">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="d9d06-103">IsDelegated</span></span>

<span data-ttu-id="d9d06-104">**IsDelegated**要素は、会議は、代理人アクセス権限を持つアカウントによって処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="d9d06-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d9d06-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9d06-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d9d06-106">Attributes and elements</span></span>

<span data-ttu-id="d9d06-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9d06-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9d06-108">Attributes</span></span>

<span data-ttu-id="d9d06-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d9d06-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9d06-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d9d06-110">Child elements</span></span>

<span data-ttu-id="d9d06-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d9d06-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9d06-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d9d06-112">Parent elements</span></span>

|<span data-ttu-id="d9d06-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d9d06-113">**Element**</span></span>|<span data-ttu-id="d9d06-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d9d06-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9d06-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d9d06-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d9d06-116">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9d06-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d9d06-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d9d06-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9d06-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d9d06-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d9d06-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d9d06-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d9d06-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d9d06-122">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9d06-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d9d06-123">Text value</span></span>

<span data-ttu-id="d9d06-124">**True**の場合、テキスト値は、会議は、代理人アクセス権限を持つアカウントによって処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="d9d06-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d9d06-125">Remarks</span><span class="sxs-lookup"><span data-stu-id="d9d06-125">Remarks</span></span>

<span data-ttu-id="d9d06-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d9d06-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9d06-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="d9d06-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9d06-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="d9d06-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9d06-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d9d06-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d9d06-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d9d06-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9d06-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d9d06-131">Validation File</span></span>  <br/> |<span data-ttu-id="d9d06-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9d06-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9d06-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d9d06-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9d06-134">False</span><span class="sxs-lookup"><span data-stu-id="d9d06-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9d06-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="d9d06-135">See also</span></span>



- [<span data-ttu-id="d9d06-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d9d06-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

