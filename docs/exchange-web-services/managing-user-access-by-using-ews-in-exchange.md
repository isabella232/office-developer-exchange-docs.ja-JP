---
title: Exchange において EWS を使用してユーザー アクセスを管理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。
ms.openlocfilehash: 476292d4db206f22cd84134ce2b46957e9fe85fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456246"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="411f2-103">Exchange において EWS を使用してユーザー アクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="411f2-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="411f2-104">Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。</span><span class="sxs-lookup"><span data-stu-id="411f2-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="411f2-105">Exchange Web サービス (EWS) と EWS マネージ API には、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange 2013 以降の Exchange バージョンでアカウントを管理するために使用できるいくつかの操作があります。</span><span class="sxs-lookup"><span data-stu-id="411f2-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="411f2-106">次の図に示されているこれらの操作を使用すると、デリゲートを管理して、他のアカウントのフォルダー アクセス許可を設定できます。</span><span class="sxs-lookup"><span data-stu-id="411f2-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="411f2-107">**デリゲートおよびフォルダー アクセスのための EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="411f2-107">**EWS operations for delegate and folder access**</span></span>

![EWS ユーザー管理オプション](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="411f2-p102">アプリケーションで、Exchange サーバーにおけるアカウントの制御をさらに必要とする場合は、Exchange 管理シェル コマンドレットを使用してアカウントを管理できます。Exchange 管理シェル コマンドレットは、次のいずれかの方法で呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="411f2-p102">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts. You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="411f2-p103">Exchange 管理シェル コマンドレットを呼び出す C# または Visual Basic を使用してアプリケーションを作成します。[Exchange 管理シェル API ドキュメント](../management/exchange-management-shell.md)に記されているサンプル コードを調べて、コマンドレットの呼び出し方法を確認できます。</span><span class="sxs-lookup"><span data-stu-id="411f2-p103">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets. You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="411f2-113">Windows PowerShell および Windows PowerShell スクリプトを使用して、Exchange 管理シェル コマンドレットを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="411f2-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="411f2-114">
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps) のすべての一覧が、使用法を示す例と共に記載されています。</span><span class="sxs-lookup"><span data-stu-id="411f2-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="411f2-115">関連項目</span><span class="sxs-lookup"><span data-stu-id="411f2-115">See also</span></span>

- [<span data-ttu-id="411f2-116">EWS アプリケーションの設定</span><span class="sxs-lookup"><span data-stu-id="411f2-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- <span data-ttu-id="411f2-117">
  [Exchange 2013 コマンドレット](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="411f2-117">[Exchange 2013 Cmdlets](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)</span></span>  
    

