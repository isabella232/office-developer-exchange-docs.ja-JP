---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: SubscriptionStatus 要素は、プッシュサブスクリプションの状態を表します。
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530945"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="e20c1-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="e20c1-103">SubscriptionStatus</span></span>

<span data-ttu-id="e20c1-104">**Subscriptionstatus**要素は、プッシュサブスクリプションの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="e20c1-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="e20c1-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e20c1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e20c1-106">Attributes and elements</span></span>

<span data-ttu-id="e20c1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e20c1-108">属性</span><span class="sxs-lookup"><span data-stu-id="e20c1-108">Attributes</span></span>

<span data-ttu-id="e20c1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e20c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e20c1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e20c1-110">Child elements</span></span>

<span data-ttu-id="e20c1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e20c1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e20c1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e20c1-112">Parent elements</span></span>

|<span data-ttu-id="e20c1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e20c1-113">**Element**</span></span>|<span data-ttu-id="e20c1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e20c1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20c1-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="e20c1-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="e20c1-116">プッシュ通知に対するクライアントアプリケーションの応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="e20c1-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e20c1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e20c1-117">Text value</span></span>

<span data-ttu-id="e20c1-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="e20c1-118">A text value is required.</span></span> <span data-ttu-id="e20c1-119">この要素に使用できるテキスト値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e20c1-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="e20c1-120">OK</span><span class="sxs-lookup"><span data-stu-id="e20c1-120">OK</span></span>
    
- <span data-ttu-id="e20c1-121">Unsubscribe</span><span class="sxs-lookup"><span data-stu-id="e20c1-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e20c1-122">注釈</span><span class="sxs-lookup"><span data-stu-id="e20c1-122">Remarks</span></span>

<span data-ttu-id="e20c1-123">この要素は、サブスクリプションの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="e20c1-124">プッシュサブスクリプションクライアントアプリケーションは、各プッシュ通知の後にクライアントアクセスサーバーの役割がインストールされている、Exchange 2007 を実行しているコンピューターにステータスを送り返します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="e20c1-125">**Subscriptionstatus**の値が**購読の取り消し**に等しい場合、クライアントアクセスサーバーは通知の送信を停止し、サブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="e20c1-126">**Subscriptionstatus**の値が**OK**の場合、クライアントアクセスサーバーは引き続き通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="e20c1-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="e20c1-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e20c1-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e20c1-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e20c1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e20c1-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="e20c1-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e20c1-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e20c1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e20c1-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e20c1-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e20c1-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e20c1-132">Validation File</span></span>  <br/> |<span data-ttu-id="e20c1-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e20c1-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e20c1-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e20c1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e20c1-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="e20c1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e20c1-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e20c1-136">See also</span></span>



- [<span data-ttu-id="e20c1-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e20c1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

