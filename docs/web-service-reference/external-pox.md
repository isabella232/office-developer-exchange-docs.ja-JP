---
title: 外部 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: External 要素には、クライアントが組織のネットワークの外部から Exchange に接続するために使用できる Url のコレクションが含まれています。
ms.openlocfilehash: 45d7e72c5a43c5c468c1edd303a5e5ea8c2cb62e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457971"
---
# <a name="external-pox"></a><span data-ttu-id="56a17-103">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-103">External (POX)</span></span>

<span data-ttu-id="56a17-104">**External**要素には、クライアントが組織のネットワークの外部から Exchange に接続するために使用できる url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="56a17-104">The **External** element contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span> 
  
[<span data-ttu-id="56a17-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="56a17-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="56a17-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="56a17-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="56a17-109">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-109">External (POX)</span></span>](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="56a17-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="56a17-110">Attributes and elements</span></span>

<span data-ttu-id="56a17-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56a17-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56a17-112">属性</span><span class="sxs-lookup"><span data-stu-id="56a17-112">Attributes</span></span>

<span data-ttu-id="56a17-113">なし。</span><span class="sxs-lookup"><span data-stu-id="56a17-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56a17-114">子要素</span><span class="sxs-lookup"><span data-stu-id="56a17-114">Child elements</span></span>

|<span data-ttu-id="56a17-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="56a17-115">**Element**</span></span>|<span data-ttu-id="56a17-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="56a17-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a17-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="56a17-118">Outlook Web Access をホストするクライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行している特定のコンピューターにアクセスするために使用される URL と認証スキーマについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56a17-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="56a17-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="56a17-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56a17-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="56a17-121">この**プロトコル**要素には、2つの子要素 (接続プロトコルを指定する[Type (POX)](type-pox.md)要素と、可用性 web サービスの EWS エンドポイントを指定する[asurl (POX)](asurl-pox.md)要素のみが含まれます。</span><span class="sxs-lookup"><span data-stu-id="56a17-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56a17-122">親要素</span><span class="sxs-lookup"><span data-stu-id="56a17-122">Parent elements</span></span>

|<span data-ttu-id="56a17-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="56a17-123">**Element**</span></span>|<span data-ttu-id="56a17-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="56a17-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56a17-125">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="56a17-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="56a17-126">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56a17-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56a17-127">注釈</span><span class="sxs-lookup"><span data-stu-id="56a17-127">Remarks</span></span>

<span data-ttu-id="56a17-128">**External**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="56a17-128">The **External** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="56a17-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="56a17-129">See also</span></span>



[<span data-ttu-id="56a17-130">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="56a17-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

