---
title: EWS アプリケーションの種類
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ca4e8b90-d0d8-4d55-aa92-19e21659d4f5
description: Exchange の EWS を使用して作成できる、最も一般的な種類のアプリケーションについて説明します。
ms.openlocfilehash: 1ce739f453ba1bc6f1b5d38edae3776daa562ffb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758885"
---
# <a name="ews-application-types"></a><span data-ttu-id="5850c-103">EWS アプリケーションの種類</span><span class="sxs-lookup"><span data-stu-id="5850c-103">EWS application types</span></span>

<span data-ttu-id="5850c-104">Exchange の EWS を使用して作成できる、最も一般的な種類のアプリケーションについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5850c-104">Find out about the most common types of applications that you can create by using EWS in Exchange.</span></span>
  
<span data-ttu-id="5850c-105">[EWS および Exchange のアーキテクチャ](ews-applications-and-the-exchange-architecture.md) は一貫した開発モデルを提供します。この開発モデルを使用して、最も一般的な種類のアプリケーションを一貫した方法で作成できます。これらのアプリケーションには、以下が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5850c-105">The [EWS and Exchange architecture](ews-applications-and-the-exchange-architecture.md) provides a uniform development model that you can use to create the most common types of applications in a consistent way, including the following:</span></span> 
  
