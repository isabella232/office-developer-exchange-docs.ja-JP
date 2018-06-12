---
title: Exchange EWS へのアクセスを制御します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 61e29e54-e3e5-404a-84c0-93b61a25ca58
description: ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。
ms.openlocfilehash: 956c28faba105ecf2a6b1452abe629ea2fc930e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758928"
---
# <a name="control-access-to-ews-in-exchange"></a><span data-ttu-id="653f7-103">Exchange EWS へのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="653f7-103">Control access to EWS in Exchange</span></span>

<span data-ttu-id="653f7-104">ユーザー、アプリケーション、組織全体の EWS へのアクセスを制御する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="653f7-104">Find out how to control access to EWS for users, applications, or the entire organization.</span></span>
  
<span data-ttu-id="653f7-p101">アプリケーション内で EWS マネージ API を使用しているにせよ EWS を直接使用しているにせよ、Exchange Web サービス (EWS) へのアクセスを制御できます。Exchange サーバーへの管理者アクセス権があれば、グローバルにアクセス制御するための Exchange Management Shell を使用して、ユーザーごとおよびアプリケーションごとに、EWS へのアクセスを管理できます。</span><span class="sxs-lookup"><span data-stu-id="653f7-p101">Whether you are using the EWS Managed API, or EWS directly, in your application, you can control access to Exchange Web Services (EWS). If you have administrator access to your Exchange server, you can manage access to EWS by using the Exchange Management Shell to control access globally, for each user, and for each application.</span></span>
  
## <a name="exchange-management-shell-cmdlets-for-configuring-access-control"></a><span data-ttu-id="653f7-107">アクセス制御を構成するための Exchange Management Shell コマンドレット</span><span class="sxs-lookup"><span data-stu-id="653f7-107">Exchange Management Shell cmdlets for configuring access control</span></span>
<span data-ttu-id="653f7-108"><a name="bk_Cmdlets"> </a></span><span class="sxs-lookup"><span data-stu-id="653f7-108"></span></span>

<span data-ttu-id="653f7-109">次の Exchange Management Shell コマンドレットを使用して、現在のアクセス構成を表示し、EWS のアクセス制御を設定できます。</span><span class="sxs-lookup"><span data-stu-id="653f7-109">You can use the following Exchange Management Shell cmdlets to view the current access configuration and set EWS access controls:</span></span>
  
