---
title: Exchange で EWS へのクライアント アプリケーションのアクセスを制御する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 60ac3f7b-ba8a-4c93-99f7-c27002caff93
description: EWS へのクライアント アプリケーション アクセスを管理するためのオプションについて説明します。
ms.openlocfilehash: 29a640178afc9814a0b2232225ae4307e49afed2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758880"
---
# <a name="controlling-client-application-access-to-ews-in-exchange"></a><span data-ttu-id="6a8bc-103">Exchange で EWS へのクライアント アプリケーションのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="6a8bc-103">Controlling client application access to EWS in Exchange</span></span>

<span data-ttu-id="6a8bc-104">EWS へのクライアント アプリケーション アクセスを管理するためのオプションについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-104">Learn about the options for managing client application access to EWS.</span></span>
  
<span data-ttu-id="6a8bc-p101">作成された EWS クライアント アプリケーションはすべて、EWS 操作を呼び出す前に、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降の バージョンの Exchange へのアクセス権を付与されている必要があります。テスト サーバーまたは運用サーバーの管理者は、Exchange 管理シェルを使用して、すべてのユーザーおよびアプリケーション、個々のユーザー、または個々のアプリケーションの EWS へのアクセスを制限できます。EWS へのアクセス制御は、ドメイン アカウントに基づきます。ローカル セキュリティ機関によって認証された資格情報で接続が行われた場合、サーバーはドメイン アカウントのみが接続できることを示すエラーを返します。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-p101">Any EWS client application that you create must be granted access to Exchange Online, Exchange Online as part of Office 365, or version of Exchange starting with Exchange 2013 before it can call EWS operations. Test or production server administrators can use the Exchange Management Shell to limit access to EWS either for all users and applications, for individual users, or for individual applications. Access control for EWS is based on domain accounts. When a connection is made with credentials that are authenticated by the local security authority, the server returns an error that indicates that only domain accounts can connect.</span></span> 
  
## <a name="access-control-for-ews-clients-and-users"></a><span data-ttu-id="6a8bc-109">EWS クライアントおよびユーザーのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="6a8bc-109">Access control for EWS clients and users</span></span>
<span data-ttu-id="6a8bc-110"><a name="bk_configure"> </a></span><span class="sxs-lookup"><span data-stu-id="6a8bc-110"></span></span>

<span data-ttu-id="6a8bc-111">テスト サーバーまたは運用サーバーの管理者は、次の方法で EWS に接続するクライアントのアクセス制御を構成できます。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-111">Your test or production server administrator can configure access control for clients that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="6a8bc-112">すべてのクライアント アプリケーションの接続をブロックする。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-112">By blocking all client applications from connecting.</span></span>
    
- <span data-ttu-id="6a8bc-113">特定のクライアント アプリケーションの接続のみを許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-113">By allowing specific client applications only to connect.</span></span>
    
- <span data-ttu-id="6a8bc-114">明示的にブロックされているものを除き、すべてのクライアント アプリケーションの接続を許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-114">By allowing any client application to connect except those that are specifically blocked.</span></span>
    
- <span data-ttu-id="6a8bc-115">すべてのクライアント アプリケーションの接続を許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-115">By allowing any client application to connect.</span></span>
    
<span data-ttu-id="6a8bc-116">アプリケーションは、HTTP Web 要求で送信されるユーザー エージェント文字列によって識別されます。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-116">Applications are identified by the user agent string that they send in the HTTP web request.</span></span>
  
> [!アプリケーション レベルのセキュリティに関するメモ]<span data-ttu-id="6a8bc-117"> ブロックは、そのセキュリティ機能ではありません。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-117"> Application-level blocking is not a security feature.</span></span> <span data-ttu-id="6a8bc-118">ユーザー エージェント文字列は容易に偽装します。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-118">The user agent string is easily spoofed.</span></span> <span data-ttu-id="6a8bc-119">アプリケーションには、EWS へのアクセスが許可されている場合、アプリケーションする必要がありますが資格情報を提示するアプリケーションは、EWS を接続する前にサーバーが認証されます。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-119">If an application is allowed access to EWS, the application must still present credentials that the server authenticates before the application can connect to EWS.</span></span> 
  
