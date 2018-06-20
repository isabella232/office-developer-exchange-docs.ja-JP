---
title: 内部 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: 内部の要素には、組織のネットワーク内から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。
ms.openlocfilehash: 0dc5b679af98b52f15ef3b40181c2d97f102f373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831946"
---
# <a name="internal-pox"></a><span data-ttu-id="07e56-103">内部 (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-103">Internal (POX)</span></span>

<span data-ttu-id="07e56-104">**内部**の要素には、組織のネットワーク内から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="07e56-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="07e56-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="07e56-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="07e56-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="07e56-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="07e56-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="07e56-109">内部 (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="07e56-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="07e56-110">Attributes and elements</span></span>

<span data-ttu-id="07e56-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="07e56-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07e56-112">属性</span><span class="sxs-lookup"><span data-stu-id="07e56-112">Attributes</span></span>

<span data-ttu-id="07e56-113">なし。</span><span class="sxs-lookup"><span data-stu-id="07e56-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07e56-114">子要素</span><span class="sxs-lookup"><span data-stu-id="07e56-114">Child elements</span></span>

|<span data-ttu-id="07e56-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="07e56-115">**Element**</span></span>|<span data-ttu-id="07e56-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="07e56-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07e56-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="07e56-118">URL を説明し、Microsoft Exchange Server を実行している特定のコンピューターへのアクセスに使用する認証スキーマには、クライアント アクセス サーバーの役割がインストールされている Outlook Web Access をホストしています。</span><span class="sxs-lookup"><span data-stu-id="07e56-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="07e56-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="07e56-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07e56-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="07e56-121">この**プロトコル**要素には 2 つの子要素:[種類 (POX)](type-pox.md)要素の接続プロトコルを指定して、 [ASUrl (POX)](asurl-pox.md) 、可用性 web サービスの EWS のエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="07e56-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07e56-122">親要素</span><span class="sxs-lookup"><span data-stu-id="07e56-122">Parent elements</span></span>

|<span data-ttu-id="07e56-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="07e56-123">**Element**</span></span>|<span data-ttu-id="07e56-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="07e56-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07e56-125">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="07e56-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="07e56-126">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="07e56-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07e56-127">備考</span><span class="sxs-lookup"><span data-stu-id="07e56-127">Remarks</span></span>

<span data-ttu-id="07e56-128">**内部**の要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="07e56-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="07e56-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="07e56-129">See also</span></span>



[<span data-ttu-id="07e56-130">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="07e56-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

