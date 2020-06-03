---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: SMTPLast 要素は、SMTP サーバーを使用して電子メールを送信する前に、SMTP (Simple Mail Transfer Protocol) サーバーで電子メールをダウンロードする必要があるかどうかを指定します。
ms.openlocfilehash: 7019da28ffa196a9abc8798aa75aff2756198da3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468433"
---
# <a name="smtplast-pox"></a><span data-ttu-id="d26fa-103">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-103">SMTPLast (POX)</span></span>

<span data-ttu-id="d26fa-104">**SMTPLast**要素は、smtp サーバーを使用して電子メールを送信する前に、Smtp (Simple Mail Transfer Protocol) サーバーで電子メールをダウンロードする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d26fa-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="d26fa-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="d26fa-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="d26fa-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="d26fa-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="d26fa-109">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d26fa-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d26fa-110">Attributes and elements</span></span>

<span data-ttu-id="d26fa-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d26fa-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d26fa-112">属性</span><span class="sxs-lookup"><span data-stu-id="d26fa-112">Attributes</span></span>

<span data-ttu-id="d26fa-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d26fa-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d26fa-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d26fa-114">Child elements</span></span>

<span data-ttu-id="d26fa-115">なし。</span><span class="sxs-lookup"><span data-stu-id="d26fa-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d26fa-116">親要素</span><span class="sxs-lookup"><span data-stu-id="d26fa-116">Parent elements</span></span>

|<span data-ttu-id="d26fa-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="d26fa-117">**Element**</span></span>|<span data-ttu-id="d26fa-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="d26fa-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d26fa-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="d26fa-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d26fa-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d26fa-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d26fa-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d26fa-121">Text value</span></span>

<span data-ttu-id="d26fa-122">テキスト値は、smtp サーバーを使用して電子メールを送信する前に、SMTP サーバーで電子メールをダウンロードする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d26fa-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="d26fa-123">有効な値は、 **[オン**] または [**オフ**] です。</span><span class="sxs-lookup"><span data-stu-id="d26fa-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="d26fa-124">既定値は**off**です。</span><span class="sxs-lookup"><span data-stu-id="d26fa-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d26fa-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="d26fa-125">See also</span></span>

- [<span data-ttu-id="d26fa-126">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="d26fa-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

