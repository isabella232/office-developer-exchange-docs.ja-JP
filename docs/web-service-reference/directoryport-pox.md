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
description: DirectoryPort 要素は、ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用されるポートを指定します。
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462088"
---
# <a name="directoryport-pox"></a><span data-ttu-id="1207f-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="1207f-104">**Directoryport**要素は、ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="1207f-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="1207f-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="1207f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="1207f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="1207f-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="1207f-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1207f-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1207f-110">Attributes and elements</span></span>

<span data-ttu-id="1207f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1207f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1207f-112">属性</span><span class="sxs-lookup"><span data-stu-id="1207f-112">Attributes</span></span>

<span data-ttu-id="1207f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="1207f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1207f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="1207f-114">Child elements</span></span>

<span data-ttu-id="1207f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="1207f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1207f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="1207f-116">Parent elements</span></span>

|<span data-ttu-id="1207f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="1207f-117">**Element**</span></span>|<span data-ttu-id="1207f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="1207f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1207f-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="1207f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1207f-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1207f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1207f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1207f-121">Text value</span></span>

<span data-ttu-id="1207f-122">Text 値は、Exchange サーバーへのアクセスに使用されるポートを表します。</span><span class="sxs-lookup"><span data-stu-id="1207f-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1207f-123">注釈</span><span class="sxs-lookup"><span data-stu-id="1207f-123">Remarks</span></span>

<span data-ttu-id="1207f-124">**Directoryport**要素は、 [Type (POX)](type-pox.md)要素が EXCH または EXPR と等しい場合にのみ使用されます。</span><span class="sxs-lookup"><span data-stu-id="1207f-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1207f-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="1207f-125">See also</span></span>

- [<span data-ttu-id="1207f-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="1207f-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

