---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: EcpUrl-tmEditing 要素は、既存のサイトメールボックスの編集に使用できる URL を生成するために、(POX) 要素の値と組み合わせることができる部分的な URL を指定します。
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463539"
---
# <a name="ecpurl-tmediting-pox"></a><span data-ttu-id="48304-103">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-103">EcpUrl-tmEditing (POX)</span></span>

<span data-ttu-id="48304-104">**EcpUrl-tmEditing**要素は、既存のサイトメールボックスの編集に使用できる url を生成するために、 [(POX)](ecpurl-pox.md)要素の値と組み合わせることができる部分的な url を指定します。</span><span class="sxs-lookup"><span data-stu-id="48304-104">The **EcpUrl-tmEditing** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> 
  
[<span data-ttu-id="48304-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="48304-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="48304-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="48304-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="48304-109">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-109">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="48304-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="48304-110">Attributes and elements</span></span>

<span data-ttu-id="48304-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="48304-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48304-112">属性</span><span class="sxs-lookup"><span data-stu-id="48304-112">Attributes</span></span>

<span data-ttu-id="48304-113">なし。</span><span class="sxs-lookup"><span data-stu-id="48304-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48304-114">子要素</span><span class="sxs-lookup"><span data-stu-id="48304-114">Child elements</span></span>

<span data-ttu-id="48304-115">なし。</span><span class="sxs-lookup"><span data-stu-id="48304-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48304-116">親要素</span><span class="sxs-lookup"><span data-stu-id="48304-116">Parent elements</span></span>

|<span data-ttu-id="48304-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="48304-117">**Element**</span></span>|<span data-ttu-id="48304-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="48304-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48304-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="48304-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="48304-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="48304-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48304-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="48304-121">Text value</span></span>

<span data-ttu-id="48304-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイトメールボックスの編集に使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="48304-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> <span data-ttu-id="48304-123">**EcpUrl-tmEditing**要素の値には、次の表に示すように、クライアントによって置き換えられる ' < ' と ' > ' 文字に含まれるパラメーターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="48304-123">The value of the **EcpUrl-tmEditing** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="48304-124">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="48304-124">**Parameter**</span></span>|<span data-ttu-id="48304-125">**代用**</span><span class="sxs-lookup"><span data-stu-id="48304-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="48304-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="48304-126">_Id_</span></span> <br/> |<span data-ttu-id="48304-127">サイトメールボックスの SMTP 電子メールアドレスまたは X500 識別名。</span><span class="sxs-lookup"><span data-stu-id="48304-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="48304-128">注釈</span><span class="sxs-lookup"><span data-stu-id="48304-128">Remarks</span></span>

<span data-ttu-id="48304-129">**EcpUrl-Tmedioffelement**は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="48304-129">The **EcpUrl-tmEditing** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="48304-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="48304-130">See also</span></span>



[<span data-ttu-id="48304-131">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="48304-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

