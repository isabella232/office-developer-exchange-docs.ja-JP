---
title: EcpUrl sms (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: f5e5e589-ee16-42a8-9cd4-ae3909fc869b
description: EcpUrl sms 要素では、メールが有効なユーザーのショート メッセージ サービス (SMS) の設定にアクセスするために使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 38471db7b7e046e43425b132b1716033c1c96afd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760184"
---
# <a name="ecpurl-sms-pox"></a><span data-ttu-id="0f1bc-103">EcpUrl sms (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-103">EcpUrl-sms (POX)</span></span>

<span data-ttu-id="0f1bc-104">**EcpUrl sms**要素では、メールが有効なユーザーのショート メッセージ サービス (SMS) の設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-104">The **EcpUrl-sms** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access Short Message Service (SMS) settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="0f1bc-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="0f1bc-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0f1bc-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0f1bc-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0f1bc-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0f1bc-109">EcpUrl sms (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-109">EcpUrl-sms (POX)</span></span>](ecpurl-sms-pox.md)
  
```XML
<EcpUrl-sms/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0f1bc-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0f1bc-110">Attributes and elements</span></span>

<span data-ttu-id="0f1bc-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f1bc-112">属性</span><span class="sxs-lookup"><span data-stu-id="0f1bc-112">Attributes</span></span>

<span data-ttu-id="0f1bc-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f1bc-114">子要素</span><span class="sxs-lookup"><span data-stu-id="0f1bc-114">Child elements</span></span>

<span data-ttu-id="0f1bc-115">なし。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f1bc-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0f1bc-116">Parent elements</span></span>

|<span data-ttu-id="0f1bc-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0f1bc-117">**Element**</span></span>|<span data-ttu-id="0f1bc-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0f1bc-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f1bc-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0f1bc-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0f1bc-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f1bc-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0f1bc-121">Text value</span></span>

<span data-ttu-id="0f1bc-122">テキスト値は、ユーザーの SMS の設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access SMS settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0f1bc-123">備考</span><span class="sxs-lookup"><span data-stu-id="0f1bc-123">Remarks</span></span>

<span data-ttu-id="0f1bc-124">**EcpUrl sms**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="0f1bc-124">The **EcpUrl-sms** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0f1bc-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="0f1bc-125">See also</span></span>



[<span data-ttu-id="0f1bc-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0f1bc-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

