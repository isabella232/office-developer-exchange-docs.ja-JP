---
title: 外部 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: 外部の要素には、組織のネットワーク外部から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。
ms.openlocfilehash: 7f01fc29b5ce63b02de0a4a6e42887dcffbb4b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760416"
---
# <a name="external-pox"></a><span data-ttu-id="a9d36-103">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-103">External (POX)</span></span>

<span data-ttu-id="a9d36-104">**外部**の要素には、組織のネットワーク外部から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9d36-104">The **External** element contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span> 
  
[<span data-ttu-id="a9d36-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="a9d36-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a9d36-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a9d36-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a9d36-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a9d36-109">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-109">External (POX)</span></span>](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="a9d36-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a9d36-110">Attributes and elements</span></span>

<span data-ttu-id="a9d36-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a9d36-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9d36-112">属性</span><span class="sxs-lookup"><span data-stu-id="a9d36-112">Attributes</span></span>

<span data-ttu-id="a9d36-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a9d36-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9d36-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a9d36-114">Child elements</span></span>

|<span data-ttu-id="a9d36-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9d36-115">**Element**</span></span>|<span data-ttu-id="a9d36-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9d36-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9d36-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="a9d36-118">URL を説明し、Microsoft Exchange Server を実行している特定のコンピューターへのアクセスに使用する認証スキーマには、クライアント アクセス サーバーの役割がインストールされている Outlook Web Access をホストしています。</span><span class="sxs-lookup"><span data-stu-id="a9d36-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="a9d36-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a9d36-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9d36-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="a9d36-121">この**プロトコル**要素には 2 つの子要素:[種類 (POX)](type-pox.md)要素の接続プロトコルを指定して、 [ASUrl (POX)](asurl-pox.md) 、可用性 web サービスの EWS のエンドポイントを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d36-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9d36-122">親要素</span><span class="sxs-lookup"><span data-stu-id="a9d36-122">Parent elements</span></span>

|<span data-ttu-id="a9d36-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9d36-123">**Element**</span></span>|<span data-ttu-id="a9d36-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9d36-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9d36-125">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a9d36-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a9d36-126">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9d36-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a9d36-127">備考</span><span class="sxs-lookup"><span data-stu-id="a9d36-127">Remarks</span></span>

<span data-ttu-id="a9d36-128">**外部**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="a9d36-128">The **External** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a9d36-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9d36-129">See also</span></span>



[<span data-ttu-id="a9d36-130">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a9d36-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

