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
description: SendNotificationResult 要素には、push 通知に対するクライアント アプリケーションの応答が含まれています。
ms.openlocfilehash: 9acaa396430cf4e06a9c996834874d19dcab50ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833350"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="1a3dd-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="1a3dd-103">SendNotificationResult</span></span>

<span data-ttu-id="1a3dd-104">**SendNotificationResult**要素には、push 通知に対するクライアント アプリケーションの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="1a3dd-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="1a3dd-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a3dd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1a3dd-106">Attributes and elements</span></span>

<span data-ttu-id="1a3dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a3dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a3dd-108">Attributes</span></span>

<span data-ttu-id="1a3dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a3dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1a3dd-110">Child elements</span></span>

|<span data-ttu-id="1a3dd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1a3dd-111">**Element**</span></span>|<span data-ttu-id="1a3dd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1a3dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a3dd-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="1a3dd-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="1a3dd-114">プッシュ サブスクリプションの状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a3dd-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1a3dd-115">Parent elements</span></span>

<span data-ttu-id="1a3dd-116">なし。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a3dd-117">備考</span><span class="sxs-lookup"><span data-stu-id="1a3dd-117">Remarks</span></span>

<span data-ttu-id="1a3dd-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="1a3dd-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a3dd-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="1a3dd-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a3dd-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="1a3dd-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a3dd-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1a3dd-121">Schema Name</span></span>  <br/> |<span data-ttu-id="1a3dd-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1a3dd-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a3dd-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1a3dd-123">Validation File</span></span>  <br/> |<span data-ttu-id="1a3dd-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a3dd-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a3dd-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1a3dd-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a3dd-126">False</span><span class="sxs-lookup"><span data-stu-id="1a3dd-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a3dd-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="1a3dd-127">See also</span></span>



- [<span data-ttu-id="1a3dd-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1a3dd-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

