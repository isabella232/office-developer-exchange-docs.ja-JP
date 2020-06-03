---
title: プロトコル (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: Protocol 要素には、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: 6fca347f49e27958ecb16cce345387b6a2146979
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467761"
---
# <a name="protocol-pox"></a><span data-ttu-id="5301f-103">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-103">Protocol (POX)</span></span>

<span data-ttu-id="5301f-104">**Protocol**要素には、クライアントアクセスサーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-104">The **Protocol** element contains the specifications for connecting a client to the computer that is running Exchange Server that has the Client Access server role installed.</span></span> 
  
[<span data-ttu-id="5301f-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5301f-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="5301f-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="5301f-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
```xml
<Protocol>
   <Type/>
   <Internal/>
   <External/>
   <TTL/>
   <Server/>
   <ServerDN/>
   <ServerVersion/>
   <MdbDN/>
   <PublicFolderServer/>
   <Port/>
   <DirectoryPort/>
   <ReferralPort/>
   <ASUrl/>
   <EwsUrl/>
   <EmwsUrl/>
   <SharingUrl/>
   <EcpUrl/>
   <EcpUrl-um/>
   <EcpUrl-aggr/>
   <EcpUrl-mt/>
   <EcpUrl-ret/>
   <EcpUrl-sms/>
   <EcpUrl-publish/>
   <EcpUrl-photo/>
   <EcpUrl-tm/>
   <EcpUrl-tmCreating/>
   <EcpUrl-tmHiding/>
   <EcpUrl-tmEditing/>
   <EcpUrl-extinstall/>
   <OOFUrl/>
   <OABUrl/>
   <UMUrl/>
   <EwsPartnerUrl/>
   <LoginName/>
   <DomainRequired/>
   <DomainName/>
   <SPA/>
   <AuthPackage/>
   <CertPrincipalName/>
   <SSL/>
   <AuthRequired/>
   <UsePOPAuth/>
   <SMTPLast/>
   <NetworkRequirements/>
   <AddressBook/>
   <MailStore/>
</Protocol>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5301f-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5301f-109">Attributes and elements</span></span>

<span data-ttu-id="5301f-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5301f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5301f-111">属性</span><span class="sxs-lookup"><span data-stu-id="5301f-111">Attributes</span></span>

|<span data-ttu-id="5301f-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="5301f-112">**Attribute**</span></span>|<span data-ttu-id="5301f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5301f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5301f-114">種類</span><span class="sxs-lookup"><span data-stu-id="5301f-114">Type</span></span>  <br/> |<span data-ttu-id="5301f-115">この**プロトコル**要素で記述されているプロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="5301f-115">Indicates the type of protocol described by this **Protocol** element.</span></span> <span data-ttu-id="5301f-116">この属性の有効な値は "Http" だけです。</span><span class="sxs-lookup"><span data-stu-id="5301f-116">The only valid value for this attribute is "mapiHttp".</span></span> <span data-ttu-id="5301f-117">この属性は、この応答に対応する自動検出要求に[MapiHttpCapability ヘッダーが含まれて](pox-autodiscover-request-for-exchange.md)いた場合にのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="5301f-117">This attribute is only present if the Autodiscover request that corresponds to this response [included an X-MapiHttpCapability header](pox-autodiscover-request-for-exchange.md).</span></span> <span data-ttu-id="5301f-118">この属性は、MAPI/HTTP プロトコルおよびターゲット Exchange Online の一部としての Exchange Online、Office 365 の一部としての Exchange Online、または、build 15.00.0847.032 (Exchange Server 2013 SP1) 以降の Exchange のオンプレミスバージョンを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5301f-118">This attribute is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, or on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>  <br/> |
|<span data-ttu-id="5301f-119">バージョン</span><span class="sxs-lookup"><span data-stu-id="5301f-119">Version</span></span>  <br/> |<span data-ttu-id="5301f-120">この**プロトコル**要素で記述されているプロトコルのバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="5301f-120">Indicates the version of the protocol described by this **Protocol** element.</span></span> <span data-ttu-id="5301f-121">この属性の有効な値は "1" だけです。</span><span class="sxs-lookup"><span data-stu-id="5301f-121">The only valid value for this attribute is "1".</span></span> <span data-ttu-id="5301f-122">この属性は、この応答に対応する自動検出要求に**MapiHttpCapability**ヘッダーが含まれていた場合にのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="5301f-122">This attribute is only present if the Autodiscover request that corresponds to this response included an **X-MapiHttpCapability** header.</span></span> <span data-ttu-id="5301f-123">この属性は、MAPI/HTTP プロトコルおよびターゲット Exchange Online の一部としての Exchange Online、Office 365 の一部としての Exchange Online、または、build 15.00.0847.032 (Exchange Server 2013 SP1) 以降の Exchange のオンプレミスバージョンを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5301f-123">This attribute is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, or on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5301f-124">子要素</span><span class="sxs-lookup"><span data-stu-id="5301f-124">Child elements</span></span>

|<span data-ttu-id="5301f-125">**Element**</span><span class="sxs-lookup"><span data-stu-id="5301f-125">**Element**</span></span>|<span data-ttu-id="5301f-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="5301f-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5301f-127">種類 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-127">Type (POX)</span></span>](type-pox.md) <br/> |<span data-ttu-id="5301f-128">構成されているメールアカウントの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="5301f-128">Identifies the type of the configured mail account.</span></span>  <br/> |
|[<span data-ttu-id="5301f-129">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-129">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="5301f-130">組織のネットワーク内から Exchange に接続するためにクライアントが使用できる Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-130">Contains a collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span>  <br/> |
|[<span data-ttu-id="5301f-131">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-131">External (POX)</span></span>](external-pox.md) <br/> |<span data-ttu-id="5301f-132">組織のネットワーク外から Exchange に接続するためにクライアントが使用できる Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-132">Contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span>  <br/> |
|[<span data-ttu-id="5301f-133">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-133">TTL (POX)</span></span>](ttl-pox.md) <br/> |<span data-ttu-id="5301f-134">設定が有効なままになる時間を時間単位で指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-134">Specifies the Time to Live, in hours, during which the settings remain valid.</span></span>  <br/> |
|[<span data-ttu-id="5301f-135">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-135">Server (POX)</span></span>](server-pox.md) <br/> |<span data-ttu-id="5301f-136">メールサーバーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-136">Specifies the name of the mail server.</span></span>  <br/> |
|[<span data-ttu-id="5301f-137">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-137">ServerDN (POX)</span></span>](serverdn-pox.md) <br/> |<span data-ttu-id="5301f-138">Exchange サーバーの識別名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-138">Specifies the Exchange Server distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="5301f-139">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-139">ServerVersion (POX)</span></span>](serverversion-pox.md) <br/> |<span data-ttu-id="5301f-140">Exchange サーバーのバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="5301f-140">Represents the Exchange Server version number.</span></span>  <br/> |
|[<span data-ttu-id="5301f-141">MdbDN (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-141">MdbDN (POX)</span></span>](mdbdn-pox.md) <br/> |<span data-ttu-id="5301f-142">メールボックスデータベースの識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="5301f-142">Represents the distinguished name of the mailbox database.</span></span>  <br/> |
|[<span data-ttu-id="5301f-143">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-143">PublicFolderServer (POX)</span></span>](publicfolderserver-pox.md) <br/> |<span data-ttu-id="5301f-144">ユーザーのパブリックフォルダーサーバーの完全修飾ドメイン名 (FQDN) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-144">Contains the fully-qualified domain name (FQDN) of the public folder server for the user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-145">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-145">Port (POX)</span></span>](port-pox.md) <br/> |<span data-ttu-id="5301f-146">ストアへの接続に使用するポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-146">Specifies the port that is used to connect to the store.</span></span>  <br/> |
|[<span data-ttu-id="5301f-147">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-147">DirectoryPort (POX)</span></span>](directoryport-pox.md) <br/> |<span data-ttu-id="5301f-148">ネームサービスプロバイダインターフェイス (NSPI) プロトコルが使用されている場合に、ディレクトリへの接続に使用するポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-148">Specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span>  <br/> |
|[<span data-ttu-id="5301f-149">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-149">ReferralPort (POX)</span></span>](referralport-pox.md) <br/> |<span data-ttu-id="5301f-150">ディレクトリへの参照を取得するために使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-150">Specifies the port that is used to get a referral to a directory.</span></span>  <br/> |
|[<span data-ttu-id="5301f-151">ASUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-151">ASUrl (POX)</span></span>](asurl-pox.md) <br/> |<span data-ttu-id="5301f-152">メールが有効なユーザーの Exchange Web サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-152">Specifies the URL of the best instance of the Exchange Web Services for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-153">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-153">EwsUrl (POX)</span></span>](ewsurl-pox.md) <br/> |<span data-ttu-id="5301f-154">メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-154">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-155">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-155">EmwsUrl (POX)</span></span>](emwsurl-pox.md) <br/> |<span data-ttu-id="5301f-156">メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-156">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-157">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-157">SharingUrl (POX)</span></span>](sharingurl-pox.md) <br/> |<span data-ttu-id="5301f-158">予定表と連絡先を組織間で共有するために使用される共有サーバーの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-158">Contains the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span>  <br/> |
|[<span data-ttu-id="5301f-159">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-159">EcpUrl (POX)</span></span>](ecpurl-pox.md) <br/> |<span data-ttu-id="5301f-160">メールが有効なユーザーの Exchange コントロールパネルの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-160">Specifies the URL of the Exchange Control Panel for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-161">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-161">EcpUrl-um (POX)</span></span>](ecpurl-um-pox.md) <br/> |<span data-ttu-id="5301f-162">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのボイスメール設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-162">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-163">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-163">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md) <br/> |<span data-ttu-id="5301f-164">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メール集計の設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-164">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-165">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-165">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md) <br/> |<span data-ttu-id="5301f-166">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの電子メールメッセージ追跡設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-166">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-167">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-167">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md) <br/> |<span data-ttu-id="5301f-168">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの保持タグの設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-168">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-169">EcpUrl-sms (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-169">EcpUrl-sms (POX)</span></span>](ecpurl-sms-pox.md) <br/> |<span data-ttu-id="5301f-170">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーのショートメッセージサービス (SMS) の設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-170">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access Short Message Service (SMS) settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-171">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-171">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md) <br/> |<span data-ttu-id="5301f-172">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの予定表の発行設定にアクセスするために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-172">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-173">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-173">EcpUrl-photo (POX)</span></span>](ecpurl-photo-pox.md) <br/> |<span data-ttu-id="5301f-174">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、メールが有効なユーザーの現在の写真を表示または変更するために使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-174">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change a mail-enabled user's current photo.</span></span>  <br/> |
|[<span data-ttu-id="5301f-175">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-175">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md) <br/> |<span data-ttu-id="5301f-176">メールが有効なユーザーが現在メンバーであるすべてのサイトメールボックスのリストにアクセスするために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて指定できる url の一部を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-176">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span>  <br/> |
|[<span data-ttu-id="5301f-177">EcpUrl-tmCreating 作成 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-177">EcpUrl-tmCreating (POX)</span></span>](ecpurl-tmcreating-pox.md) <br/> |<span data-ttu-id="5301f-178">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、新しいサイトメールボックスの作成に使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-178">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5301f-179">EcpUrl-tmHiding 表示 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-179">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md) <br/> |<span data-ttu-id="5301f-180">サイトメールボックスからのユーザーの登録を解除するために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-180">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5301f-181">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-181">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md) <br/> |<span data-ttu-id="5301f-182">[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて、既存のサイトメールボックスの編集に使用できる url を生成できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-182">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5301f-183">EcpUrl-extinstall (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-183">EcpUrl-extinstall (POX)</span></span>](ecpurl-extinstall-pox.md) <br/> |<span data-ttu-id="5301f-184">ユーザーのメールボックスに現在インストールされているメールアプリを表示または変更するために使用できる URL を生成するために、 [EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できる url の部分を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-184">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change the mail apps currently installed in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5301f-185">OOFUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-185">OOFUrl (POX)</span></span>](oofurl-pox.md) <br/> |<span data-ttu-id="5301f-186">メールが有効なユーザーの空き時間情報サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-186">Specifies the URL of the best instance of the Availability service for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-187">OABUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-187">OABUrl (POX)</span></span>](oaburl-pox.md) <br/> |<span data-ttu-id="5301f-188">Exchange トポロジのオフラインアドレス帳構成サーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-188">Specifies the Offline Address Book configuration server URL for an Exchange topology.</span></span>  <br/> |
|[<span data-ttu-id="5301f-189">UMUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-189">UMUrl (POX)</span></span>](umurl-pox.md) <br/> |<span data-ttu-id="5301f-190">メールが有効なユーザーに対して、ユニファイドメッセージング Web サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-190">Specifies the URL of the best instance of the Unified Messaging Web service for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-191">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-191">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md) <br/> |<span data-ttu-id="5301f-192">メールが有効なユーザーのために、Exchange Web サービス (EWS) の最適なエンドポイントインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-192">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5301f-193">ログイン (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-193">LoginName (POX)</span></span>](loginname-pox.md) <br/> |<span data-ttu-id="5301f-194">ユーザーのログオン名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-194">Specifies the user's logon name.</span></span>  <br/> |
|[<span data-ttu-id="5301f-195">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-195">DomainRequired (POX)</span></span>](domainrequired-pox.md) <br/> |<span data-ttu-id="5301f-196">ドメインが認証に必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5301f-196">Indicates whether the domain is required for authentication.</span></span>  <br/> |
|[<span data-ttu-id="5301f-197">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-197">DomainName (POX)</span></span>](domainname-pox.md) <br/> |<span data-ttu-id="5301f-198">ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-198">Specifies the user's domain.</span></span>  <br/> |
|[<span data-ttu-id="5301f-199">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-199">SPA (POX)</span></span>](spa-pox.md) <br/> |<span data-ttu-id="5301f-200">セキュリティで保護されたパスワード認証が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5301f-200">Indicates whether secure password authentication is required.</span></span>  <br/> |
|[<span data-ttu-id="5301f-201">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-201">AuthPackage (POX)</span></span>](authpackage-pox.md) <br/> |<span data-ttu-id="5301f-202">メールボックスサーバーの役割がインストールされている Exchange 2007 コンピューターに対して認証を行うときに使用する認証方式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-202">Specifies the authentication scheme that is used when authenticating against the Exchange 2007 computer that has the Mailbox server role installed.</span></span>  <br/> |
|[<span data-ttu-id="5301f-203">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-203">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md) <br/> |<span data-ttu-id="5301f-204">SSL を使用して Microsoft Exchange 組織に接続するために必要な SSL (Secure Sockets Layer) 証明書プリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-204">Specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>  <br/> |
|[<span data-ttu-id="5301f-205">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-205">SSL (POX)</span></span>](ssl-pox.md) <br/> |<span data-ttu-id="5301f-206">セキュリティで保護されたログオンが必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-206">Specifies whether secure logon is needed.</span></span>  <br/> |
|[<span data-ttu-id="5301f-207">AuthRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-207">AuthRequired (POX)</span></span>](authrequired-pox.md) <br/> |<span data-ttu-id="5301f-208">認証が必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-208">Specifies whether authentication is required.</span></span>  <br/> |
|[<span data-ttu-id="5301f-209">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-209">UsePOPAuth (POX)</span></span>](usepopauth-pox.md) <br/> |<span data-ttu-id="5301f-210">POP3 の種類のアカウントに対して提供された認証情報が簡易メール転送プロトコル (SMTP) にも使用されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5301f-210">Indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span>  <br/> |
|[<span data-ttu-id="5301f-211">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-211">SMTPLast (POX)</span></span>](smtplast-pox.md) <br/> |<span data-ttu-id="5301f-212">Smtp サーバーを使用して電子メールを送信する前に、SMTP サーバーで電子メールをダウンロードする必要があるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-212">Specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="5301f-213">NetworkRequirements 要件 (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-213">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md) <br/> |<span data-ttu-id="5301f-214">サーバーに接続するためのインターネットサービスプロバイダーの要件を満たすネットワーク上にクライアントコンピューターがあるかどうかを判断するために使用される条件が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-214">Contains the criteria that are used to determine whether the client computer is on a network that meets the Internet Service Provider's requirements to connect to the server.</span></span>  <br/> |
|[<span data-ttu-id="5301f-215">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-215">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="5301f-216">MAPI/HTTP プロトコルを使用して、アドレス帳サーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-216">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="5301f-217">この要素は、 **Protocol**要素の**Type**属性が存在し、"http" に設定されている場合にのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="5301f-217">This element is only present if the **Type** attribute on the **Protocol** element is present and set to "mapiHttp".</span></span> <span data-ttu-id="5301f-218">**AddressBook**要素は、MAPI/HTTP プロトコルと、ターゲットの exchange Online と、15.00.0847.032 以降のバージョンの exchange を実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5301f-218">The **AddressBook** element is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online and versions of Exchange starting with 15.00.0847.032.</span></span>  <br/> |
|[<span data-ttu-id="5301f-219">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-219">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="5301f-220">MAPI/HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5301f-220">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="5301f-221">この要素は、 **Protocol**要素の**Type**属性が存在し、"http" に設定されている場合にのみ存在します。</span><span class="sxs-lookup"><span data-stu-id="5301f-221">This element is only present if the **Type** attribute on the **Protocol** element is present and set to "mapiHttp".</span></span> <span data-ttu-id="5301f-222">**Mailstore**要素は、MAPI/HTTP プロトコルと、15.00.0847.032 から始まる exchange のバージョンを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5301f-222">The **MailStore** element is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online and versions of Exchange starting with 15.00.0847.032.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5301f-223">親要素</span><span class="sxs-lookup"><span data-stu-id="5301f-223">Parent elements</span></span>

|<span data-ttu-id="5301f-224">**要素**</span><span class="sxs-lookup"><span data-stu-id="5301f-224">**Element**</span></span>|<span data-ttu-id="5301f-225">**説明**</span><span class="sxs-lookup"><span data-stu-id="5301f-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5301f-226">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5301f-226">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="5301f-227">ユーザーのアカウント設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="5301f-227">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5301f-228">注釈</span><span class="sxs-lookup"><span data-stu-id="5301f-228">Remarks</span></span>

<span data-ttu-id="5301f-229">**Protocol**要素は、**設定**と同じ[処理 (POX)](action-pox.md)値を持つ応答内に存在します。</span><span class="sxs-lookup"><span data-stu-id="5301f-229">The **Protocol** element is present in a response that has an [Action (POX)](action-pox.md) value that is equal to **settings**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5301f-230">関連項目</span><span class="sxs-lookup"><span data-stu-id="5301f-230">See also</span></span>



[<span data-ttu-id="5301f-231">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="5301f-231">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

