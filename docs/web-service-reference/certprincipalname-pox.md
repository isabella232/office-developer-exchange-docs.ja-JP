---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: CertPrincipalName 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な SSL (Secure Sockets Layer) 証明書プリンシパル名を指定します。
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463343"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="df166-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="df166-104">**CertPrincipalName**要素は、ssl を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Ssl (Secure Sockets layer) 証明書プリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="df166-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="df166-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="df166-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="df166-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="df166-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="df166-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="df166-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="df166-110">Attributes and elements</span></span>

<span data-ttu-id="df166-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df166-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df166-112">属性</span><span class="sxs-lookup"><span data-stu-id="df166-112">Attributes</span></span>

<span data-ttu-id="df166-113">なし。</span><span class="sxs-lookup"><span data-stu-id="df166-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df166-114">子要素</span><span class="sxs-lookup"><span data-stu-id="df166-114">Child elements</span></span>

<span data-ttu-id="df166-115">なし。</span><span class="sxs-lookup"><span data-stu-id="df166-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df166-116">親要素</span><span class="sxs-lookup"><span data-stu-id="df166-116">Parent elements</span></span>

|<span data-ttu-id="df166-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="df166-117">**Element**</span></span>|<span data-ttu-id="df166-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="df166-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df166-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="df166-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="df166-120">クライアントアクセスサーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="df166-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df166-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="df166-121">Text value</span></span>

<span data-ttu-id="df166-122">テキスト値は、SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL 証明書のプリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="df166-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df166-123">注釈</span><span class="sxs-lookup"><span data-stu-id="df166-123">Remarks</span></span>

<span data-ttu-id="df166-124">**CertPrincipalName**要素が指定されていない場合、既定で msstd: server が設定されます。ここで、Server は[server (POX)](server-pox.md)要素で指定された値です。</span><span class="sxs-lookup"><span data-stu-id="df166-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="df166-125">たとえば、SERVER が example.com として指定されていて、 [SSL (POX)](ssl-pox.md)が有効になっている場合、 **CertPrincipalName**を空白のままにすると、既定値の**CertPrincipalName**は msstd: example .com になります。</span><span class="sxs-lookup"><span data-stu-id="df166-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="df166-126">**何も**指定されていない場合、WINDOWS は MSDN の[プリンシパル名](https://go.microsoft.com/fwlink/?LinkId=93417)のトピックに記載されている情報に従って、証明書のプリンシパル名を検証します。</span><span class="sxs-lookup"><span data-stu-id="df166-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](https://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="df166-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="df166-127">See also</span></span>



[<span data-ttu-id="df166-128">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="df166-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

