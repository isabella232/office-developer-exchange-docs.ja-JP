---
title: SendNotificationResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResult
api_type:
- schema
ms.assetid: fa9d6202-fa66-4f10-9858-53f4f1ce14bc
description: SendNotificationResult 要素には、プッシュ通知へのクライアントアプリケーションの応答が含まれています。
ms.openlocfilehash: 4ee9a0dda3d887f8fbfa2c2b34a9a077e7af37ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464890"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="5226b-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="5226b-103">SendNotificationResult</span></span>

<span data-ttu-id="5226b-104">**Sendnotificationresult**要素には、プッシュ通知へのクライアントアプリケーションの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5226b-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="5226b-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="5226b-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5226b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5226b-106">Attributes and elements</span></span>

<span data-ttu-id="5226b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5226b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5226b-108">属性</span><span class="sxs-lookup"><span data-stu-id="5226b-108">Attributes</span></span>

<span data-ttu-id="5226b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5226b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5226b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5226b-110">Child elements</span></span>

|<span data-ttu-id="5226b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5226b-111">**Element**</span></span>|<span data-ttu-id="5226b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5226b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5226b-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="5226b-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="5226b-114">プッシュサブスクリプションの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5226b-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5226b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5226b-115">Parent elements</span></span>

<span data-ttu-id="5226b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="5226b-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5226b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="5226b-117">Remarks</span></span>

<span data-ttu-id="5226b-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5226b-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5226b-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5226b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5226b-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="5226b-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5226b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5226b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="5226b-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5226b-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5226b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5226b-123">Validation File</span></span>  <br/> |<span data-ttu-id="5226b-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5226b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5226b-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5226b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="5226b-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="5226b-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5226b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="5226b-127">See also</span></span>



- [<span data-ttu-id="5226b-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5226b-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

