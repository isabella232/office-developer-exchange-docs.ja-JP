---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: EcpUrl 要素は、EcpUrl (POX) 要素の値と組み合わせて、メールが有効なユーザーの電子メールメッセージ追跡設定にアクセスするために使用できる URL を生成できる部分的な URL を指定します。
ms.openlocfilehash: 097811add5635bca14c659814652bca244a1398d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458713"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="b1b13-103">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="b1b13-104">**EcpUrl**要素は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メールメッセージ追跡設定にアクセスするために使用できる url を生成できる部分的な url を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1b13-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="b1b13-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="b1b13-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="b1b13-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="b1b13-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="b1b13-109">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b1b13-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b1b13-110">Attributes and elements</span></span>

<span data-ttu-id="b1b13-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b1b13-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1b13-112">属性</span><span class="sxs-lookup"><span data-stu-id="b1b13-112">Attributes</span></span>

<span data-ttu-id="b1b13-113">なし。</span><span class="sxs-lookup"><span data-stu-id="b1b13-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1b13-114">子要素</span><span class="sxs-lookup"><span data-stu-id="b1b13-114">Child elements</span></span>

<span data-ttu-id="b1b13-115">なし。</span><span class="sxs-lookup"><span data-stu-id="b1b13-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1b13-116">親要素</span><span class="sxs-lookup"><span data-stu-id="b1b13-116">Parent elements</span></span>

|<span data-ttu-id="b1b13-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="b1b13-117">**Element**</span></span>|<span data-ttu-id="b1b13-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="b1b13-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1b13-119">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="b1b13-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b1b13-120">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b1b13-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b1b13-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b1b13-121">Text value</span></span>

<span data-ttu-id="b1b13-122">テキスト値は、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、ユーザーの電子メール追跡設定にアクセスするために使用できる url を生成できる url の部分を表します。</span><span class="sxs-lookup"><span data-stu-id="b1b13-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="b1b13-123">**EcpUrl**要素の値には、次の表に示すように、クライアントによって置き換えられる ' < ' と ' > ' 文字に含まれるパラメータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b1b13-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="b1b13-124">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="b1b13-124">**Parameter**</span></span>|<span data-ttu-id="b1b13-125">**代用**</span><span class="sxs-lookup"><span data-stu-id="b1b13-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="b1b13-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="b1b13-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="b1b13-127">n</span><span class="sxs-lookup"><span data-stu-id="b1b13-127">n</span></span>  <br/> |
| <span data-ttu-id="b1b13-128">_MsgID_</span><span class="sxs-lookup"><span data-stu-id="b1b13-128">_MsgID_</span></span> <br/> |<span data-ttu-id="b1b13-129">メッセージ ID ヘッダーで指定されているように追跡するメッセージのインターネットメッセージ id。</span><span class="sxs-lookup"><span data-stu-id="b1b13-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="b1b13-130">_.Dbx_</span><span class="sxs-lookup"><span data-stu-id="b1b13-130">_Mbx_</span></span> <br/> |<span data-ttu-id="b1b13-131">メールボックスの所有者の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="b1b13-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="b1b13-132">_Sender_</span><span class="sxs-lookup"><span data-stu-id="b1b13-132">_Sender_</span></span> <br/> |<span data-ttu-id="b1b13-133">メッセージの送信者の SMTP アドレス。</span><span class="sxs-lookup"><span data-stu-id="b1b13-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1b13-134">注釈</span><span class="sxs-lookup"><span data-stu-id="b1b13-134">Remarks</span></span>

<span data-ttu-id="b1b13-135">**EcpUrl**要素は、 **Protocol**要素のオプションの子要素です。</span><span class="sxs-lookup"><span data-stu-id="b1b13-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b1b13-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="b1b13-136">See also</span></span>



[<span data-ttu-id="b1b13-137">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="b1b13-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

