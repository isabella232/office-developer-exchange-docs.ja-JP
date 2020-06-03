---
title: Unsubscribe
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
description: 講読解除要素には、サブスクリプションのサブスクライブを解除するために使用されるプロパティが含まれています。
ms.openlocfilehash: d3d9c3bf9ad97cc0fdabf574c6505c797583838a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467215"
---
# <a name="unsubscribe"></a><span data-ttu-id="5df57-103">Unsubscribe</span><span class="sxs-lookup"><span data-stu-id="5df57-103">Unsubscribe</span></span>

<span data-ttu-id="5df57-104">**講読解除**要素には、サブスクリプションのサブスクライブを解除するために使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5df57-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="5df57-105">登録を解除する</span><span class="sxs-lookup"><span data-stu-id="5df57-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="5df57-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="5df57-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5df57-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5df57-107">Attributes and elements</span></span>

<span data-ttu-id="5df57-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5df57-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5df57-109">属性</span><span class="sxs-lookup"><span data-stu-id="5df57-109">Attributes</span></span>

<span data-ttu-id="5df57-110">なし。</span><span class="sxs-lookup"><span data-stu-id="5df57-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5df57-111">子要素</span><span class="sxs-lookup"><span data-stu-id="5df57-111">Child elements</span></span>

|<span data-ttu-id="5df57-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="5df57-112">**Element**</span></span>|<span data-ttu-id="5df57-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5df57-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5df57-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="5df57-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="5df57-115">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="5df57-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5df57-116">親要素</span><span class="sxs-lookup"><span data-stu-id="5df57-116">Parent elements</span></span>

<span data-ttu-id="5df57-117">なし。</span><span class="sxs-lookup"><span data-stu-id="5df57-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5df57-118">注釈</span><span class="sxs-lookup"><span data-stu-id="5df57-118">Remarks</span></span>

<span data-ttu-id="5df57-119">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5df57-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5df57-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5df57-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5df57-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5df57-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5df57-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5df57-122">Schema name</span></span>  <br/> |<span data-ttu-id="5df57-123">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5df57-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5df57-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5df57-124">Validation file</span></span>  <br/> |<span data-ttu-id="5df57-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5df57-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5df57-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5df57-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5df57-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="5df57-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5df57-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="5df57-128">See also</span></span>



[<span data-ttu-id="5df57-129">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="5df57-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5df57-130">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="5df57-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5df57-131">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="5df57-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

