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
ms.openlocfilehash: bdc5c86560800464d677a9043607bed3f7872e32
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526187"
---
# <a name="errorsubscriptionids"></a><span data-ttu-id="6425e-103">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="6425e-103">ErrorSubscriptionIds</span></span>

<span data-ttu-id="6425e-104">**Errorsubscriptionids**要素には、無効なサブスクリプション id の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6425e-104">The **ErrorSubscriptionIds** element contains an array of invalid subscription IDs.</span></span> 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 <span data-ttu-id="6425e-105">**非 Emptyarrayofsubscriptionidstype**</span><span class="sxs-lookup"><span data-stu-id="6425e-105">**NonEmptyArrayOfSubscriptionIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6425e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6425e-106">Attributes and elements</span></span>

<span data-ttu-id="6425e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6425e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6425e-108">属性</span><span class="sxs-lookup"><span data-stu-id="6425e-108">Attributes</span></span>

<span data-ttu-id="6425e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6425e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6425e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6425e-110">Child elements</span></span>

|<span data-ttu-id="6425e-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6425e-111">**Element**</span></span>|<span data-ttu-id="6425e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6425e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6425e-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="6425e-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="6425e-114">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="6425e-114">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6425e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6425e-115">Parent elements</span></span>

|<span data-ttu-id="6425e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6425e-116">**Element**</span></span>|<span data-ttu-id="6425e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6425e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6425e-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6425e-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="6425e-119">1つの[Getstreamingevents 操作](getstreamingevents-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="6425e-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6425e-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6425e-120">Text value</span></span>

<span data-ttu-id="6425e-121">なし。</span><span class="sxs-lookup"><span data-stu-id="6425e-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6425e-122">注釈</span><span class="sxs-lookup"><span data-stu-id="6425e-122">Remarks</span></span>

<span data-ttu-id="6425e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6425e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6425e-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6425e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6425e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6425e-125">Namespace</span></span>  <br/> |<span data-ttu-id="6425e-126">https://schemas.microsoft.com/exchange/services/2006/messages と https://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="6425e-126">https://schemas.microsoft.com/exchange/services/2006/messages and https://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="6425e-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6425e-127">Schema Name</span></span>  <br/> |<span data-ttu-id="6425e-128">メッセージスキーマ。Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6425e-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="6425e-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6425e-129">Validation File</span></span>  <br/> |<span data-ttu-id="6425e-130">メッセージ .xsd。型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6425e-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6425e-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6425e-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="6425e-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="6425e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6425e-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="6425e-133">See also</span></span>



[<span data-ttu-id="6425e-134">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="6425e-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="6425e-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6425e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

