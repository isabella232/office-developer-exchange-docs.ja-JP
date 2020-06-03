---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: AddressBook 要素には、MAPI/HTTP プロトコルを使用してアドレス帳サーバーにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463637"
---
# <a name="addressbook-pox"></a><span data-ttu-id="81670-103">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-103">AddressBook (POX)</span></span>

<span data-ttu-id="81670-104">**AddressBook**要素には、MAPI/HTTP プロトコルを使用してアドレス帳サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81670-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="81670-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="81670-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="81670-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="81670-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="81670-109">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="81670-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="81670-110">Attributes and elements</span></span>

<span data-ttu-id="81670-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="81670-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81670-112">属性</span><span class="sxs-lookup"><span data-stu-id="81670-112">Attributes</span></span>

<span data-ttu-id="81670-113">なし。</span><span class="sxs-lookup"><span data-stu-id="81670-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81670-114">子要素</span><span class="sxs-lookup"><span data-stu-id="81670-114">Child elements</span></span>

|<span data-ttu-id="81670-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="81670-115">**Element**</span></span>|<span data-ttu-id="81670-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="81670-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81670-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="81670-118">MAPI/HTTP プロトコルを使用して、組織のネットワークの外部からアドレス帳にアクセスするために使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81670-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="81670-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="81670-120">MAPI/HTTP プロトコルを使用して、組織のネットワーク内からアドレス帳にアクセスするために使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81670-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81670-121">親要素</span><span class="sxs-lookup"><span data-stu-id="81670-121">Parent elements</span></span>

|<span data-ttu-id="81670-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="81670-122">**Element**</span></span>|<span data-ttu-id="81670-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="81670-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81670-124">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="81670-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="81670-125">クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="81670-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81670-126">注釈</span><span class="sxs-lookup"><span data-stu-id="81670-126">Remarks</span></span>

<span data-ttu-id="81670-127">**AddressBook**要素は、 **Type**属性の値が "Http" である[Protocol (POX)](protocol-pox.md)要素を持つ応答に存在します。</span><span class="sxs-lookup"><span data-stu-id="81670-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="81670-128">**AddressBook**要素は、MAPI/HTTP プロトコルおよびターゲット exchange online の一部としての exchange Online、Office 365 の一部としての exchange online、およびビルド 15.00.0847.032 (exchange SERVER 2013 SP1) 以降のオンプレミスバージョンの exchange を実装するクライアントで使用できます。</span><span class="sxs-lookup"><span data-stu-id="81670-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="81670-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="81670-129">See also</span></span>

- [<span data-ttu-id="81670-130">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="81670-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

