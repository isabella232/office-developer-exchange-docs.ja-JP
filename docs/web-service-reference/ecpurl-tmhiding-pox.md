---
title: EcpUrl-tmHiding 表示 (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: EcpUrl 非表示要素は、EcpUrl (POX) 要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる URL を生成できる url の一部を指定します。
ms.openlocfilehash: 68b949db8b8d98caddbac3b9f96c5d5e55b104b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463532"
---
# <a name="ecpurl-tmhiding-pox"></a><span data-ttu-id="9683c-103">EcpUrl-tmHiding 表示 (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-103">EcpUrl-tmHiding (POX)</span></span>

<span data-ttu-id="9683c-104">**EcpUrl 非表示**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる url を生成できる url の一部を指定します。</span><span class="sxs-lookup"><span data-stu-id="9683c-104">The **EcpUrl-tmHiding** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> 
  
[<span data-ttu-id="9683c-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9683c-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9683c-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9683c-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9683c-109">EcpUrl-tmHiding 表示 (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-109">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9683c-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9683c-110">Attributes and elements</span></span>

<span data-ttu-id="9683c-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9683c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9683c-112">属性</span><span class="sxs-lookup"><span data-stu-id="9683c-112">Attributes</span></span>

<span data-ttu-id="9683c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9683c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9683c-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9683c-114">Child elements</span></span>

<span data-ttu-id="9683c-115">なし。</span><span class="sxs-lookup"><span data-stu-id="9683c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9683c-116">親要素</span><span class="sxs-lookup"><span data-stu-id="9683c-116">Parent elements</span></span>

|<span data-ttu-id="9683c-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="9683c-117">**Element**</span></span>|<span data-ttu-id="9683c-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="9683c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9683c-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="9683c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9683c-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9683c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9683c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9683c-121">Text value</span></span>

<span data-ttu-id="9683c-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、サイトメールボックスからユーザーの登録を解除するために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="9683c-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> <span data-ttu-id="9683c-123">**EcpUrl 非表示**要素の値には、次の表に示すように、クライアントによって置き換えられる ' < ' および ' > ' 文字に含まれるパラメーターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9683c-123">The value of the **EcpUrl-tmHiding** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="9683c-124">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="9683c-124">**Parameter**</span></span>|<span data-ttu-id="9683c-125">**代用**</span><span class="sxs-lookup"><span data-stu-id="9683c-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="9683c-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="9683c-126">_Id_</span></span> <br/> |<span data-ttu-id="9683c-127">サイトメールボックスの SMTP 電子メールアドレスまたは X500 識別名。</span><span class="sxs-lookup"><span data-stu-id="9683c-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9683c-128">注釈</span><span class="sxs-lookup"><span data-stu-id="9683c-128">Remarks</span></span>

<span data-ttu-id="9683c-129">**EcpUrl 非表示**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="9683c-129">The **EcpUrl-tmHiding** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9683c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="9683c-130">See also</span></span>



[<span data-ttu-id="9683c-131">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="9683c-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