- <span data-ttu-id="653f7-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - はどのようなパラメーターを特定のメールボックスの設定を示しています。</span><span class="sxs-lookup"><span data-stu-id="653f7-110">[Get-CASMailbox](http://technet.microsoft.com/en-us/library/bb124754.aspx) - Shows you what parameters are set for a particular mailbox.</span></span>   
- <span data-ttu-id="653f7-111">[セット-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - 特定のメールボックスのパラメーターを設定します。</span><span class="sxs-lookup"><span data-stu-id="653f7-111">[Set-CASMailbox](http://technet.microsoft.com/en-us/library/bb125264.aspx) - Sets parameters for a particular mailbox.</span></span>    
- <span data-ttu-id="653f7-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - は、組織全体のパラメーターを示しています。</span><span class="sxs-lookup"><span data-stu-id="653f7-112">[Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997571.aspx) - Shows you the parameters for the entire organization.</span></span>    
- <span data-ttu-id="653f7-113">[セット OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx)には、組織全体のパラメーターを設定します。</span><span class="sxs-lookup"><span data-stu-id="653f7-113">[Set-OrganizationConfig](http://technet.microsoft.com/en-us/library/aa997443.aspx) - Sets the parameters for the entire organization.</span></span> 

<span data-ttu-id="653f7-114"><a name="bk_Examples"> </a></span><span class="sxs-lookup"><span data-stu-id="653f7-114"></span></span>

## <a name="examples-controlling-access-to-ews"></a><span data-ttu-id="653f7-115">例</span><span class="sxs-lookup"><span data-stu-id="653f7-115">Examples: Controlling access to EWS</span></span>

<span data-ttu-id="653f7-116">アプリケーションへのアクセスを制御する方法を説明するいくつかのシナリオを見てみましょう。</span><span class="sxs-lookup"><span data-stu-id="653f7-116">Let's take a look at a few scenarios that show you how you can control access to your application.</span></span>
  
<span data-ttu-id="653f7-117">**表 1 です。EWS へのアクセスを制御するためのコマンド**</span><span class="sxs-lookup"><span data-stu-id="653f7-117">**Table 1. Commands for controlling access to EWS**</span></span>

|<span data-ttu-id="653f7-118">目的</span><span class="sxs-lookup"><span data-stu-id="653f7-118">If you want to</span></span> |<span data-ttu-id="653f7-119">このコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="653f7-119">Use this command</span></span>|
|:-----|:-----|
|<span data-ttu-id="653f7-120">EWS を使用しないよう、すべてのクライアント アプリケーションをブロックする。 </span><span class="sxs-lookup"><span data-stu-id="653f7-120">Block all client applications from using EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList`<br/><br/><span data-ttu-id="653f7-p102">これは、AllowList に記載されているアプリケーションの接続を許可します。この例では、AllowList にアプリケーションが含まれていないため、EWS を使用できるアプリケーションはありません。</span><span class="sxs-lookup"><span data-stu-id="653f7-p102">This allows applications listed in the AllowList to connect. In this example, no applications are included in the AllowList, so no applications can use EWS.</span></span> |
|<span data-ttu-id="653f7-123">EWS を使用することを、リストに載っているクライアント アプリケーションに許可する。 </span><span class="sxs-lookup"><span data-stu-id="653f7-123">Allow a list of client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceAllowList -EwsAllowList:"OWA/*"`<br/><br/><span data-ttu-id="653f7-124">これにより、EWS を使用するアプリケーションを特定できます。</span><span class="sxs-lookup"><span data-stu-id="653f7-124">This allows specific applications to use EWS.</span></span> <span data-ttu-id="653f7-125">ユーザー エージェント文字列を任意のアプリケーションが始まり、この例では"OWA と」アクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="653f7-125">In this example, any application that has a user agent string that starts with "OWA/" is allowed access.</span></span> |
|<span data-ttu-id="653f7-126">特にブロックされているものを除き、すべてのクライアント アプリケーションに EWS の使用を許可する。 </span><span class="sxs-lookup"><span data-stu-id="653f7-126">Allow all client applications to use EWS except those that are specifically blocked.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList -EwsBlockList:"OWA/*"`<br/> <br/><span data-ttu-id="653f7-127">次の使用例のみで始まるユーザー エージェント文字列を持っている EWS を使用してからアプリケーションをブロックする"OWA と」。</span><span class="sxs-lookup"><span data-stu-id="653f7-127">This example only blocks applications from using EWS that have a user agent string that starts with "OWA/".</span></span> |
|<span data-ttu-id="653f7-128">すべてのクライアント アプリケーションに EWS の使用を許可する。</span><span class="sxs-lookup"><span data-stu-id="653f7-128">Allow all client applications to use EWS.</span></span> | `Set-OrganizationConfig -EwsApplicationAccessPolicy:EnforceBlockList` <br/><br/> <span data-ttu-id="653f7-129">ブロック リストが指定されていないため、すべてのアプリケーションが EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="653f7-129">Because no BlockList is specified, all applications can use EWS.</span></span> |
|<span data-ttu-id="653f7-130">EWS を使用できないよう、組織全体をブロックする。</span><span class="sxs-lookup"><span data-stu-id="653f7-130">Block the entire organization from using EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$false` |
|<span data-ttu-id="653f7-131">EWS を使用できるよう、組織全体を許可する。</span><span class="sxs-lookup"><span data-stu-id="653f7-131">Allow the entire organization to use EWS.</span></span> | `Set-OrganizationConfig -EwsEnabled:$true`|
|<span data-ttu-id="653f7-132">EWS を使用できないよう、個々のメールボックスをブロックする。</span><span class="sxs-lookup"><span data-stu-id="653f7-132">Block an individual mailbox from using EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$false`|
|<span data-ttu-id="653f7-133">EWS を使用できるよう、個々のメールボックスを許可する。</span><span class="sxs-lookup"><span data-stu-id="653f7-133">Allow an individual mailbox to use EWS.</span></span> | `Set-CASMailbox -Identity adam@contoso.com -EwsEnabled:$true`|
   
## <a name="see-also"></a><span data-ttu-id="653f7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="653f7-134">See also</span></span>

- [<span data-ttu-id="653f7-135">EWS アプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="653f7-135">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)    
- [<span data-ttu-id="653f7-136">Exchange クライアント アプリケーションの EWS へのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="653f7-136">Controlling client application access to EWS in Exchange</span></span>](controlling-client-application-access-to-ews-in-exchange.md)   
- [<span data-ttu-id="653f7-137">Exchange Server PowerShell (Exchange 管理シェル)</span><span class="sxs-lookup"><span data-stu-id="653f7-137">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) 
- [<span data-ttu-id="653f7-138">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="653f7-138">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

