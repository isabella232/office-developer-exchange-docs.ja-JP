---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: ExternalUrl 要素には、アドレス帳のサーバーまたはユーザーの組織の外部からのユーザーのメールボックスに MAPI または HTTP プロトコルを使用してクライアントを接続するための URL が含まれています。
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760454"
---
# <a name="externalurl-pox"></a><span data-ttu-id="0e50c-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="0e50c-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="0e50c-104">**ExternalUrl**要素には、アドレス帳のサーバーまたはユーザーの組織の外部からのユーザーのメールボックスに MAPI または HTTP プロトコルを使用してクライアントを接続するための URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e50c-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0e50c-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0e50c-105">Attributes and elements</span></span>

<span data-ttu-id="0e50c-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e50c-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e50c-107">属性</span><span class="sxs-lookup"><span data-stu-id="0e50c-107">Attributes</span></span>

<span data-ttu-id="0e50c-108">なし。</span><span class="sxs-lookup"><span data-stu-id="0e50c-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e50c-109">子要素</span><span class="sxs-lookup"><span data-stu-id="0e50c-109">Child elements</span></span>

<span data-ttu-id="0e50c-110">なし。</span><span class="sxs-lookup"><span data-stu-id="0e50c-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e50c-111">親要素</span><span class="sxs-lookup"><span data-stu-id="0e50c-111">Parent elements</span></span>

|<span data-ttu-id="0e50c-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e50c-112">**Element**</span></span>|<span data-ttu-id="0e50c-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e50c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e50c-114">アドレス帳 (POX)</span><span class="sxs-lookup"><span data-stu-id="0e50c-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="0e50c-115">MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e50c-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="0e50c-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="0e50c-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="0e50c-117">MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e50c-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e50c-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0e50c-118">Text value</span></span>

<span data-ttu-id="0e50c-119">テキスト値は、アドレス帳のサーバーまたはユーザーの組織の外部からのユーザーのメールボックスへのアクセスに使用できる URL を表します。</span><span class="sxs-lookup"><span data-stu-id="0e50c-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e50c-120">備考</span><span class="sxs-lookup"><span data-stu-id="0e50c-120">Remarks</span></span>

<span data-ttu-id="0e50c-121">**ExternalUrl**要素は、"mapiHttp"の**型**の属性値を持つ[プロトコル (POX)](protocol-pox.md)要素を持つ応答で使用できます。</span><span class="sxs-lookup"><span data-stu-id="0e50c-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="0e50c-122">**ExternalUrl**要素は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに使用し、設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。.</span><span class="sxs-lookup"><span data-stu-id="0e50c-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0e50c-123">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e50c-123">See also</span></span>



[<span data-ttu-id="0e50c-124">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e50c-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

