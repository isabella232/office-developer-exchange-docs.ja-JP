---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: DirectoryPort 要素は、ネーム サービス プロバイダー インターフェイス (NSPI) プロトコルを使用すると、ディレクトリへの接続に使用されるポートを指定します。
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760051"
---
# <a name="directoryport-pox"></a><span data-ttu-id="a9bba-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="a9bba-104">**DirectoryPort**要素は、ネーム サービス プロバイダー インターフェイス (NSPI) プロトコルを使用すると、ディレクトリへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="a9bba-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="a9bba-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="a9bba-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="a9bba-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="a9bba-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="a9bba-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="a9bba-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a9bba-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a9bba-110">Attributes and elements</span></span>

<span data-ttu-id="a9bba-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a9bba-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9bba-112">属性</span><span class="sxs-lookup"><span data-stu-id="a9bba-112">Attributes</span></span>

<span data-ttu-id="a9bba-113">なし。</span><span class="sxs-lookup"><span data-stu-id="a9bba-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9bba-114">子要素</span><span class="sxs-lookup"><span data-stu-id="a9bba-114">Child elements</span></span>

<span data-ttu-id="a9bba-115">なし。</span><span class="sxs-lookup"><span data-stu-id="a9bba-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9bba-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a9bba-116">Parent elements</span></span>

|<span data-ttu-id="a9bba-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="a9bba-117">**Element**</span></span>|<span data-ttu-id="a9bba-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="a9bba-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9bba-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="a9bba-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a9bba-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9bba-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9bba-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a9bba-121">Text value</span></span>

<span data-ttu-id="a9bba-122">テキスト値は、Exchange サーバーへのアクセスに使用するポートを表します。</span><span class="sxs-lookup"><span data-stu-id="a9bba-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a9bba-123">備考</span><span class="sxs-lookup"><span data-stu-id="a9bba-123">Remarks</span></span>

<span data-ttu-id="a9bba-124">**DirectoryPort**要素は、EXCH または EXPR[型 (POX)](type-pox.md)の要素が等しい場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="a9bba-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a9bba-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="a9bba-125">See also</span></span>

- [<span data-ttu-id="a9bba-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a9bba-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

