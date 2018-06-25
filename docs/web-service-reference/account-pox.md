---
title: アカウント (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: アカウントの要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。
ms.openlocfilehash: 88911aad41816f7cefbffef151e066fe5d4da192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760437"
---
# <a name="account-pox"></a><span data-ttu-id="ecf67-103">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-103">Account (POX)</span></span>

<span data-ttu-id="ecf67-104">**アカウント**の要素はユーザーのアカウントの設定を指定またはエラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="ecf67-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="ecf67-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="ecf67-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="ecf67-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-107">Account (POX)</span></span>](account-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="ecf67-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ecf67-108">Attributes and elements</span></span>

<span data-ttu-id="ecf67-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ecf67-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecf67-110">属性</span><span class="sxs-lookup"><span data-stu-id="ecf67-110">Attributes</span></span>

<span data-ttu-id="ecf67-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ecf67-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecf67-112">子要素</span><span class="sxs-lookup"><span data-stu-id="ecf67-112">Child elements</span></span>

|<span data-ttu-id="ecf67-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ecf67-113">**Element**</span></span>|<span data-ttu-id="ecf67-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ecf67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecf67-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="ecf67-116">アカウントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ecf67-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-117">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="ecf67-118">ユーザーの構成情報を取得する別の自動検出要求が必要かどうかを決定するために使用される情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ecf67-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="ecf67-120">Office 365 の一部としてかどうかユーザーのメールボックスがホストされている Exchange オンラインまたは Exchange Online を示す値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="ecf67-122">クライアント アクセス サーバーの役割がインストールされている自動検出の設定を取得するために使用する必要があります Exchange Server を実行しているコンピューターの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="ecf67-124">以降の自動検出要求に使用する電子メール アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="ecf67-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-125">イメージ (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="ecf67-126">構成のエクスペリエンスのブランド化に使用されるイメージのパスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="ecf67-128">インターネット サービス プロバイダー (ISP) のホーム ページの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="ecf67-129">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ecf67-130">クライアント アクセス サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="ecf67-132">クライアント ユーザーのパブリック フォルダー情報を検出する自動検出要求の送信に使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="ecf67-133">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="ecf67-134">自動検出エラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ecf67-135">親要素</span><span class="sxs-lookup"><span data-stu-id="ecf67-135">Parent elements</span></span>

|<span data-ttu-id="ecf67-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="ecf67-136">**Element**</span></span>|<span data-ttu-id="ecf67-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="ecf67-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ecf67-138">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="ecf67-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="ecf67-139">自動検出サービスからの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ecf67-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecf67-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="ecf67-140">See also</span></span>

- [<span data-ttu-id="ecf67-141">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ecf67-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

