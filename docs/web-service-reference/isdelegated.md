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
description: IsDelegated 要素は、代理人アクセス権を持つアカウントによって会議が処理されたかどうかを示します。
ms.openlocfilehash: 2c62b59665431d5ea203e972a506aa90afc76601
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456445"
---
# <a name="isdelegated"></a><span data-ttu-id="0bb90-103">IsDelegated</span><span class="sxs-lookup"><span data-stu-id="0bb90-103">IsDelegated</span></span>

<span data-ttu-id="0bb90-104">**Isdelegated**要素は、代理人アクセス権を持つアカウントによって会議が処理されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="0bb90-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0bb90-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bb90-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0bb90-106">Attributes and elements</span></span>

<span data-ttu-id="0bb90-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bb90-108">属性</span><span class="sxs-lookup"><span data-stu-id="0bb90-108">Attributes</span></span>

<span data-ttu-id="0bb90-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0bb90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bb90-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0bb90-110">Child elements</span></span>

<span data-ttu-id="0bb90-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0bb90-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bb90-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0bb90-112">Parent elements</span></span>

|<span data-ttu-id="0bb90-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bb90-113">**Element**</span></span>|<span data-ttu-id="0bb90-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bb90-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bb90-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0bb90-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0bb90-116">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb90-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0bb90-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0bb90-118">Exchange ストア内の会議を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb90-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0bb90-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0bb90-120">Exchange ストア内の会議出席依頼を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0bb90-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0bb90-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0bb90-122">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bb90-123">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0bb90-123">Text value</span></span>

<span data-ttu-id="0bb90-124">テキスト値が**true の場合**は、会議が代理人アクセス権を持つアカウントによって処理されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="0bb90-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0bb90-125">注釈</span><span class="sxs-lookup"><span data-stu-id="0bb90-125">Remarks</span></span>

<span data-ttu-id="0bb90-126">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0bb90-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bb90-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0bb90-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bb90-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bb90-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bb90-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bb90-129">Schema Name</span></span>  <br/> |<span data-ttu-id="0bb90-130">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0bb90-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bb90-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bb90-131">Validation File</span></span>  <br/> |<span data-ttu-id="0bb90-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0bb90-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bb90-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0bb90-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bb90-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="0bb90-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bb90-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bb90-135">See also</span></span>



- [<span data-ttu-id="0bb90-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0bb90-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

