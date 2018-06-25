---
title: 登録を解除する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 5584db5f-553a-47ce-85fb-f9902c9990ab
description: 購読取り消しの要素には、サブスクリプションの購読を解除するためのプロパティが含まれています。
ms.openlocfilehash: bab797ff74a921e3e93c993229bc6d6d289e0c5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839819"
---
# <a name="unsubscribe"></a><span data-ttu-id="21fa3-103">登録を解除する</span><span class="sxs-lookup"><span data-stu-id="21fa3-103">Unsubscribe</span></span>

<span data-ttu-id="21fa3-104">**購読取り消し**の要素には、サブスクリプションの購読を解除するためのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="21fa3-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="21fa3-105">購読の取り消し</span><span class="sxs-lookup"><span data-stu-id="21fa3-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="21fa3-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="21fa3-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21fa3-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="21fa3-107">Attributes and elements</span></span>

<span data-ttu-id="21fa3-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21fa3-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21fa3-109">属性</span><span class="sxs-lookup"><span data-stu-id="21fa3-109">Attributes</span></span>

<span data-ttu-id="21fa3-110">なし。</span><span class="sxs-lookup"><span data-stu-id="21fa3-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21fa3-111">子要素</span><span class="sxs-lookup"><span data-stu-id="21fa3-111">Child elements</span></span>

|<span data-ttu-id="21fa3-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="21fa3-112">**Element**</span></span>|<span data-ttu-id="21fa3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="21fa3-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21fa3-114">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="21fa3-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="21fa3-115">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="21fa3-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21fa3-116">親要素</span><span class="sxs-lookup"><span data-stu-id="21fa3-116">Parent elements</span></span>

<span data-ttu-id="21fa3-117">なし。</span><span class="sxs-lookup"><span data-stu-id="21fa3-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21fa3-118">備考</span><span class="sxs-lookup"><span data-stu-id="21fa3-118">Remarks</span></span>

<span data-ttu-id="21fa3-119">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="21fa3-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21fa3-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="21fa3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21fa3-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="21fa3-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21fa3-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21fa3-122">Schema name</span></span>  <br/> |<span data-ttu-id="21fa3-123">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="21fa3-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21fa3-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21fa3-124">Validation file</span></span>  <br/> |<span data-ttu-id="21fa3-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="21fa3-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21fa3-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="21fa3-126">Can be empty</span></span>  <br/> |<span data-ttu-id="21fa3-127">False</span><span class="sxs-lookup"><span data-stu-id="21fa3-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21fa3-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="21fa3-128">See also</span></span>



[<span data-ttu-id="21fa3-129">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="21fa3-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="21fa3-130">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="21fa3-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="21fa3-131">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="21fa3-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

