---
title: アドレス帳 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: アドレス帳の要素には、MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: c30f0ee7c36de7e63157d07d003a11187d661fd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759295"
---
# <a name="addressbook-pox"></a><span data-ttu-id="b6fba-103">アドレス帳 (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-103">AddressBook (POX)</span></span>

<span data-ttu-id="b6fba-104">**アドレス帳**の要素には、MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6fba-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="b6fba-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="b6fba-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="b6fba-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="b6fba-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="b6fba-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="b6fba-109">アドレス帳 (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b6fba-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b6fba-110">Attributes and elements</span></span>

<span data-ttu-id="b6fba-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6fba-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6fba-112">属性</span><span class="sxs-lookup"><span data-stu-id="b6fba-112">Attributes</span></span>

<span data-ttu-id="b6fba-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b6fba-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b6fba-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b6fba-114">Child elements</span></span>

|<span data-ttu-id="b6fba-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6fba-115">**Element**</span></span>|<span data-ttu-id="b6fba-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6fba-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6fba-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="b6fba-118">MAPI または HTTP プロトコルを使用して組織のネットワークの外部からのアドレス帳にアクセスするために使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6fba-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="b6fba-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="b6fba-120">MAPI または HTTP プロトコルを使用して組織のネットワーク内からアドレス帳にアクセスに使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6fba-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6fba-121">親要素</span><span class="sxs-lookup"><span data-stu-id="b6fba-121">Parent elements</span></span>

|<span data-ttu-id="b6fba-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6fba-122">**Element**</span></span>|<span data-ttu-id="b6fba-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6fba-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6fba-124">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b6fba-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b6fba-125">クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b6fba-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6fba-126">備考</span><span class="sxs-lookup"><span data-stu-id="b6fba-126">Remarks</span></span>

<span data-ttu-id="b6fba-127">**アドレス帳**要素は、"mapiHttp"の**型**の属性値を持つ[プロトコル (POX)](protocol-pox.md)要素を持つ応答であります。</span><span class="sxs-lookup"><span data-stu-id="b6fba-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="b6fba-128">ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに**アドレス帳**の要素があるし、設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。.</span><span class="sxs-lookup"><span data-stu-id="b6fba-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b6fba-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6fba-129">See also</span></span>

- [<span data-ttu-id="b6fba-130">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b6fba-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

