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
description: Account 要素は、ユーザーのアカウント設定を指定するか、エラー応答を含みます。
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462319"
---
# <a name="account-pox"></a><span data-ttu-id="17860-103">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-103">Account (POX)</span></span>

<span data-ttu-id="17860-104">**Account**要素は、ユーザーのアカウント設定を指定するか、エラー応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="17860-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="17860-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="17860-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="17860-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-107">Account (POX)</span></span>](account-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="17860-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="17860-108">Attributes and elements</span></span>

<span data-ttu-id="17860-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="17860-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17860-110">属性</span><span class="sxs-lookup"><span data-stu-id="17860-110">Attributes</span></span>

<span data-ttu-id="17860-111">なし。</span><span class="sxs-lookup"><span data-stu-id="17860-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17860-112">子要素</span><span class="sxs-lookup"><span data-stu-id="17860-112">Child elements</span></span>

|<span data-ttu-id="17860-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="17860-113">**Element**</span></span>|<span data-ttu-id="17860-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="17860-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17860-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="17860-116">アカウントの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="17860-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="17860-117">アクション (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="17860-118">ユーザー構成情報を返すために別の自動検出要求が必要かどうかを判断するために使用される情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="17860-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="17860-119">Microsoft Online (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="17860-120">ユーザーのメールボックスが、Office 365 の一部として Exchange Online または Exchange Online でホストされているかどうかを示す値を格納します。</span><span class="sxs-lookup"><span data-stu-id="17860-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="17860-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="17860-122">自動検出設定を取得するために使用する必要がある、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17860-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="17860-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="17860-124">以降の自動検出要求に使用する電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="17860-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="17860-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="17860-126">構成環境をブランド化するために使用されるイメージのパスを含みます。</span><span class="sxs-lookup"><span data-stu-id="17860-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="17860-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="17860-128">インターネットサービスプロバイダー (ISP) のホームページの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17860-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="17860-129">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="17860-130">クライアントをクライアントアクセスサーバーに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17860-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="17860-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="17860-132">クライアントが、ユーザーのパブリックフォルダー情報を検出するために自動検出要求を送信するために使用できる情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="17860-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="17860-133">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="17860-134">自動検出エラー応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="17860-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="17860-135">親要素</span><span class="sxs-lookup"><span data-stu-id="17860-135">Parent elements</span></span>

|<span data-ttu-id="17860-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="17860-136">**Element**</span></span>|<span data-ttu-id="17860-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="17860-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17860-138">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="17860-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="17860-139">自動検出サービスからの応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="17860-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17860-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="17860-140">See also</span></span>

- [<span data-ttu-id="17860-141">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="17860-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

