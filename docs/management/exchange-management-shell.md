---
title: Exchange 管理シェル
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。
ms.openlocfilehash: 38e75339a4ad97cf8ff99e1cbe9c01059e157941
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435808"
---
# <a name="exchange-management-shell"></a><span data-ttu-id="e45e1-103">Exchange 管理シェル</span><span class="sxs-lookup"><span data-stu-id="e45e1-103">Exchange Management Shell</span></span>

<span data-ttu-id="e45e1-104">Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e45e1-104">Find information about how to use the Exchange Management Shell to develop tools for Exchange server administration.</span></span>
  
<span data-ttu-id="e45e1-105">**適用対象:** Exchange Online |Exchange Server 2013 |Office 365</span><span class="sxs-lookup"><span data-stu-id="e45e1-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="e45e1-106">Exchange 管理シェルは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースにした豊富なコマンド セットを提供します。</span><span class="sxs-lookup"><span data-stu-id="e45e1-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="e45e1-107">Exchange 管理シェルを使用すると、Windows PowerShell 環境内で動作するコマンドラインスクリプトと、管理インターフェイスを使用して Exchange 管理シェルコマンドレットを使用するツールという2種類のツールを作成できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-107">You can use the Exchange Management Shell to create two kinds of tools: command-line scripts that work within the Windows PowerShell environment, and tools that use the Exchange Management Shell cmdlets through a managed interface.</span></span> <span data-ttu-id="e45e1-108">管理されたアプリケーションを使用して、Exchange サーバーを管理するための標準の Windows または web ベースの UI を作成できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-108">You can use managed applications to create a standard Windows or web-based UI to administer an Exchange server.</span></span> 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a><span data-ttu-id="e45e1-109">Exchange 管理シェルについて知っておくべき事項</span><span class="sxs-lookup"><span data-stu-id="e45e1-109">What you need to know about the Exchange Management Shell</span></span>