<span data-ttu-id="6a8bc-120">管理者は、次の方法で EWS に接続するメールボックスの所有者のアクセス制御を構成できます。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-120">Administrators can also configure access control for mailbox owners that connect to EWS in the following ways:</span></span> 
  
- <span data-ttu-id="6a8bc-121">組織全体をブロックまたは、許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-121">By blocking or allowing an entire organization.</span></span>
    
- <span data-ttu-id="6a8bc-122">EWS へのアクセス権を持たないメールボックスの所有者を包含または除外する役割ベースの認証スコープによって識別された、ユーザーのグループをブロック、または許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-122">By blocking or allowing a group of users identified by a role-based authentication scope that includes or excludes mailbox owners that do not have access to EWS.</span></span>
    
- <span data-ttu-id="6a8bc-123">個々のメールボックスの所有者をブロック、または許可する。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-123">By blocking or allowing an individual mailbox owner.</span></span>
    
<span data-ttu-id="6a8bc-p103">特定のアクセス制御の設定は、アクセス制御の全般設定より優先されます。たとえば、組織によって EWS へのアクセスが拒否されている場合でも、個々のメールボックスの所有者がアプリケーションへのアクセスを許可されている場合、個々の設定が優先され、アクセスが許可されます。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-p103">Specific access control settings override general access control settings. For example, if an organization denies EWS access but an individual mailbox owner is allowed application access, the individual setting prevails and access is allowed.</span></span> 
  
## <a name="delegation-and-ews-access-management"></a><span data-ttu-id="6a8bc-126">EWS へのアクセス管理および委任 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-126">Delegation and EWS access management</span></span>
<span data-ttu-id="6a8bc-127"><a name="bk_delegation"> </a></span><span class="sxs-lookup"><span data-stu-id="6a8bc-127"></span></span>

<span data-ttu-id="6a8bc-p104">アクセス権を持たない委任ユーザーがクライアント アプリケーションを使用した場合、プリンシパル ユーザーが EWS へのアクセス権を持っている場合でも、そのユーザーは EWS を使用してプリンシパル ユーザーのメールボックスにアクセスすることはできません。委任ユーザーが EWS へのアクセス権を持っている場合、プリンシパル ユーザーが EWS のアクセス権がなくても、その委任ユーザーは EWS クライアント アプリケーションを使用してプリンシパル ユーザーのメールボックスにアクセスすることができます。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-p104">When delegate users who do not have access to EWS use your client application, they will not be able to access the principal user's mailbox by using EWS, even if the principal user has EWS access. If the delegate user has EWS access, the delegate will be able to use your EWS client application to access the principal user's mailbox even if the principal user does not have EWS access.</span></span> 
  
## <a name="impersonation-and-ews-access-management"></a><span data-ttu-id="6a8bc-130">権限の借用および EWS へのアクセス管理 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-130">Impersonation and EWS access management</span></span>
<span data-ttu-id="6a8bc-131"><a name="bk_impersonation"> </a></span><span class="sxs-lookup"><span data-stu-id="6a8bc-131"></span></span>

<span data-ttu-id="6a8bc-p105">メールボックスの所有者の代わりに EWS に接続するクライアント アプリケーションは、メールボックスの所有者の EWS 設定を使用できない場合があります。たとえば、会社に電子メールをアーカイブするアプリケーションは、メールボックス ユーザーの設定に関係なく EWS に接続する必要があります。メール クライアントなどその他のアプリケーションは、メールボックスの所有者の EWS 設定を使用する必要があります。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-p105">Client applications that connect to EWS on behalf of mailbox owners might not be able to use the EWS settings of the mailbox owner. For example, an application that archives email messages for a company has to connect to EWS regardless of what the mailbox users' settings are. Other applications, such as mail clients, do have to use the mailbox owner's EWS settings.</span></span> 
  
