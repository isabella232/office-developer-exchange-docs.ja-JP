---
title: ErrorSubscriptionIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrorSubscriptionIds
api_type:
- schema
ms.assetid: e64e76ff-4d98-4082-9acc-a1114ae45f44
description: ErrorSubscriptionIds 要素には、無効なサブスクリプション Id の配列が含まれています。
ms.openlocfilehash: 5cdbbeb1083754510f431bc092bb67dc0addecab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760334"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="f7304-103">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="f7304-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="f7304-104">**ErrorSubscriptionIds**要素には、無効なサブスクリプション Id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f7304-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="f7304-105">**NonEmptyArrayOfSubscriptionIdsType**</span><span class="sxs-lookup"><span data-stu-id="f7304-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7304-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f7304-106">Attributes and elements</span></span>

<span data-ttu-id="f7304-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f7304-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7304-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7304-108">Attributes</span></span>

<span data-ttu-id="f7304-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f7304-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7304-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f7304-110">Child elements</span></span>

|<span data-ttu-id="f7304-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f7304-111">**Element**</span></span>|<span data-ttu-id="f7304-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7304-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7304-113">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="f7304-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="f7304-114">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="f7304-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7304-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f7304-115">Parent elements</span></span>

|<span data-ttu-id="f7304-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="f7304-116">**Element**</span></span>|<span data-ttu-id="f7304-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="f7304-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7304-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f7304-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="f7304-119">状態および 1 つの結果が含まれています[GetStreamingEvents の操作](getstreamingevents-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="f7304-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7304-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f7304-120">Text value</span></span>

<span data-ttu-id="f7304-121">なし。</span><span class="sxs-lookup"><span data-stu-id="f7304-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f7304-122">備考</span><span class="sxs-lookup"><span data-stu-id="f7304-122">Remarks</span></span>

<span data-ttu-id="f7304-123">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f7304-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7304-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="f7304-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7304-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="f7304-125">Namespace</span></span>  <br/> |<span data-ttu-id="f7304-126">http://schemas.microsoft.com/exchange/services/2006/messages と http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="f7304-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="f7304-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f7304-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f7304-128">メッセージ スキーマです。タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="f7304-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="f7304-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f7304-129">Validation File</span></span>  <br/> |<span data-ttu-id="f7304-130">Messages.xsd です。Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7304-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7304-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f7304-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7304-132">False</span><span class="sxs-lookup"><span data-stu-id="f7304-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7304-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="f7304-133">See also</span></span>



[<span data-ttu-id="f7304-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="f7304-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="f7304-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f7304-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

