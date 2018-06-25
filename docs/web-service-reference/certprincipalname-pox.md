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
description: CertPrincipalName 要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759618"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="335df-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="335df-104">**CertPrincipalName**要素は、SSL を使用して Microsoft Exchange Server 2007 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="335df-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="335df-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="335df-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="335df-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="335df-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="335df-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="335df-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="335df-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="335df-110">Attributes and elements</span></span>

<span data-ttu-id="335df-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="335df-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="335df-112">属性</span><span class="sxs-lookup"><span data-stu-id="335df-112">Attributes</span></span>

<span data-ttu-id="335df-113">なし。</span><span class="sxs-lookup"><span data-stu-id="335df-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="335df-114">子要素</span><span class="sxs-lookup"><span data-stu-id="335df-114">Child elements</span></span>

<span data-ttu-id="335df-115">なし。</span><span class="sxs-lookup"><span data-stu-id="335df-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="335df-116">親要素</span><span class="sxs-lookup"><span data-stu-id="335df-116">Parent elements</span></span>

|<span data-ttu-id="335df-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="335df-117">**Element**</span></span>|<span data-ttu-id="335df-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="335df-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="335df-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="335df-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="335df-120">クライアント アクセス サーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="335df-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="335df-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="335df-121">Text value</span></span>

<span data-ttu-id="335df-122">テキスト値は、SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL 証明書のプリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="335df-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="335df-123">備考</span><span class="sxs-lookup"><span data-stu-id="335df-123">Remarks</span></span>

<span data-ttu-id="335df-124">**CertPrincipalName**要素が指定されていない場合、デフォルトは msstd:SERVER に設定されてサーバーと[サーバー (POX)](server-pox.md)要素で指定されている値があります。</span><span class="sxs-lookup"><span data-stu-id="335df-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="335df-125">たとえば、example.com としてサーバーを指定すると、 **CertPrincipalName**は空白のままに[SSL (POX)](ssl-pox.md)がオンに、 **CertPrincipalName**の既定値になります msstd:example.com。</span><span class="sxs-lookup"><span data-stu-id="335df-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="335df-126">何も指定されて**いない**場合、Windows は MSDN で、[プリンシパル名](http://go.microsoft.com/fwlink/?LinkId=93417)」のトピックに含まれる情報に基づいて証明書のプリンシパル名を検証します。</span><span class="sxs-lookup"><span data-stu-id="335df-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](http://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="335df-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="335df-127">See also</span></span>



[<span data-ttu-id="335df-128">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="335df-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

