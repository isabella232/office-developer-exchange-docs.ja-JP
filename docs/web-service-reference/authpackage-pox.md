---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: AuthPackage 要素は、メールボックスサーバーの役割がインストールされている Exchange サーバーに対する認証時に使用される認証方式を指定します。
ms.openlocfilehash: 5317cf49d354a558417829e1d1b5b67cd6874309
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459105"
---
# <a name="authpackage-pox"></a><span data-ttu-id="fa7f8-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-103">AuthPackage (POX)</span></span>

<span data-ttu-id="fa7f8-104">**Authpackage**要素は、メールボックスサーバーの役割がインストールされている Exchange サーバーに対する認証時に使用される認証方式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="fa7f8-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="fa7f8-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="fa7f8-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="fa7f8-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="fa7f8-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="fa7f8-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fa7f8-110">Attributes and elements</span></span>

<span data-ttu-id="fa7f8-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa7f8-112">属性</span><span class="sxs-lookup"><span data-stu-id="fa7f8-112">Attributes</span></span>

<span data-ttu-id="fa7f8-113">なし。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa7f8-114">子要素</span><span class="sxs-lookup"><span data-stu-id="fa7f8-114">Child elements</span></span>

<span data-ttu-id="fa7f8-115">なし。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa7f8-116">親要素</span><span class="sxs-lookup"><span data-stu-id="fa7f8-116">Parent elements</span></span>

|<span data-ttu-id="fa7f8-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa7f8-117">**Element**</span></span>|<span data-ttu-id="fa7f8-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa7f8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa7f8-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="fa7f8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="fa7f8-120">クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa7f8-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fa7f8-121">Text value</span></span>

<span data-ttu-id="fa7f8-122">テキスト値は、メールボックスサーバーに対する認証時に使用される認証スキームを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="fa7f8-123">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="fa7f8-124">基本的な</span><span class="sxs-lookup"><span data-stu-id="fa7f8-124">basic</span></span>
- <span data-ttu-id="fa7f8-125">kerb</span><span class="sxs-lookup"><span data-stu-id="fa7f8-125">kerb</span></span>
- <span data-ttu-id="fa7f8-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="fa7f8-126">kerbntlm</span></span>
- <span data-ttu-id="fa7f8-127">ntlm</span><span class="sxs-lookup"><span data-stu-id="fa7f8-127">ntlm</span></span>
- <span data-ttu-id="fa7f8-128">certificate</span><span class="sxs-lookup"><span data-stu-id="fa7f8-128">certificate</span></span>
- <span data-ttu-id="fa7f8-129">取り決め</span><span class="sxs-lookup"><span data-stu-id="fa7f8-129">negotiate</span></span>
- <span data-ttu-id="fa7f8-130">nego2</span><span class="sxs-lookup"><span data-stu-id="fa7f8-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fa7f8-131">注釈</span><span class="sxs-lookup"><span data-stu-id="fa7f8-131">Remarks</span></span>

<span data-ttu-id="fa7f8-132">**Authpackage**要素は、 [Type (POX)](type-pox.md)要素のテキスト値が EXCH または EXPR の場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="fa7f8-133">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="fa7f8-133">Version differences</span></span>

<span data-ttu-id="fa7f8-134">Office 365、Exchange Online、およびオンプレミスバージョンの Exchange では、サーバーが Negotiate 認証を使用するように構成されており、クライアントに "Negotiate" が含まれる[X ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれている場合にのみ、"negotiate" という値を返します。</span><span class="sxs-lookup"><span data-stu-id="fa7f8-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fa7f8-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa7f8-135">See also</span></span>

- [<span data-ttu-id="fa7f8-136">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa7f8-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

