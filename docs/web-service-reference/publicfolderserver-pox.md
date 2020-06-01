---
title: PublicFolderServer (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 37ad46ab-7817-4fdd-ad2d-26cb525cd96b
description: PublicFolderServer 要素には、ユーザーのパブリックフォルダーサーバーの完全修飾ドメイン名 (FQDN) が含まれています。
ms.openlocfilehash: 868eab83d05387f570bc033522121f25f09817c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433687"
---
# <a name="publicfolderserver-pox"></a><span data-ttu-id="0d4a1-103">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-103">PublicFolderServer (POX)</span></span>

<span data-ttu-id="0d4a1-104">**Publicfolderserver**要素には、ユーザーのパブリックフォルダーサーバーの完全修飾ドメイン名 (FQDN) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-104">The **PublicFolderServer** element contains the fully-qualified domain name (FQDN) of the public folder server for the user.</span></span> 
  
[<span data-ttu-id="0d4a1-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0d4a1-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0d4a1-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0d4a1-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0d4a1-109">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-109">PublicFolderServer (POX)</span></span>](publicfolderserver-pox.md)
  
```XML
<PublicFolderServer/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0d4a1-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0d4a1-110">Attributes and elements</span></span>

<span data-ttu-id="0d4a1-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d4a1-112">属性</span><span class="sxs-lookup"><span data-stu-id="0d4a1-112">Attributes</span></span>

<span data-ttu-id="0d4a1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d4a1-114">子要素</span><span class="sxs-lookup"><span data-stu-id="0d4a1-114">Child elements</span></span>

<span data-ttu-id="0d4a1-115">なし。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d4a1-116">親要素</span><span class="sxs-lookup"><span data-stu-id="0d4a1-116">Parent elements</span></span>

|<span data-ttu-id="0d4a1-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="0d4a1-117">**Element**</span></span>|<span data-ttu-id="0d4a1-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="0d4a1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d4a1-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="0d4a1-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0d4a1-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d4a1-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0d4a1-121">Text value</span></span>

<span data-ttu-id="0d4a1-122">Text 値は、ユーザーのパブリックフォルダーサーバーの FQDN を表します。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-122">The text value represents the FQDN of the public folder server for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d4a1-123">注釈</span><span class="sxs-lookup"><span data-stu-id="0d4a1-123">Remarks</span></span>

<span data-ttu-id="0d4a1-124">**Publicfolderserver**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="0d4a1-124">The **PublicFolderServer** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0d4a1-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="0d4a1-125">See also</span></span>



[<span data-ttu-id="0d4a1-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="0d4a1-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

