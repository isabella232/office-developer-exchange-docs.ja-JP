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
description: SMTPLast 要素は、簡易メール転送プロトコル (SMTP) サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833505"
---
# <a name="smtplast-pox"></a><span data-ttu-id="af08f-103">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-103">SMTPLast (POX)</span></span>

<span data-ttu-id="af08f-104">**SMTPLast**要素は、簡易メール転送プロトコル (SMTP) サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af08f-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="af08f-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="af08f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="af08f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="af08f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="af08f-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="af08f-109">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="af08f-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af08f-110">Attributes and elements</span></span>

<span data-ttu-id="af08f-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af08f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af08f-112">属性</span><span class="sxs-lookup"><span data-stu-id="af08f-112">Attributes</span></span>

<span data-ttu-id="af08f-113">なし。</span><span class="sxs-lookup"><span data-stu-id="af08f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af08f-114">子要素</span><span class="sxs-lookup"><span data-stu-id="af08f-114">Child elements</span></span>

<span data-ttu-id="af08f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="af08f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af08f-116">親要素</span><span class="sxs-lookup"><span data-stu-id="af08f-116">Parent elements</span></span>

|<span data-ttu-id="af08f-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="af08f-117">**Element**</span></span>|<span data-ttu-id="af08f-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="af08f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af08f-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="af08f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="af08f-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="af08f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af08f-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="af08f-121">Text value</span></span>

<span data-ttu-id="af08f-122">テキスト値は、SMTP サーバーに電子メールが SMTP サーバーを使用して電子メールを送信する前にダウンロードすることが必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af08f-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="af08f-123">使用可能な値は、**オン**と**オフを**します。</span><span class="sxs-lookup"><span data-stu-id="af08f-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="af08f-124">既定値では**オフ**です。</span><span class="sxs-lookup"><span data-stu-id="af08f-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="af08f-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="af08f-125">See also</span></span>

- [<span data-ttu-id="af08f-126">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="af08f-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

