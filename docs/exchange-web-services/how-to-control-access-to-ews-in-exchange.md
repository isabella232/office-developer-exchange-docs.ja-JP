---
title: Exchange での EWS に対するアクセスの制御
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758928"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="331a3-103">Exchange での EWS に対するアクセスの制御</span><span class="sxs-lookup"><span data-stu-id="331a3-103">How to: Control access to EWS in Exchange</span></span>

<span data-ttu-id="331a3-104">ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="331a3-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="331a3-p101">アプリケーション内で EWS マネージ API を使用しているにせよ EWS を直接使用しているにせよ、Exchange Web サービス (EWS) へのアクセスを制御できます。Exchange サーバーへの管理者アクセス権があれば、グローバルにアクセス制御するための Exchange Management Shell を使用して、ユーザーごとおよびアプリケーションごとに、EWS へのアクセスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="331a3-p101">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS). If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="331a3-107">アクセス制御を構成するための Exchange 管理シェル コマンドレット</span><span class="sxs-lookup"><span data-stu-id="331a3-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="331a3-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="331a3-108"></span></span>

<span data-ttu-id="331a3-109">次の Exchange 管理シェル コマンドレットを使用して、現在のアクセス構成を表示し、EWS のアクセス制御を設定できます。</span><span class="sxs-lookup"><span data-stu-id="331a3-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="331a3-110">[Get-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) - 特定のメールボックスに対して設定されているパラメーターを表示します。</span><span class="sxs-lookup"><span data-stu-id="331a3-110">[Get-CASMailboxhttp://technet.microsoft.com/ja-JP/library/bb124754.aspx](http://technet.microsoft.com/ja-JP/library/bb124754.aspx) – Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="331a3-111">[Set-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb125264.aspx) - 特定のメールボックスのパラメーターを設定します。</span><span class="sxs-lookup"><span data-stu-id="331a3-111">[Set-CASMailbox](http://technet.microsoft.com/ja-JP/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="331a3-112">[Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) - 組織全体のパラメーターを表示します。</span><span class="sxs-lookup"><span data-stu-id="331a3-112">[Get-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="331a3-113">[Set-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997443.aspx) - 組織全体のパラメーターを設定します。</span><span class="sxs-lookup"><span data-stu-id="331a3-113">[Set-OrganizationConfig](http://technet.microsoft.com/ja-JP/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="331a3-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="331a3-114"></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="331a3-115">例: EWS へのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="331a3-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="331a3-116">アプリケーションへのアクセスを制御する方法を説明するいくつかのシナリオを見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="331a3-116">Let’s take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="331a3-117">**表 1. EWS へのアクセスを制御するためのコマンド**</span><span class="sxs-lookup"><span data-stu-id="331a3-117">**Table 1.  Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="331a3-118">目的</span><span class="sxs-lookup"><span data-stu-id="331a3-118">If you want to</span></span> |<span data-ttu-id="331a3-119">使用するコマンド</span><span class="sxs-lookup"><span data-stu-id="331a3-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="331a3-120">EWS を使用しないよう、すべてのクライアント アプリケーションをブロックする。</span><span class="sxs-lookup"><span data-stu-id="331a3-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="331a3-p102">これは、AllowList に記載されているアプリケーションの接続を許可します。この例では、AllowList にアプリケーションが含まれていないため、EWS を使用できるアプリケーションはありません。</span><span class="sxs-lookup"><span data-stu-id="331a3-p102">This allows applications listed in the AllowList to connect. In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="331a3-123">リストに載っているクライアント アプリケーションに EWS の使用を許可する。</span><span class="sxs-lookup"><span data-stu-id="331a3-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="331a3-124">これは、特定のアプリケーションに対して EWS の使用を許可します。</span><span class="sxs-lookup"><span data-stu-id="331a3-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="331a3-125">この例では、"OWA/" から始まるユーザー エージェント文字列を含むすべてのアプリケーションにアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="331a3-125">This allows specific applications to use EWS. In this example, any application that has a user agent string that starts with “OWA/” is allowed access.</span></span> |
|<span data-ttu-id="331a3-126">明示的にブロックされているものを除き、すべてのクライアント アプリケーションに EWS の使用を許可する。</span><span class="sxs-lookup"><span data-stu-id="331a3-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="331a3-127">この例では、"OWA/" で始まるユーザー エージェント文字列を含むアプリケーションのみをブロックして EWS を使用できないようにします。</span><span class="sxs-lookup"><span data-stu-id="331a3-127">This example only blocks applications from using EWS that have a user agent string that starts with “OWA/”.</span></span> |
|<span data-ttu-id="331a3-128">すべてのクライアント アプリケーションに EWS の使用を許可する。</span><span class="sxs-lookup"><span data-stu-id="331a3-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="331a3-129">ブロック リストが指定されていないため、すべてのアプリケーションが EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="331a3-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="331a3-130">EWS を使用できないよう、組織全体をブロックする。</span><span class="sxs-lookup"><span data-stu-id="331a3-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="331a3-131">EWS を使用できるよう、組織全体を許可する。</span><span class="sxs-lookup"><span data-stu-id="331a3-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="331a3-132">EWS を使用できないよう、個々のメールボックスをブロックする。</span><span class="sxs-lookup"><span data-stu-id="331a3-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="331a3-133">個々のメールボックスに EWS の使用を許可する。</span><span class="sxs-lookup"><span data-stu-id="331a3-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="331a3-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="331a3-134">See also</span></span>

- [<span data-ttu-id="331a3-135">EWS アプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="331a3-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="331a3-136">Exchange で EWS へのクライアント アプリケーションのアクセスを制御する</span><span class="sxs-lookup"><span data-stu-id="331a3-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- <span data-ttu-id="331a3-137">
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="331a3-137">[Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)</span></span> 
- [<span data-ttu-id="331a3-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="331a3-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/ja-JP/library/dd835506%28v=vs.85%29.aspx)
    