<span data-ttu-id="6a8bc-p106">管理者は、それぞれのサーバー上で使用するアプリケーションやアプリケーション クラスごとに権限借用アカウントを作成する必要があります。これにより管理者は、EWS へのアクセス許可を持たないすべてのユーザーに役割ベースのアクセス制御スコープを構成できます。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-p106">Administrators should create an impersonation account for each application or application class that they use on their server. This will enable the administrator to configure the role-based access control scope for all users that do not have EWS permissions.</span></span> 
  
<span data-ttu-id="6a8bc-137">権限借用アカウントを有効にするには、テストまたは運用サーバー管理者が次のいずれかを実行します。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-137">To enable impersonation accounts, your test or production server administrator should do one of the following:</span></span> 
  
- <span data-ttu-id="6a8bc-138">認証ユーザー グループを Pre-Win2K Compatible Access グループに追加する。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-138">Add the Authenticated Users group to the Pre-Win2K Compatible Access Group.</span></span> 
    
- <span data-ttu-id="6a8bc-139">Exchange Servers グループを Windows Authorization Access グループに追加する。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-139">Add the Exchange Servers group to the Windows Authorization Access group.</span></span> 
    
## <a name="exchange-management-shell-cmdlets-for-access-management"></a><span data-ttu-id="6a8bc-140">アクセス管理のための Exchange 管理シェル コマンドレット </span><span class="sxs-lookup"><span data-stu-id="6a8bc-140">Exchange Management Shell cmdlets for access management</span></span>
<span data-ttu-id="6a8bc-141"><a name="bk_cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="6a8bc-141"></span></span>

<span data-ttu-id="6a8bc-142">管理者は、次の Exchange 管理シェル コマンドレットを使用して EWS のアクセス制御を構成します。 </span><span class="sxs-lookup"><span data-stu-id="6a8bc-142">Administrators use the following Exchange Management Shell cmdlets to configure EWS access controls:</span></span> 
  
- [<span data-ttu-id="6a8bc-143">Get CASMailbox</span><span class="sxs-lookup"><span data-stu-id="6a8bc-143">Get-CASMailbox</span></span>](http://technet.microsoft.com/ja-jp/library/bb124754.aspx)
    
- [<span data-ttu-id="6a8bc-144">セット CASMailbox</span><span class="sxs-lookup"><span data-stu-id="6a8bc-144">Set-CASMailbox</span></span>](http://technet.microsoft.com/ja-jp/library/bb125264.aspx)
    
- [<span data-ttu-id="6a8bc-145">Get OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="6a8bc-145">Get-OrganizationConfig</span></span>](http://technet.microsoft.com/ja-jp/library/aa997571.aspx)
    
- [<span data-ttu-id="6a8bc-146">セット OrganizationConfig</span><span class="sxs-lookup"><span data-stu-id="6a8bc-146">Set-OrganizationConfig</span></span>](http://technet.microsoft.com/ja-jp/library/aa997443.aspx)
    
## <a name="see-also"></a><span data-ttu-id="6a8bc-147">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a8bc-147">See also</span></span>

- [<span data-ttu-id="6a8bc-148">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="6a8bc-148">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)  
- [<span data-ttu-id="6a8bc-149">Exchange EWS へのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="6a8bc-149">Control access to EWS in Exchange</span></span>](how-to-control-access-to-ews-in-exchange.md)
- [<span data-ttu-id="6a8bc-150">Exchange Server PowerShell (Exchange 管理シェル)</span><span class="sxs-lookup"><span data-stu-id="6a8bc-150">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/ja-jp/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
- [<span data-ttu-id="6a8bc-151">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="6a8bc-151">Windows PowerShell</span></span>](http://msdn.microsoft.com/ja-jp/library/dd835506%28v=vs.85%29.aspx)
    

