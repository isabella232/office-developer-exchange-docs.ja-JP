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
description: SubscriptionStatus 要素では、プッシュ サブスクリプションの状態について説明します。
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839619"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="18eb1-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="18eb1-103">SubscriptionStatus</span></span>

<span data-ttu-id="18eb1-104">**SubscriptionStatus**要素では、プッシュ サブスクリプションの状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="18eb1-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="18eb1-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="18eb1-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="18eb1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="18eb1-106">Attributes and elements</span></span>

<span data-ttu-id="18eb1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="18eb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18eb1-108">属性</span><span class="sxs-lookup"><span data-stu-id="18eb1-108">Attributes</span></span>

<span data-ttu-id="18eb1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="18eb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18eb1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="18eb1-110">Child elements</span></span>

<span data-ttu-id="18eb1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="18eb1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="18eb1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="18eb1-112">Parent elements</span></span>

|<span data-ttu-id="18eb1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="18eb1-113">**Element**</span></span>|<span data-ttu-id="18eb1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="18eb1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18eb1-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="18eb1-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="18eb1-116">クライアント アプリケーションの応答が含まれています ' プッシュ通知をします。</span><span class="sxs-lookup"><span data-stu-id="18eb1-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="18eb1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="18eb1-117">Text value</span></span>

<span data-ttu-id="18eb1-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="18eb1-118">A text value is required.</span></span> <span data-ttu-id="18eb1-119">この要素の使用可能なテキスト値は、次のように。</span><span class="sxs-lookup"><span data-stu-id="18eb1-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="18eb1-120">OK</span><span class="sxs-lookup"><span data-stu-id="18eb1-120">OK</span></span>
    
- <span data-ttu-id="18eb1-121">登録を解除する</span><span class="sxs-lookup"><span data-stu-id="18eb1-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="18eb1-122">備考</span><span class="sxs-lookup"><span data-stu-id="18eb1-122">Remarks</span></span>

<span data-ttu-id="18eb1-123">この要素では、サブスクリプションの状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="18eb1-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="18eb1-124">プッシュ サブスクリプションのクライアント アプリケーションは、プッシュ通知の後にインストールされているクライアント アクセス サーバーの役割を Exchange 2007 を実行しているコンピューターにステータスを送信します。</span><span class="sxs-lookup"><span data-stu-id="18eb1-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="18eb1-125">**SubscriptionStatus**の値には、**購読の取り消し**が等しくなると、クライアント アクセス サーバーは通知の送信を停止し、サブスクリプションを終了します。</span><span class="sxs-lookup"><span data-stu-id="18eb1-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="18eb1-126">**SubscriptionStatus**の値には、 **[ok]** が表示、クライアント アクセス サーバーの通知を送信する続けます。</span><span class="sxs-lookup"><span data-stu-id="18eb1-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="18eb1-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="18eb1-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18eb1-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="18eb1-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18eb1-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="18eb1-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="18eb1-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="18eb1-130">Schema Name</span></span>  <br/> |<span data-ttu-id="18eb1-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="18eb1-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="18eb1-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="18eb1-132">Validation File</span></span>  <br/> |<span data-ttu-id="18eb1-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="18eb1-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18eb1-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="18eb1-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="18eb1-135">False</span><span class="sxs-lookup"><span data-stu-id="18eb1-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18eb1-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="18eb1-136">See also</span></span>



- [<span data-ttu-id="18eb1-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="18eb1-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