- <span data-ttu-id="5850c-106">[クライアント アプリケーション](#bk_clientapps) — EWS を使用して Exchange データにアクセスするスタンドアロン アプリケーション。</span><span class="sxs-lookup"><span data-stu-id="5850c-106">[Client applications](#bk_clientapps) — Standalone applications that use EWS to access Exchange data. Outlook and Outlook Web App are examples of client applications.</span></span> <span data-ttu-id="5850c-107">Outlook および Outlook Web App は、クライアント アプリケーションの例です。</span><span class="sxs-lookup"><span data-stu-id="5850c-107">Client applications — Standalone applications that use EWS to access Exchange data. Outlook and Outlook Web App are examples of client applications.</span></span> 
    
- <span data-ttu-id="5850c-108">[ポータル アプリケーション](#bk_portalapps) — 空き時間情報や連絡先情報など、Exchange から受け取った情報を含めることによって既存の Web ページを拡張するアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="5850c-108">[Portal applications](#bk_portalapps) — Applications that extend an existing web page by including information retrieved from Exchange, such as free/busy or contact information. A SharePoint web part that retrieves Exchange data is an example of a portal application.</span></span> <span data-ttu-id="5850c-109">Exchange データを取得する、SharePoint Web パーツは、ポータル アプリケーションの例です。</span><span class="sxs-lookup"><span data-stu-id="5850c-109">A SharePoint web part that retrieves Exchange data is an example of a portal application.</span></span> 
    
- <span data-ttu-id="5850c-110">[サービス アプリケーション](#bk_serviceapps) — Exchange からのデータを既存のシステムに組み入れるまたは同期させるために使用されるバックグラウンド ジョブ。</span><span class="sxs-lookup"><span data-stu-id="5850c-110">[Service applications](#bk_serviceapps) — Background jobs used to integrate or synchronize data from Exchange into an existing system. For example, an application that synchronizes contact information from Exchange into a CRM application.</span></span> <span data-ttu-id="5850c-111">たとえば、Exchange からの連絡先情報を CRM アプリケーションに同期させるアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="5850c-111">Service applications — Background jobs used to integrate or synchronize data from Exchange into an existing system. For example, an application that synchronizes contact information from Exchange into a CRM application.</span></span> 
    
<span data-ttu-id="5850c-112">これらのアプリケーション モデルはそれぞれ、共通コード ベースを使用して Exchange から情報を取得できます。したがって、情報を取得するために使用される EWS コードをクライアント アプリケーション、ポータル アプリケーション、またはサービス アプリケーションの間で変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="5850c-112">Each of these application models can use a common code base to retrieve information from Exchange – so you don't need to change the EWS code used to retrieve item information between a client, portal, or service application. What might change from one application to the next is the mailbox access and authentication mechanism. For example, client applications commonly use direct user access and basic or NTLM authentication, whereas a service application likely uses impersonation for mailbox access and OAuth authentication.</span></span> <span data-ttu-id="5850c-113">あるアプリケーションと次のアプリケーションで変わる可能性があるのは、メールボックス アクセスと認証メカニズムです。</span><span class="sxs-lookup"><span data-stu-id="5850c-113">What might change from one application to the next is the mailbox access and authentication mechanism.</span></span> <span data-ttu-id="5850c-114">たとえば、クライアント アプリケーションは一般に、直接ユーザー アクセスと基本認証または NTLM 認証を使用するのに対して、サービス アプリケーションはメールボックス アクセスと OAuth 認証に偽装を使用する傾向があります。</span><span class="sxs-lookup"><span data-stu-id="5850c-114">For example, client applications commonly use direct user access and basic or NTLM authentication, whereas a service application likely uses impersonation for mailbox access and OAuth authentication.</span></span>
  
## <a name="client-applications"></a><span data-ttu-id="5850c-115">クライアント アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5850c-115">Client applications</span></span>
<span data-ttu-id="5850c-116"><a name="bk_clientapps"> </a></span><span class="sxs-lookup"><span data-stu-id="5850c-116"></span></span>

<span data-ttu-id="5850c-p105">EWS クライアント アプリケーションは、EWS を使用して Exchange ストアから情報を取得するスタンドアロン アプリケーションです。EWS クライアント アプリケーションは、直接クライアント アクセスまたは代理人アクセスを使用して、メールボックス ストアからデータを取得します。EWS を使用するクライアント アプリケーションの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5850c-p105">An EWS client application is any standalone application that uses EWS to retrieve information from the Exchange store. EWS client applications use direct client access or delegate access to retrieve data from the mailbox store. The following are some examples of client applications that use EWS:</span></span>
  
- <span data-ttu-id="5850c-120">Outlook (メール ヒント、可用性、ユーザー不在時状態などの機能の中)</span><span class="sxs-lookup"><span data-stu-id="5850c-120">Outlook, in features such as MailTips, availability, and user OOF status</span></span>
    
- <span data-ttu-id="5850c-121">デバイス用 OWA</span><span class="sxs-lookup"><span data-stu-id="5850c-121">OWA for Devices</span></span>
    
- <span data-ttu-id="5850c-122">Outlook for Mac 2011</span><span class="sxs-lookup"><span data-stu-id="5850c-122">Outlook for Mac 2011</span></span>
    
- <span data-ttu-id="5850c-123">Lync (空き時間情報用)</span><span class="sxs-lookup"><span data-stu-id="5850c-123">Lync, for availability information</span></span>
    
<span data-ttu-id="5850c-124">クライアント アプリケーションは一般に、直接アクセスと基本認証または NTLM 認証を使用します。そのためユーザーは、自分のログオン資格情報を使用して自分のメールボックス内の情報にしかアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="5850c-124">Client applications commonly use direct access and basic or NTLM authentication, so that users are limited to accessing information in their own mailbox with their own logon credentials. Client applications should also support delegate access for users who have been given permission to access another user’s mailbox.</span></span> <span data-ttu-id="5850c-125">クライアント アプリケーションは、別のユーザーのメールボックスにアクセスする権限が与えられているユーザーの代理人アクセスもサポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5850c-125">Client applications should also support delegate access for users who have been given permission to access another user's mailbox.</span></span>
  
## <a name="portal-applications"></a><span data-ttu-id="5850c-126">ポータル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5850c-126">Portal applications</span></span>
<span data-ttu-id="5850c-127"><a name="bk_portalapps"> </a></span><span class="sxs-lookup"><span data-stu-id="5850c-127"></span></span>

<span data-ttu-id="5850c-p107">ポータル アプリケーションは、既存の Web ページまたはポータルを拡張して、Exchange メールボックス情報をページの個人用コンポーネントとして含めます。SharePoint Web パーツは最も一般的なポータル アプリケーションであり、パーソナライズ エキスペリエンスをユーザーに提供します。そのために、よく表示される SharePoint ポータル ページだけでなく、未読メッセージや最新メッセージ、予定表イベントなど、Exchange メールボックス データのビューを提供します。EWS ポータル アプリケーションは、直接クライアント アクセス、代理人アクセス、または偽装を使用して、メールボックス ストアからデータを取得します。Exchange 2013 と SharePoint 2013 の両方が、サーバー相互認証のための OAuth 認証プロトコルをサポートしているので、OAuth は最もシームレスでセキュリティ保護された認証方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="5850c-p107">A portal application extends an existing web page or portal to include Exchange mailbox information as a personalized component of the page. SharePoint web parts are the most common portal applications and provide users with a personalized experience by providing views into Exchange mailbox data, such as unread messages, most recent messages, and calendar events, alongside their commonly viewed SharePoint portal page. EWS portal applications can use direct client access, delegate access, or impersonation to retrieve data from the mailbox store. Because Exchange 2013 and SharePoint 2013 both support the OAuth authorization protocol for server-to-server authentication, OAuth provides the most seamless and secure authentication method.</span></span>
  
## <a name="service-applications"></a><span data-ttu-id="5850c-132">サービス アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5850c-132">Service applications</span></span>
<span data-ttu-id="5850c-133"><a name="bk_serviceapps"> </a></span><span class="sxs-lookup"><span data-stu-id="5850c-133"></span></span>

<span data-ttu-id="5850c-p108">サービス アプリケーションは通常、既存のアプリケーションに組み込まれるバックグラウンド ジョブであり、Exchange を拡張してシステムと Exchange ストアの間でデータを相互に関連付けます。一般に、サービス アプリケーションにはユーザー インターフェイスがありません。また、サービス アプリケーションは認証とアクセスに偽装または OAuth を使用します。EWS サービス アプリでは、ユーザーを偽装するサービス アカウントを作成することは一般的です。一組のユーザーを偽装する権限を単一のアカウントに付与でき、それらのアカウントに代わってメールボックス操作を実行できるからです。たとえば、EWS サービス アプリケーションは、サービス アカウントと偽装を使用して、CRM ソリューションのマーケティング リストと Exchange 配布グループの間でデータを同期させることができます。</span><span class="sxs-lookup"><span data-stu-id="5850c-p108">A service application is usually a background job built into an existing application that extends to Exchange to correlate data between the system and the Exchange store. Service applications typically do not have a user interface and use impersonation or OAuth for authentication and access. Creating a service account to impersonate users is common in EWS service apps because you can grant a single account permission to impersonate a set of users and perform mailbox operations for those accounts. For example, an EWS service application can synchronize data between marketing lists in a CRM solution and Exchange distribution groups by using a service account and impersonation.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5850c-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5850c-138">See also</span></span>


- [<span data-ttu-id="5850c-139">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="5850c-139">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="5850c-140">EWS アプリケーションと Exchange のアーキテクチャ</span><span class="sxs-lookup"><span data-stu-id="5850c-140">EWS applications and the Exchange architecture</span></span>](ews-applications-and-the-exchange-architecture.md)
    
- [<span data-ttu-id="5850c-141">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="5850c-141">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