|<span data-ttu-id="e45e1-110">ご参考までに</span><span class="sxs-lookup"><span data-stu-id="e45e1-110">If you're wondering about</span></span>|<span data-ttu-id="e45e1-111">説明</span><span class="sxs-lookup"><span data-stu-id="e45e1-111">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="e45e1-112">Availability</span><span class="sxs-lookup"><span data-stu-id="e45e1-112">Availability</span></span>  <br/> |<span data-ttu-id="e45e1-113">Exchange 管理シェル コマンドは、Exchange 2007 以降のバージョンの Exchange を実行しているすべてのサーバーにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-113">Exchange Management Shell commands are installed on all servers running versions of Exchange starting with Exchange 2007.</span></span><br/><span data-ttu-id="e45e1-114">クライアント アプリケーションは、Windows PowerShell 2.0 を実行しているすべてのコンピューターに展開できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-114">Client applications can be deployed on any computer running Windows PowerShell 2.0.</span></span><br/> <span data-ttu-id="e45e1-115">シェルへのアクセスについては、「 [Exchange Server PowerShell (Exchange Management shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e45e1-115">For information about accessing the shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>  <br/> |
|<span data-ttu-id="e45e1-116">言語とツール</span><span class="sxs-lookup"><span data-stu-id="e45e1-116">Languages and tools</span></span>  <br/> |<span data-ttu-id="e45e1-117">Exchange 管理シェル スクリプトは任意のテキスト エディターで作成できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-117">You can create Exchange Management Shell scripts in any text editor.</span></span><br/><span data-ttu-id="e45e1-118">Exchange 管理シェルで使用できる Windows PowerShell スクリプトを作成するために、多くのサード パーティ製ツールのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-118">You can use one of many third-party tools for creating Windows PowerShell scripts that can be used with the Exchange Management Shell.</span></span>  <br/> <span data-ttu-id="e45e1-119">[Exchange 管理シェルのオブジェクト モデル](exchange-management-shell-namespaces.md)は、.NET Framework に基づいています。</span><span class="sxs-lookup"><span data-stu-id="e45e1-119">The [Exchange Management Shell object model](exchange-management-shell-namespaces.md) is based on the .NET Framework.</span></span><br/><span data-ttu-id="e45e1-120">Exchange 管理シェル アプリケーションを開発するために任意の .NET 言語を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-120">You can use any .NET language to develop Exchange Management Shell applications.</span></span>  <br/> |
|<span data-ttu-id="e45e1-121">利用可能なテスト ツールとデバッグ ツール</span><span class="sxs-lookup"><span data-stu-id="e45e1-121">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="e45e1-122">Exchange 管理シェル スクリプトをテストしてデバッグするには、多くのサード パーティ製アプリケーションのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-122">You can use one of many third-party applications to test and debug Exchange Management Shell scripts.</span></span>  <br/> <span data-ttu-id="e45e1-123">管理対象の Exchange 管理シェルのアプリケーションをテストしてデバッグするには、Visual Studio とサードパーティ製のツールを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-123">You can use Visual Studio and third-party tools to test and debug managed Exchange Management Shell applications.</span></span>  <br/> |
|<span data-ttu-id="e45e1-124">サーバー プラットフォームの要件</span><span class="sxs-lookup"><span data-stu-id="e45e1-124">Server platform requirements</span></span>  <br/> |<span data-ttu-id="e45e1-125">Windows PowerShell 2.0 がインストールされているすべての Exchange サーバーで、Exchange 管理シェルを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e45e1-125">You can use the Exchange Management Shell on any Exchange server that has Windows PowerShell 2.0 installed.</span></span>  <br/> |
|<span data-ttu-id="e45e1-126">クライアント プラットフォームの要件</span><span class="sxs-lookup"><span data-stu-id="e45e1-126">Client platform requirements</span></span>  <br/> |<span data-ttu-id="e45e1-127">Exchange 管理シェルのクライアント アプリケーションでは、Windows PowerShell 2.0 が必要です。</span><span class="sxs-lookup"><span data-stu-id="e45e1-127">Exchange Management Shell client applications require Windows PowerShell 2.0.</span></span>  <br/> |
|<span data-ttu-id="e45e1-128">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e45e1-128">Permissions</span></span>  <br/> |<span data-ttu-id="e45e1-129">Exchange 管理シェル アプリケーションを実行するには、ユーザーが Exchange ストアの影響を受けるデータに対する役割ベースのアクセス制御の権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="e45e1-129">Running an Exchange Management Shell application requires that the user have role-based access control rights to the affected data on the Exchange store.</span></span><br/><span data-ttu-id="e45e1-130">役割ベースのアクセス制御の詳細については、「[役割ベース](https://technet.microsoft.com/library/dd298183.aspx)のアクセス制御について」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e45e1-130">For more information about role-based access control, see [Understanding Role Based Access Control](https://technet.microsoft.com/library/dd298183.aspx).</span></span>  <br/> |
   
<span data-ttu-id="e45e1-131">このセクションの記事では、Exchange 管理ツールを作成するための重要な Exchange 管理シェルの機能について説明します。</span><span class="sxs-lookup"><span data-stu-id="e45e1-131">The articles in this section describe Exchange Management Shell features that are important for creating Exchange management tools.</span></span> <span data-ttu-id="e45e1-132">Exchange の計画、構成、または保守の詳細については、「 [exchange](https://docs.microsoft.com/exchange/)サイト」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e45e1-132">For information about planning, configuring, or maintaining Exchange, see the [Exchange](https://docs.microsoft.com/exchange/) site.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e45e1-133">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="e45e1-133">In this section</span></span>

- [<span data-ttu-id="e45e1-134">Exchange 管理シェル ツールの作成</span><span class="sxs-lookup"><span data-stu-id="e45e1-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)
    
- [<span data-ttu-id="e45e1-135">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="e45e1-135">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a><span data-ttu-id="e45e1-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e45e1-136">See also</span></span>
  
- [<span data-ttu-id="e45e1-137">Windows PowerShell ドキュメント</span><span class="sxs-lookup"><span data-stu-id="e45e1-137">Windows PowerShell documentation</span></span>](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [<span data-ttu-id="e45e1-138">PowerShell スクリプト</span><span class="sxs-lookup"><span data-stu-id="e45e1-138">PowerShell scripting</span></span>](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

