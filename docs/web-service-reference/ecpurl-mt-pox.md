---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: EcpUrl mt の要素では、メールが有効なユーザーの設定を追跡する電子メール メッセージにアクセスするために使用できる URL を生成する EcpUrl (POX) 要素の値と組み合わせて使用できますが、部分的な URL を指定します。
ms.openlocfilehash: 13954a4dab8e81f4ba75b3578e6ba7f67f4b8b96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760176"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="6bd4e-103">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="6bd4e-104">**EcpUrl mt**の要素では、メールが有効なユーザーの設定を追跡する電子メール メッセージにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="6bd4e-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="6bd4e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6bd4e-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6bd4e-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6bd4e-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6bd4e-109">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6bd4e-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6bd4e-110">Attributes and elements</span></span>

<span data-ttu-id="6bd4e-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bd4e-112">属性</span><span class="sxs-lookup"><span data-stu-id="6bd4e-112">Attributes</span></span>

<span data-ttu-id="6bd4e-113">なし。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bd4e-114">子要素</span><span class="sxs-lookup"><span data-stu-id="6bd4e-114">Child elements</span></span>

<span data-ttu-id="6bd4e-115">なし。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6bd4e-116">親要素</span><span class="sxs-lookup"><span data-stu-id="6bd4e-116">Parent elements</span></span>

|<span data-ttu-id="6bd4e-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="6bd4e-117">**Element**</span></span>|<span data-ttu-id="6bd4e-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="6bd4e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bd4e-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="6bd4e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6bd4e-120">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bd4e-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6bd4e-121">Text value</span></span>

<span data-ttu-id="6bd4e-122">テキスト値は、部分的な進捗管理の設定、ユーザーの電子メールにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できます URL を表します。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="6bd4e-123">**EcpUrl mt**の要素の値には、内に含まれるパラメーターが含まれています '<' と' >' 文字を次の表に示すようにクライアントによって置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="6bd4e-124">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="6bd4e-124">**Parameter**</span></span>|<span data-ttu-id="6bd4e-125">**置き換える**</span><span class="sxs-lookup"><span data-stu-id="6bd4e-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="6bd4e-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="6bd4e-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="6bd4e-127">n</span><span class="sxs-lookup"><span data-stu-id="6bd4e-127">n</span></span>  <br/> |
| <span data-ttu-id="6bd4e-128">_MsgID_</span><span class="sxs-lookup"><span data-stu-id="6bd4e-128">_MsgID_</span></span> <br/> |<span data-ttu-id="6bd4e-129">追跡するメッセージのインターネット メッセージ id、メッセージ ID ヘッダーで指定されたとおりです。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="6bd4e-130">_Mbx_</span><span class="sxs-lookup"><span data-stu-id="6bd4e-130">_Mbx_</span></span> <br/> |<span data-ttu-id="6bd4e-131">メールボックス所有者の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="6bd4e-132">_送信者_</span><span class="sxs-lookup"><span data-stu-id="6bd4e-132">_Sender_</span></span> <br/> |<span data-ttu-id="6bd4e-133">メッセージの送信者の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6bd4e-134">備考</span><span class="sxs-lookup"><span data-stu-id="6bd4e-134">Remarks</span></span>

<span data-ttu-id="6bd4e-135">**EcpUrl mt**の要素は、**プロトコル**要素の省略可能な子要素です。</span><span class="sxs-lookup"><span data-stu-id="6bd4e-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6bd4e-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="6bd4e-136">See also</span></span>



[<span data-ttu-id="6bd4e-137">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6bd4e-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

