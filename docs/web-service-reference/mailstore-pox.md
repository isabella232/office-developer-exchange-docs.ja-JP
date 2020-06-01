---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: MailStore 要素には、MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。
ms.openlocfilehash: 635228fcfeb3ad791c845050b82666a6e060b229
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459792"
---
# <a name="mailstore-pox"></a><span data-ttu-id="bfd99-103">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-103">MailStore (POX)</span></span>

<span data-ttu-id="bfd99-104">**Mailstore**要素には、MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfd99-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="bfd99-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="bfd99-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="bfd99-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="bfd99-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="bfd99-109">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="bfd99-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bfd99-110">Attributes and elements</span></span>

<span data-ttu-id="bfd99-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bfd99-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfd99-112">属性</span><span class="sxs-lookup"><span data-stu-id="bfd99-112">Attributes</span></span>

<span data-ttu-id="bfd99-113">なし。</span><span class="sxs-lookup"><span data-stu-id="bfd99-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfd99-114">子要素</span><span class="sxs-lookup"><span data-stu-id="bfd99-114">Child elements</span></span>

|<span data-ttu-id="bfd99-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="bfd99-115">**Element**</span></span>|<span data-ttu-id="bfd99-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="bfd99-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfd99-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="bfd99-118">MAPI/HTTP プロトコルを使用して、組織のネットワークの外部からユーザーのメールボックスにアクセスするために使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfd99-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="bfd99-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="bfd99-120">MAPI/HTTP プロトコルを使用して、組織のネットワーク内からユーザーのメールボックスにアクセスするために使用する URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfd99-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfd99-121">親要素</span><span class="sxs-lookup"><span data-stu-id="bfd99-121">Parent elements</span></span>

|<span data-ttu-id="bfd99-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="bfd99-122">**Element**</span></span>|<span data-ttu-id="bfd99-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="bfd99-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfd99-124">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="bfd99-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="bfd99-125">クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfd99-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bfd99-126">注釈</span><span class="sxs-lookup"><span data-stu-id="bfd99-126">Remarks</span></span>

<span data-ttu-id="bfd99-127">**Mailstore**要素は、 **Type**属性の値が "Http" である[Protocol (POX)](protocol-pox.md)要素を持つ応答に存在します。</span><span class="sxs-lookup"><span data-stu-id="bfd99-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="bfd99-128">**Mailstore**要素は、MAPI/HTTP プロトコルおよびターゲット exchange online の一部としての exchange Online、Office 365 の一部としての exchange online、および build 15.00.0847.032 (exchange SERVER 2013 SP1) 以降のオンプレミスバージョンの exchange を実装するクライアントで使用できます。</span><span class="sxs-lookup"><span data-stu-id="bfd99-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bfd99-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="bfd99-129">See also</span></span>



[<span data-ttu-id="bfd99-130">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="bfd99-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

