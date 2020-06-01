---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: OWAUrl 要素には、Outlook Web Access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマが記述されています。
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457264"
---
# <a name="owaurl-pox"></a><span data-ttu-id="9e877-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-103">OWAUrl (POX)</span></span>

<span data-ttu-id="9e877-104">**Owaurl**要素には、Outlook Web access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマが記述されています。</span><span class="sxs-lookup"><span data-stu-id="9e877-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="9e877-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9e877-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9e877-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9e877-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9e877-109">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="9e877-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9e877-111">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9e877-111">Attributes and elements</span></span>

<span data-ttu-id="9e877-112">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e877-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e877-113">属性</span><span class="sxs-lookup"><span data-stu-id="9e877-113">Attributes</span></span>

|<span data-ttu-id="9e877-114">**属性**</span><span class="sxs-lookup"><span data-stu-id="9e877-114">**Attribute**</span></span>|<span data-ttu-id="9e877-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e877-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e877-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="9e877-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="9e877-117">Outlook Web Access にアクセスするための認証方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e877-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="9e877-118">AuthenticationMethod 属性</span><span class="sxs-lookup"><span data-stu-id="9e877-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="9e877-119">**値**</span><span class="sxs-lookup"><span data-stu-id="9e877-119">**Value**</span></span>|<span data-ttu-id="9e877-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e877-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e877-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="9e877-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="9e877-122">統合 Windows 認証。</span><span class="sxs-lookup"><span data-stu-id="9e877-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="9e877-123">FBA</span><span class="sxs-lookup"><span data-stu-id="9e877-123">FBA</span></span>  <br/> |<span data-ttu-id="9e877-124">フォームベース認証。</span><span class="sxs-lookup"><span data-stu-id="9e877-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="9e877-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="9e877-125">NTLM</span></span>  <br/> |<span data-ttu-id="9e877-126">NTLM 認証。</span><span class="sxs-lookup"><span data-stu-id="9e877-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="9e877-127">Digest</span><span class="sxs-lookup"><span data-stu-id="9e877-127">Digest</span></span>  <br/> |<span data-ttu-id="9e877-128">ダイジェスト認証。</span><span class="sxs-lookup"><span data-stu-id="9e877-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="9e877-129">基本</span><span class="sxs-lookup"><span data-stu-id="9e877-129">Basic</span></span>  <br/> |<span data-ttu-id="9e877-130">基本認証。</span><span class="sxs-lookup"><span data-stu-id="9e877-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9e877-131">子要素</span><span class="sxs-lookup"><span data-stu-id="9e877-131">Child elements</span></span>

<span data-ttu-id="9e877-132">なし。</span><span class="sxs-lookup"><span data-stu-id="9e877-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e877-133">親要素</span><span class="sxs-lookup"><span data-stu-id="9e877-133">Parent elements</span></span>

|<span data-ttu-id="9e877-134">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e877-134">**Element**</span></span>|<span data-ttu-id="9e877-135">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e877-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e877-136">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="9e877-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="9e877-137">クライアントがファイアウォールの内側にいる場合に接続できる Outlook Web Access Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9e877-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e877-138">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e877-138">Text value</span></span>

<span data-ttu-id="9e877-139">Text 値は、クライアントアクセスサーバー上の Outlook Web Access サービスの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="9e877-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9e877-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e877-140">See also</span></span>



[<span data-ttu-id="9e877-141">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e877-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

