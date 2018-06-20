---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: EcpUrl tmEditing 要素は、サイトの既存のメールボックスの編集に使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 29b27ffe9ef3c18a3b6471ca4a42956a43a5aaa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760188"
---
# <a name="ecpurl-tmediting-pox"></a><span data-ttu-id="820c6-103">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-103">EcpUrl-tmEditing (POX)</span></span>

<span data-ttu-id="820c6-104">**EcpUrl tmEditing**要素は、サイトの既存のメールボックスの編集に使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="820c6-104">The **EcpUrl-tmEditing** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> 
  
[<span data-ttu-id="820c6-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="820c6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="820c6-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="820c6-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="820c6-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="820c6-109">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-109">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="820c6-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="820c6-110">Attributes and elements</span></span>

<span data-ttu-id="820c6-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="820c6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="820c6-112">属性</span><span class="sxs-lookup"><span data-stu-id="820c6-112">Attributes</span></span>

<span data-ttu-id="820c6-113">なし。</span><span class="sxs-lookup"><span data-stu-id="820c6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="820c6-114">子要素</span><span class="sxs-lookup"><span data-stu-id="820c6-114">Child elements</span></span>

<span data-ttu-id="820c6-115">なし。</span><span class="sxs-lookup"><span data-stu-id="820c6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="820c6-116">親要素</span><span class="sxs-lookup"><span data-stu-id="820c6-116">Parent elements</span></span>

|<span data-ttu-id="820c6-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="820c6-117">**Element**</span></span>|<span data-ttu-id="820c6-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="820c6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="820c6-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="820c6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="820c6-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="820c6-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="820c6-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="820c6-121">Text value</span></span>

<span data-ttu-id="820c6-122">テキスト値は、サイトの既存のメールボックスの編集に使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を表します。</span><span class="sxs-lookup"><span data-stu-id="820c6-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> <span data-ttu-id="820c6-123">**EcpUrl tmEditing**要素の値には、内に含まれるパラメーターが含まれています '<' と' >' 文字を次の表に示すようにクライアントによって置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="820c6-123">The value of the **EcpUrl-tmEditing** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="820c6-124">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="820c6-124">**Parameter**</span></span>|<span data-ttu-id="820c6-125">**置き換える**</span><span class="sxs-lookup"><span data-stu-id="820c6-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="820c6-126">
  _Id_</span><span class="sxs-lookup"><span data-stu-id="820c6-126">_Id_</span></span> <br/> |<span data-ttu-id="820c6-127">SMTP 電子メール アドレス、または、X500 は、サイトのメールボックスの名前を識別します。</span><span class="sxs-lookup"><span data-stu-id="820c6-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="820c6-128">備考</span><span class="sxs-lookup"><span data-stu-id="820c6-128">Remarks</span></span>

<span data-ttu-id="820c6-129">**EcpUrl tmEditing**要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="820c6-129">The **EcpUrl-tmEditing** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="820c6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="820c6-130">See also</span></span>



[<span data-ttu-id="820c6-131">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="820c6-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

