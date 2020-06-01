---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: InternalUrl 要素には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれています。
ms.openlocfilehash: 9c6ba621a681ec54d88089de6b7ae1eefdebc679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465577"
---
# <a name="internalurl-pox"></a><span data-ttu-id="f3109-103">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="f3109-103">InternalUrl (POX)</span></span>

<span data-ttu-id="f3109-104">**Internalurl**要素には、MAPI/HTTP プロトコルを使用して、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにクライアントを接続するための URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3109-104">The **InternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from inside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f3109-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f3109-105">Attributes and elements</span></span>

<span data-ttu-id="f3109-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3109-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3109-107">属性</span><span class="sxs-lookup"><span data-stu-id="f3109-107">Attributes</span></span>

<span data-ttu-id="f3109-108">なし。</span><span class="sxs-lookup"><span data-stu-id="f3109-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3109-109">子要素</span><span class="sxs-lookup"><span data-stu-id="f3109-109">Child elements</span></span>

<span data-ttu-id="f3109-110">なし。</span><span class="sxs-lookup"><span data-stu-id="f3109-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3109-111">親要素</span><span class="sxs-lookup"><span data-stu-id="f3109-111">Parent elements</span></span>

|<span data-ttu-id="f3109-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3109-112">**Element**</span></span>|<span data-ttu-id="f3109-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3109-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3109-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="f3109-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="f3109-115">MAPI/HTTP プロトコルを使用して、アドレス帳サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3109-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="f3109-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="f3109-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="f3109-117">MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3109-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3109-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f3109-118">Text value</span></span>

<span data-ttu-id="f3109-119">Text 値は、ユーザーの組織内からアドレス帳サーバーまたはユーザーのメールボックスにアクセスするために使用できる URL を表します。</span><span class="sxs-lookup"><span data-stu-id="f3109-119">The text value represents a URL that can be used to access an address book server or user's mailbox from inside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3109-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f3109-120">Remarks</span></span>

<span data-ttu-id="f3109-121">**Internalurl**要素は、 **Type**属性の値が "Http" である[Protocol (POX)](protocol-pox.md)要素を持つ応答に存在できます。</span><span class="sxs-lookup"><span data-stu-id="f3109-121">The **InternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="f3109-122">**Internalurl**要素は、MAPI/HTTP プロトコルおよびターゲット exchange online の一部としての exchange Online、Office 365 の一部としての exchange online、および build 15.00.0847.032 (exchange SERVER 2013 SP1) 以降のオンプレミスバージョンの exchange を実装するクライアントで利用できます。</span><span class="sxs-lookup"><span data-stu-id="f3109-122">The **InternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f3109-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3109-123">See also</span></span>



[<span data-ttu-id="f3109-124">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="f3109-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

