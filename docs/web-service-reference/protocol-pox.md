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
description: プロトコル要素には、クライアント アクセス サーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。
ms.openlocfilehash: e58ae82ea5ec9d39db0f9219f6019df7da24a343
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832926"
---
# <a name="protocol-pox"></a><span data-ttu-id="5965d-103">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-103">Protocol (POX)</span></span>

<span data-ttu-id="5965d-104">**プロトコル**要素には、クライアント アクセス サーバーの役割がインストールされている Exchange Server を実行しているコンピューターにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-104">The **Protocol** element contains the specifications for connecting a client to the computer that is running Exchange Server that has the Client Access server role installed.</span></span> 
  
[<span data-ttu-id="5965d-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="5965d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5965d-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="5965d-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="5965d-108">プロトコル (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-108">Protocol (POX)</span></span>](protocol-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="5965d-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5965d-109">Attributes and elements</span></span>

<span data-ttu-id="5965d-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5965d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5965d-111">属性</span><span class="sxs-lookup"><span data-stu-id="5965d-111">Attributes</span></span>

|<span data-ttu-id="5965d-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="5965d-112">**Attribute**</span></span>|<span data-ttu-id="5965d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5965d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5965d-114">種類</span><span class="sxs-lookup"><span data-stu-id="5965d-114">Type</span></span>  <br/> |<span data-ttu-id="5965d-115">この**プロトコル**要素で記述されたプロトコルの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="5965d-115">Indicates the type of protocol described by this **Protocol** element.</span></span> <span data-ttu-id="5965d-116">この属性の唯一の有効値は、"mapiHttp"です。</span><span class="sxs-lookup"><span data-stu-id="5965d-116">The only valid value for this attribute is "mapiHttp".</span></span> <span data-ttu-id="5965d-117">この属性は、唯一の現在の自動検出を要求する場合に対応するこの応答は[、X-MapiHttpCapability ヘッダーが含まれています](pox-autodiscover-request-for-exchange.md)。</span><span class="sxs-lookup"><span data-stu-id="5965d-117">This attribute is only present if the Autodiscover request that corresponds to this response [included an X-MapiHttpCapability header](pox-autodiscover-request-for-exchange.md).</span></span> <span data-ttu-id="5965d-118">この属性は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに適用または設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。</span><span class="sxs-lookup"><span data-stu-id="5965d-118">This attribute is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, or on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>  <br/> |
|<span data-ttu-id="5965d-119">バージョン</span><span class="sxs-lookup"><span data-stu-id="5965d-119">Version</span></span>  <br/> |<span data-ttu-id="5965d-120">この**プロトコル**要素で記述されたプロトコルのバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="5965d-120">Indicates the version of the protocol described by this **Protocol** element.</span></span> <span data-ttu-id="5965d-121">この属性の唯一の有効値は、「1」です。</span><span class="sxs-lookup"><span data-stu-id="5965d-121">The only valid value for this attribute is "1".</span></span> <span data-ttu-id="5965d-122">この属性は、この応答に対応する自動検出要求には、 **X-MapiHttpCapability**ヘッダーが含まれている場合のみです。</span><span class="sxs-lookup"><span data-stu-id="5965d-122">This attribute is only present if the Autodiscover request that corresponds to this response included an **X-MapiHttpCapability** header.</span></span> <span data-ttu-id="5965d-123">この属性は、ターゲット Exchange Online では、Office 365 の一部として Exchange Online MAPI または HTTP プロトコルを実装するクライアントに適用または設置型のバージョンの Exchange が始まる 15.00.0847.032 (Exchange Server 2013 SP1) を構築します。</span><span class="sxs-lookup"><span data-stu-id="5965d-123">This attribute is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, or on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5965d-124">子要素</span><span class="sxs-lookup"><span data-stu-id="5965d-124">Child elements</span></span>

|<span data-ttu-id="5965d-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="5965d-125">**Element**</span></span>|<span data-ttu-id="5965d-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="5965d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5965d-127">(POX) の種類</span><span class="sxs-lookup"><span data-stu-id="5965d-127">Type (POX)</span></span>](type-pox.md) <br/> |<span data-ttu-id="5965d-128">設定したメール アカウントの種類を識別します。</span><span class="sxs-lookup"><span data-stu-id="5965d-128">Identifies the type of the configured mail account.</span></span>  <br/> |
|[<span data-ttu-id="5965d-129">内部 (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-129">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="5965d-130">組織のネットワーク内から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-130">Contains a collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span>  <br/> |
|[<span data-ttu-id="5965d-131">外部 (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-131">External (POX)</span></span>](external-pox.md) <br/> |<span data-ttu-id="5965d-132">組織のネットワーク外部から Exchange に接続するクライアントを使用する Url のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-132">Contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span>  <br/> |
|[<span data-ttu-id="5965d-133">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-133">TTL (POX)</span></span>](ttl-pox.md) <br/> |<span data-ttu-id="5965d-134">時間、期間の設定が有効なままで、Live までの時間を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-134">Specifies the Time to Live, in hours, during which the settings remain valid.</span></span>  <br/> |
|[<span data-ttu-id="5965d-135">サーバー (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-135">Server (POX)</span></span>](server-pox.md) <br/> |<span data-ttu-id="5965d-136">メール サーバーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-136">Specifies the name of the mail server.</span></span>  <br/> |
|[<span data-ttu-id="5965d-137">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-137">ServerDN (POX)</span></span>](serverdn-pox.md) <br/> |<span data-ttu-id="5965d-138">Exchange Server の識別名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-138">Specifies the Exchange Server distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="5965d-139">ServerVersion (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-139">ServerVersion (POX)</span></span>](serverversion-pox.md) <br/> |<span data-ttu-id="5965d-140">Exchange Server のバージョン番号を表します。</span><span class="sxs-lookup"><span data-stu-id="5965d-140">Represents the Exchange Server version number.</span></span>  <br/> |
|[<span data-ttu-id="5965d-141">MdbDN (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-141">MdbDN (POX)</span></span>](mdbdn-pox.md) <br/> |<span data-ttu-id="5965d-142">メールボックス データベースの識別名を表します。</span><span class="sxs-lookup"><span data-stu-id="5965d-142">Represents the distinguished name of the mailbox database.</span></span>  <br/> |
|[<span data-ttu-id="5965d-143">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-143">PublicFolderServer (POX)</span></span>](publicfolderserver-pox.md) <br/> |<span data-ttu-id="5965d-144">ユーザーのパブリック フォルダー サーバーの完全修飾ドメイン名 (FQDN) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-144">Contains the fully-qualified domain name (FQDN) of the public folder server for the user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-145">ポート (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-145">Port (POX)</span></span>](port-pox.md) <br/> |<span data-ttu-id="5965d-146">ストアへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-146">Specifies the port that is used to connect to the store.</span></span>  <br/> |
|[<span data-ttu-id="5965d-147">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-147">DirectoryPort (POX)</span></span>](directoryport-pox.md) <br/> |<span data-ttu-id="5965d-148">ネーム サービス プロバイダー インターフェイス (NSPI) プロトコルを使用すると、ディレクトリへの接続に使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-148">Specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span>  <br/> |
|[<span data-ttu-id="5965d-149">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-149">ReferralPort (POX)</span></span>](referralport-pox.md) <br/> |<span data-ttu-id="5965d-150">ディレクトリへの参照を取得するために使用されるポートを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-150">Specifies the port that is used to get a referral to a directory.</span></span>  <br/> |
|[<span data-ttu-id="5965d-151">ASUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-151">ASUrl (POX)</span></span>](asurl-pox.md) <br/> |<span data-ttu-id="5965d-152">メールが有効なユーザーの Exchange Web サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-152">Specifies the URL of the best instance of the Exchange Web Services for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-153">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-153">EwsUrl (POX)</span></span>](ewsurl-pox.md) <br/> |<span data-ttu-id="5965d-154">メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-154">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-155">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-155">EmwsUrl (POX)</span></span>](emwsurl-pox.md) <br/> |<span data-ttu-id="5965d-156">メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-156">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-157">SharingUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-157">SharingUrl (POX)</span></span>](sharingurl-pox.md) <br/> |<span data-ttu-id="5965d-158">組織間の予定表と連絡先の共有に使用する共有サーバーの URL が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-158">Contains the URL of the sharing server used for cross-organization sharing of calendars and contacts.</span></span>  <br/> |
|[<span data-ttu-id="5965d-159">EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-159">EcpUrl (POX)</span></span>](ecpurl-pox.md) <br/> |<span data-ttu-id="5965d-160">メールが有効なユーザーの Exchange コントロール パネルの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-160">Specifies the URL of the Exchange Control Panel for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-161">EcpUrl-um (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-161">EcpUrl-um (POX)</span></span>](ecpurl-um-pox.md) <br/> |<span data-ttu-id="5965d-162">メールが有効なユーザーのボイス メールの設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-162">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access voice mail settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-163">EcpUrl-aggr (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-163">EcpUrl-aggr (POX)</span></span>](ecpurl-aggr-pox.md) <br/> |<span data-ttu-id="5965d-164">メールが有効なユーザーの e メールの集計の設定へのアクセスに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-164">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email aggregation settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-165">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-165">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md) <br/> |<span data-ttu-id="5965d-166">メールが有効なユーザーの設定を追跡する電子メール メッセージにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-166">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-167">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-167">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md) <br/> |<span data-ttu-id="5965d-168">メールが有効なユーザーの保持タグの設定にアクセスするために使用する URL を生成するのには[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-168">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-169">EcpUrl sms (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-169">EcpUrl-sms (POX)</span></span>](ecpurl-sms-pox.md) <br/> |<span data-ttu-id="5965d-170">メールが有効なユーザーのショート メッセージ サービス (SMS) の設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-170">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access Short Message Service (SMS) settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-171">(POX) を EcpUrl 発行</span><span class="sxs-lookup"><span data-stu-id="5965d-171">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md) <br/> |<span data-ttu-id="5965d-172">メールが有効なユーザーの予定表の公開設定にアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-172">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-173">(POX) の EcpUrl の写真</span><span class="sxs-lookup"><span data-stu-id="5965d-173">EcpUrl-photo (POX)</span></span>](ecpurl-photo-pox.md) <br/> |<span data-ttu-id="5965d-174">表示またはメールが有効なユーザーの現在の写真を変更するために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-174">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change a mail-enabled user's current photo.</span></span>  <br/> |
|[<span data-ttu-id="5965d-175">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-175">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md) <br/> |<span data-ttu-id="5965d-176">先のすべてのサイトのメールボックスのメールが有効なユーザーは、現在メンバー リストにアクセスするために使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-176">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span>  <br/> |
|[<span data-ttu-id="5965d-177">EcpUrl-tmCreating (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-177">EcpUrl-tmCreating (POX)</span></span>](ecpurl-tmcreating-pox.md) <br/> |<span data-ttu-id="5965d-178">サイトの新しいメールボックスを作成するのに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-178">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to create a new site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5965d-179">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-179">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md) <br/> |<span data-ttu-id="5965d-180">サイトのメールボックスからユーザーの購読を解除するために使用する URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-180">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5965d-181">EcpUrl-tmEditing (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-181">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md) <br/> |<span data-ttu-id="5965d-182">サイトの既存のメールボックスの編集に使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-182">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5965d-183">EcpUrl-extinstall (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-183">EcpUrl-extinstall (POX)</span></span>](ecpurl-extinstall-pox.md) <br/> |<span data-ttu-id="5965d-184">表示または変更するユーザーのメールボックスに現在インストールされているメール ・ アプリケーションに使用できる URL を生成する[EcpUrl (POX)](ecpurl-pox.md)要素の値と組み合わせて使用できますが、部分的な URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-184">Specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to view or change the mail apps currently installed in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="5965d-185">OOFUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-185">OOFUrl (POX)</span></span>](oofurl-pox.md) <br/> |<span data-ttu-id="5965d-186">メールが有効なユーザーの可用性サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-186">Specifies the URL of the best instance of the Availability service for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-187">OABUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-187">OABUrl (POX)</span></span>](oaburl-pox.md) <br/> |<span data-ttu-id="5965d-188">Exchange トポロジの場合、オフライン アドレス帳の構成サーバーの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-188">Specifies the Offline Address Book configuration server URL for an Exchange topology.</span></span>  <br/> |
|[<span data-ttu-id="5965d-189">UMUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-189">UMUrl (POX)</span></span>](umurl-pox.md) <br/> |<span data-ttu-id="5965d-190">メールが有効なユーザーのユニファイド メッセージングの Web サービスの最適なインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-190">Specifies the URL of the best instance of the Unified Messaging Web service for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-191">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-191">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md) <br/> |<span data-ttu-id="5965d-192">メールが有効なユーザーの Exchange Web サービス (EWS) の最適なエンドポイントのインスタンスの URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-192">Specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span>  <br/> |
|[<span data-ttu-id="5965d-193">LoginName (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-193">LoginName (POX)</span></span>](loginname-pox.md) <br/> |<span data-ttu-id="5965d-194">ユーザーのログオン名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-194">Specifies the user's logon name.</span></span>  <br/> |
|[<span data-ttu-id="5965d-195">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-195">DomainRequired (POX)</span></span>](domainrequired-pox.md) <br/> |<span data-ttu-id="5965d-196">ドメインが認証に必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5965d-196">Indicates whether the domain is required for authentication.</span></span>  <br/> |
|[<span data-ttu-id="5965d-197">ドメイン名 (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-197">DomainName (POX)</span></span>](domainname-pox.md) <br/> |<span data-ttu-id="5965d-198">ユーザーのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-198">Specifies the user's domain.</span></span>  <br/> |
|[<span data-ttu-id="5965d-199">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-199">SPA (POX)</span></span>](spa-pox.md) <br/> |<span data-ttu-id="5965d-200">セキュリティで保護されたパスワード認証が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5965d-200">Indicates whether secure password authentication is required.</span></span>  <br/> |
|[<span data-ttu-id="5965d-201">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-201">AuthPackage (POX)</span></span>](authpackage-pox.md) <br/> |<span data-ttu-id="5965d-202">メールボックス サーバーの役割がインストールされている Exchange 2007 コンピューターに対して認証するときに使用される認証スキームを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-202">Specifies the authentication scheme that is used when authenticating against the Exchange 2007 computer that has the Mailbox server role installed.</span></span>  <br/> |
|[<span data-ttu-id="5965d-203">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-203">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md) <br/> |<span data-ttu-id="5965d-204">SSL を使用して Microsoft Exchange 組織に接続するために必要な Secure Sockets Layer (SSL) 証明書のプリンシパル名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-204">Specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>  <br/> |
|[<span data-ttu-id="5965d-205">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-205">SSL (POX)</span></span>](ssl-pox.md) <br/> |<span data-ttu-id="5965d-206">セキュリティで保護されたログオンが必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-206">Specifies whether secure logon is needed.</span></span>  <br/> |
|[<span data-ttu-id="5965d-207">AuthRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-207">AuthRequired (POX)</span></span>](authrequired-pox.md) <br/> |<span data-ttu-id="5965d-208">認証が必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-208">Specifies whether authentication is required.</span></span>  <br/> |
|[<span data-ttu-id="5965d-209">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-209">UsePOPAuth (POX)</span></span>](usepopauth-pox.md) <br/> |<span data-ttu-id="5965d-210">POP3 アカウントの種類の指定された認証情報は、簡易メール転送プロトコル (SMTP) を使用してもかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5965d-210">Indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span>  <br/> |
|[<span data-ttu-id="5965d-211">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-211">SMTPLast (POX)</span></span>](smtplast-pox.md) <br/> |<span data-ttu-id="5965d-212">SMTP サーバーの SMTP サーバーを使用して電子メールを送信する前に電子メールをダウンロードすることが必要かどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-212">Specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="5965d-213">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-213">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md) <br/> |<span data-ttu-id="5965d-214">使用してクライアント コンピューターがネットワーク サーバーに接続するインターネット サービス プロバイダーの要件を満たしているかどうかを決定する基準が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-214">Contains the criteria that are used to determine whether the client computer is on a network that meets the Internet Service Provider's requirements to connect to the server.</span></span>  <br/> |
|[<span data-ttu-id="5965d-215">アドレス帳 (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-215">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="5965d-216">MAPI または HTTP プロトコルを使用してアドレス帳のサーバーにクライアントを接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-216">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="5965d-217">**プロトコル**要素の**Type**属性が存在し、設定の場合でこの要素があるだけに"mapiHttp"です。</span><span class="sxs-lookup"><span data-stu-id="5965d-217">This element is only present if the **Type** attribute on the **Protocol** element is present and set to "mapiHttp".</span></span> <span data-ttu-id="5965d-218">**アドレス帳**の要素は、MAPI または HTTP プロトコルと Exchange Online のターゲットと 15.00.0847.032 以降の Exchange のバージョンを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5965d-218">The **AddressBook** element is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online and versions of Exchange starting with 15.00.0847.032.</span></span>  <br/> |
|[<span data-ttu-id="5965d-219">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-219">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="5965d-220">MAPI または HTTP プロトコルを使用してクライアントをユーザーのメールボックスに接続するための仕様が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5965d-220">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="5965d-221">**プロトコル**要素の**Type**属性が存在し、設定の場合でこの要素があるだけに"mapiHttp"です。</span><span class="sxs-lookup"><span data-stu-id="5965d-221">This element is only present if the **Type** attribute on the **Protocol** element is present and set to "mapiHttp".</span></span> <span data-ttu-id="5965d-222">**MailStore**要素は、MAPI または HTTP プロトコルと Exchange Online のターゲットと 15.00.0847.032 以降の Exchange のバージョンを実装するクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5965d-222">The **MailStore** element is applicable to clients that implement the MAPI/HTTP protocol and target Exchange Online and versions of Exchange starting with 15.00.0847.032.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5965d-223">親要素</span><span class="sxs-lookup"><span data-stu-id="5965d-223">Parent elements</span></span>

|<span data-ttu-id="5965d-224">**要素**</span><span class="sxs-lookup"><span data-stu-id="5965d-224">**Element**</span></span>|<span data-ttu-id="5965d-225">**説明**</span><span class="sxs-lookup"><span data-stu-id="5965d-225">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5965d-226">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="5965d-226">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="5965d-227">ユーザーのアカウントの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="5965d-227">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5965d-228">備考</span><span class="sxs-lookup"><span data-stu-id="5965d-228">Remarks</span></span>

<span data-ttu-id="5965d-229">**プロトコル**要素は、**設定**と同じである[アクション (POX)](action-pox.md)の値を持つ応答に存在します。</span><span class="sxs-lookup"><span data-stu-id="5965d-229">The **Protocol** element is present in a response that has an [Action (POX)](action-pox.md) value that is equal to **settings**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5965d-230">関連項目</span><span class="sxs-lookup"><span data-stu-id="5965d-230">See also</span></span>



[<span data-ttu-id="5965d-231">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5965d-231">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

