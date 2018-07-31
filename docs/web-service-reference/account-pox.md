---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: アカウントの要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353344"
---
# <a name="account-pox"></a><span data-ttu-id="b0b6c-103">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-103">Account (POX)</span></span>

<span data-ttu-id="b0b6c-104">**アカウント**の要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="b0b6c-105">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="b0b6c-106">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="b0b6c-107">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-107">Account (POX)</span></span>](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b0b6c-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b0b6c-108">Attributes and elements</span></span>

<span data-ttu-id="b0b6c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0b6c-110">属性</span><span class="sxs-lookup"><span data-stu-id="b0b6c-110">Attributes</span></span>

<span data-ttu-id="b0b6c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0b6c-112">子要素</span><span class="sxs-lookup"><span data-stu-id="b0b6c-112">Child elements</span></span>

|<span data-ttu-id="b0b6c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0b6c-113">**Element**</span></span>|<span data-ttu-id="b0b6c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0b6c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0b6c-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="b0b6c-116">アカウントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="b0b6c-118">ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="b0b6c-120">Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="b0b6c-122">クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Exchange Server を実行しているコンピューターの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="b0b6c-124">以降の自動検出要求に使用する電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-125">イメージ (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="b0b6c-126">構成のエクスペリエンスのブランド化に使用されるイメージのパスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="b0b6c-128">インターネット サービス プロバイダー (ISP) のホーム ページの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b0b6c-130">クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="b0b6c-132">クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="b0b6c-133">Error (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="b0b6c-134">自動検出エラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0b6c-135">親要素</span><span class="sxs-lookup"><span data-stu-id="b0b6c-135">Parent elements</span></span>

|<span data-ttu-id="b0b6c-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="b0b6c-136">**Element**</span></span>|<span data-ttu-id="b0b6c-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="b0b6c-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0b6c-138">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="b0b6c-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="b0b6c-139">自動検出サービスからの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b0b6c-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0b6c-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="b0b6c-140">See also</span></span>

- [<span data-ttu-id="b0b6c-141">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b0b6c-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

