---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: ConnectionFailureCause 要素は、電話の呼び出しからの切断の理由を指定します。
ms.openlocfilehash: 54b4f5b89efdb42ef82dbef8f1af14a39c0ccc6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759658"
---
# <a name="connectionfailurecause"></a><span data-ttu-id="3b66e-103">ConnectionFailureCause</span><span class="sxs-lookup"><span data-stu-id="3b66e-103">ConnectionFailureCause</span></span>

<span data-ttu-id="3b66e-104">**ConnectionFailureCause**要素は、電話の呼び出しからの切断の理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="3b66e-104">The **ConnectionFailureCause** element specifies the reason for a disconnection from a telephone call.</span></span> 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 <span data-ttu-id="3b66e-105">**ConnectionFailureCauseType**</span><span class="sxs-lookup"><span data-stu-id="3b66e-105">**ConnectionFailureCauseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b66e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3b66e-106">Attributes and elements</span></span>

<span data-ttu-id="3b66e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3b66e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b66e-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b66e-108">Attributes</span></span>

<span data-ttu-id="3b66e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3b66e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b66e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3b66e-110">Child elements</span></span>

<span data-ttu-id="3b66e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3b66e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b66e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3b66e-112">Parent elements</span></span>

|<span data-ttu-id="3b66e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3b66e-113">**Element**</span></span>|<span data-ttu-id="3b66e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b66e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b66e-115">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="3b66e-115">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="3b66e-116">電話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="3b66e-116">Specifies the state information for a telephone call.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b66e-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3b66e-117">Text value</span></span>

<span data-ttu-id="3b66e-118">次の表は、 **ConnectionFailureCause**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="3b66e-118">The following table lists the possible values for the **ConnectionFailureCause** element.</span></span> 
  
<span data-ttu-id="3b66e-119">**ConnectionFailureCause 要素の値**</span><span class="sxs-lookup"><span data-stu-id="3b66e-119">**ConnectionFailureCause element values**</span></span>

|<span data-ttu-id="3b66e-120">**値**</span><span class="sxs-lookup"><span data-stu-id="3b66e-120">**Value**</span></span>|<span data-ttu-id="3b66e-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b66e-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3b66e-122">なし</span><span class="sxs-lookup"><span data-stu-id="3b66e-122">None</span></span>  <br/> |<span data-ttu-id="3b66e-123">呼び出しの状態が切り離されていないか、切断の理由が不明です。</span><span class="sxs-lookup"><span data-stu-id="3b66e-123">Call state is not disconnected or the disconnect reason is not known.</span></span>  <br/> |
|<span data-ttu-id="3b66e-124">UserBusy</span><span class="sxs-lookup"><span data-stu-id="3b66e-124">UserBusy</span></span>  <br/> |<span data-ttu-id="3b66e-125">呼ばれるパーティの回線がビジー状態でした。</span><span class="sxs-lookup"><span data-stu-id="3b66e-125">The called party line was busy.</span></span>  <br/> |
|<span data-ttu-id="3b66e-126">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="3b66e-126">NoAnswer</span></span>  <br/> |<span data-ttu-id="3b66e-127">呼に応答しませんでした。</span><span class="sxs-lookup"><span data-stu-id="3b66e-127">The called party did not answer.</span></span>  <br/> |
|<span data-ttu-id="3b66e-128">使用できない</span><span class="sxs-lookup"><span data-stu-id="3b66e-128">Unavailable</span></span>  <br/> |<span data-ttu-id="3b66e-129">呼び出し先の番号は使用できませんでした。</span><span class="sxs-lookup"><span data-stu-id="3b66e-129">The called party number was not available.</span></span>  <br/> |
|<span data-ttu-id="3b66e-130">その他</span><span class="sxs-lookup"><span data-stu-id="3b66e-130">Other</span></span>  <br/> |<span data-ttu-id="3b66e-131">切断の理由には、キャッチ オール。</span><span class="sxs-lookup"><span data-stu-id="3b66e-131">Catch-all for other disconnect reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b66e-132">備考</span><span class="sxs-lookup"><span data-stu-id="3b66e-132">Remarks</span></span>

<span data-ttu-id="3b66e-133">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3b66e-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b66e-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="3b66e-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b66e-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="3b66e-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b66e-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3b66e-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3b66e-137">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3b66e-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b66e-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3b66e-138">Validation File</span></span>  <br/> |<span data-ttu-id="3b66e-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b66e-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b66e-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3b66e-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b66e-141">False</span><span class="sxs-lookup"><span data-stu-id="3b66e-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b66e-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b66e-142">See also</span></span>



- [<span data-ttu-id="3b66e-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3b66e-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

