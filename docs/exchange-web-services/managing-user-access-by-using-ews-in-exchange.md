---
title: Exchange において EWS を使用してユーザー アクセスを管理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759089"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a><span data-ttu-id="299a7-103">Exchange において EWS を使用してユーザー アクセスを管理する</span><span class="sxs-lookup"><span data-stu-id="299a7-103">Managing user access by using EWS in Exchange</span></span>

<span data-ttu-id="299a7-104">Exchange サーバーに対するユーザー アカウントのアクセス権を管理するためのオプションについて説明します。</span><span class="sxs-lookup"><span data-stu-id="299a7-104">Find out what your options are for managing user account access to your Exchange server.</span></span>
  
<span data-ttu-id="299a7-105">Exchange Web サービス (EWS) と、EWS のマネージ API Exchange Online、Office 365 の一部として Exchange のオンラインまたは Exchange 2013 で開始する Exchange のバージョンのアカウントを管理するために使用できる操作の数に制限を提供します。</span><span class="sxs-lookup"><span data-stu-id="299a7-105">Exchange Web Services (EWS) and the EWS managed API provide a limited number of operations that you can use to manage accounts on Exchange Online, Exchange Online as part of Office 365, or a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="299a7-106">委任を管理して、他のアカウントのフォルダーのアクセス許可を設定するのには、次の図に示すように操作を使用できます。</span><span class="sxs-lookup"><span data-stu-id="299a7-106">You can use the operations shown in the following figure to manage delegates and to set folder access permissions for other accounts.</span></span> 
  
<span data-ttu-id="299a7-107">**デリゲートおよびフォルダーのアクセスの EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="299a7-107">**EWS operations for delegate and folder access**</span></span>

![EWS ユーザー管理オプション](media/Exchange_ManagingUserAccess_1.png)
  
<span data-ttu-id="299a7-p102">アプリケーションで、Exchange サーバーにおけるアカウントの制御をさらに必要とする場合は、Exchange 管理シェル コマンドレットを使用してアカウントを管理できます。Exchange 管理シェル コマンドレットは、次のいずれかの方法で呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="299a7-p102">If your application needs additional control over the accounts on an Exchange server, you can use Exchange Management Shell cmdlets to manage the accounts. You can call the Exchange Management Shell cmdlets by doing one of the following:</span></span>
  
- <span data-ttu-id="299a7-111">C# または Exchange 管理シェル コマンドレットを呼び出す Visual Basic を使用してアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="299a7-111">Writing an application using C# or Visual Basic that calls the Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="299a7-112">コマンドレットを呼び出す方法については、 [Exchange 管理シェルの API ドキュメント](../management/exchange-management-shell.md)のサンプル コードを見ることができます。</span><span class="sxs-lookup"><span data-stu-id="299a7-112">You can look at the sample code in the [Exchange Management Shell API documentation](../management/exchange-management-shell.md) to learn how to call a cmdlet.</span></span> 
    
- <span data-ttu-id="299a7-113">Exchange 管理シェル コマンドレットを呼び出す Windows PowerShell および Windows PowerShell スクリプトを使用します。</span><span class="sxs-lookup"><span data-stu-id="299a7-113">Using Windows PowerShell and Windows PowerShell scripts to call Exchange Management Shell cmdlets.</span></span> <span data-ttu-id="299a7-114">[PowerShell の Exchange Server (Exchange 管理シェル)](https://docs.microsoft.com/ja-jp/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を使用する方法を示す例との完全な一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="299a7-114">You can find a complete list of the [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/ja-jp/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), along with examples that show how to use them.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="299a7-115">関連項目</span><span class="sxs-lookup"><span data-stu-id="299a7-115">See also</span></span>

- [<span data-ttu-id="299a7-116">EWS アプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="299a7-116">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="299a7-117">Exchange 2013 コマンドレット</span><span class="sxs-lookup"><span data-stu-id="299a7-117">Exchange 2013 Cmdlets</span></span>](https://docs.microsoft.com/ja-jp/powershell/exchange/?view=exchange-ps)  
    

