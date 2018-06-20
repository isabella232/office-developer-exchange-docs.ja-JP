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
description: AuthPackage 要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759468"
---
# <a name="authpackage-pox"></a><span data-ttu-id="dbcc9-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-103">AuthPackage (POX)</span></span>

<span data-ttu-id="dbcc9-104">**AuthPackage**要素は、メールボックス サーバーの役割がインストールされている Exchange サーバーに対して認証するときに使用される認証スキームを指定します。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="dbcc9-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="dbcc9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="dbcc9-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="dbcc9-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="dbcc9-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="dbcc9-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="dbcc9-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dbcc9-110">Attributes and elements</span></span>

<span data-ttu-id="dbcc9-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbcc9-112">属性</span><span class="sxs-lookup"><span data-stu-id="dbcc9-112">Attributes</span></span>

<span data-ttu-id="dbcc9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbcc9-114">子要素</span><span class="sxs-lookup"><span data-stu-id="dbcc9-114">Child elements</span></span>

<span data-ttu-id="dbcc9-115">なし。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbcc9-116">親要素</span><span class="sxs-lookup"><span data-stu-id="dbcc9-116">Parent elements</span></span>

|<span data-ttu-id="dbcc9-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="dbcc9-117">**Element**</span></span>|<span data-ttu-id="dbcc9-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="dbcc9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbcc9-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="dbcc9-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="dbcc9-120">クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dbcc9-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dbcc9-121">Text value</span></span>

<span data-ttu-id="dbcc9-122">テキスト値は、メールボックス サーバーに対して認証するときに使用されている認証スキームを指定します。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="dbcc9-123">指定可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="dbcc9-124">基本的な</span><span class="sxs-lookup"><span data-stu-id="dbcc9-124">basic</span></span>
- <span data-ttu-id="dbcc9-125">kerb</span><span class="sxs-lookup"><span data-stu-id="dbcc9-125">kerb</span></span>
- <span data-ttu-id="dbcc9-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="dbcc9-126">kerbntlm</span></span>
- <span data-ttu-id="dbcc9-127">ntlm</span><span class="sxs-lookup"><span data-stu-id="dbcc9-127">ntlm</span></span>
- <span data-ttu-id="dbcc9-128">証明書</span><span class="sxs-lookup"><span data-stu-id="dbcc9-128">certificate</span></span>
- <span data-ttu-id="dbcc9-129">交渉</span><span class="sxs-lookup"><span data-stu-id="dbcc9-129">negotiate</span></span>
- <span data-ttu-id="dbcc9-130">nego2</span><span class="sxs-lookup"><span data-stu-id="dbcc9-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="dbcc9-131">備考</span><span class="sxs-lookup"><span data-stu-id="dbcc9-131">Remarks</span></span>

<span data-ttu-id="dbcc9-132">**AuthPackage**要素は、[型 (POX)](type-pox.md)要素に EXCH または EXPR のテキスト値が設定されている場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="dbcc9-133">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="dbcc9-133">Version differences</span></span>

<span data-ttu-id="dbcc9-134">Office 365、Exchange Online では、および設置型バージョンの Exchange から始まる値をビルド 15.00.0995.014 の戻り値「交渉」のネゴシエート認証を使用するサーバーが構成されているクライアントには、 [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md)ヘッダーが含まれて 場合にのみです"Negotiate"が含まれています。</span><span class="sxs-lookup"><span data-stu-id="dbcc9-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dbcc9-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="dbcc9-135">See also</span></span>

- [<span data-ttu-id="dbcc9-136">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dbcc9-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

