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
ms.openlocfilehash: 1cb0328bdb0eebda0ce4eda929e1bfb21be451f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759196"
---
# <a name="exchange-management-shell"></a><span data-ttu-id="a19c9-103">Exchange 管理シェル</span><span class="sxs-lookup"><span data-stu-id="a19c9-103">Exchange Management Shell</span></span>

<span data-ttu-id="a19c9-104">Exchange 管理シェルを使用して Exchange サーバー管理用のツールを開発する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="a19c9-104">Find information about how to use the Exchange Management Shell to develop tools for Exchange server administration.</span></span>
  
<span data-ttu-id="a19c9-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="a19c9-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="a19c9-106">Exchange 管理シェルでは、Exchange 2013 で始まるコマンドは、Exchange のオンライン、Office 365 の一部として Exchange のオンラインまたは、設置型バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースに豊富なセットを提供します。</span><span class="sxs-lookup"><span data-stu-id="a19c9-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="a19c9-107">Exchange 管理シェルを使用するには 2 種類のツールを作成する: コマンド ライン スクリプトが、Windows PowerShell の環境内で動作し、Exchange 管理シェル コマンドレットを使用して、マネージ インターフェイスを使用するツールです。</span><span class="sxs-lookup"><span data-stu-id="a19c9-107">You can use the Exchange Management Shell to create two kinds of tools: command-line scripts that work within the Windows PowerShell environment, and tools that use the Exchange Management Shell cmdlets through a managed interface.</span></span> <span data-ttu-id="a19c9-108">マネージ アプリケーションを使用すると、Exchange サーバーを管理するのにには、標準の Windows または web ベースの UI を作成します。</span><span class="sxs-lookup"><span data-stu-id="a19c9-108">You can use managed applications to create a standard Windows or web-based UI to administer an Exchange server.</span></span> 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a><span data-ttu-id="a19c9-109">Exchange 管理シェルについて知っておくべき事項</span><span class="sxs-lookup"><span data-stu-id="a19c9-109">What you need to know about the Exchange Management Shell</span></span>

|<span data-ttu-id="a19c9-110">についてわからない場合</span><span class="sxs-lookup"><span data-stu-id="a19c9-110">If you're wondering about</span></span>|<span data-ttu-id="a19c9-111">説明</span><span class="sxs-lookup"><span data-stu-id="a19c9-111">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="a19c9-112">可用性</span><span class="sxs-lookup"><span data-stu-id="a19c9-112">Availability</span></span>  <br/> |<span data-ttu-id="a19c9-113">Exchange 管理シェル コマンドは、Exchange が Exchange 2007 以降のバージョンを実行しているすべてのサーバーにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-113">Exchange Management Shell commands are installed on all servers running versions of Exchange starting with Exchange 2007.</span></span><br/><span data-ttu-id="a19c9-114">クライアント アプリケーションは、Windows PowerShell 2.0 を実行しているすべてのコンピューターに展開できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-114">Client applications can be deployed on any computer running Windows PowerShell 2.0.</span></span><br/> <span data-ttu-id="a19c9-115">シェルへのアクセス方法の詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/ja-jp/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a19c9-115">For information about accessing the shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/ja-jp/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>  <br/> |
|<span data-ttu-id="a19c9-116">言語とツール</span><span class="sxs-lookup"><span data-stu-id="a19c9-116">Languages and tools</span></span>  <br/> |<span data-ttu-id="a19c9-117">任意のテキスト エディターでは、Exchange 管理シェル スクリプトを作成できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-117">You can create Exchange Management Shell scripts in any text editor.</span></span><br/><span data-ttu-id="a19c9-118">Exchange 管理シェルで使用できる Windows PowerShell スクリプトを作成するためには、多くのサード パーティ製ツールのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-118">You can use one of many third-party tools for creating Windows PowerShell scripts that can be used with the Exchange Management Shell.</span></span>  <br/> <span data-ttu-id="a19c9-119">[Exchange 管理シェル オブジェクト モデル](exchange-management-shell-namespaces.md)は、.NET Framework に基づいています。</span><span class="sxs-lookup"><span data-stu-id="a19c9-119">The [Exchange Management Shell object model](exchange-management-shell-namespaces.md) is based on the .NET Framework.</span></span><br/><span data-ttu-id="a19c9-120">Exchange 管理シェル アプリケーションを開発するのに任意の .NET 言語を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-120">You can use any .NET language to develop Exchange Management Shell applications.</span></span>  <br/> |
|<span data-ttu-id="a19c9-121">利用可能なテスト ツールとデバッグ ツール</span><span class="sxs-lookup"><span data-stu-id="a19c9-121">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="a19c9-122">Exchange 管理シェル スクリプトをテストしてデバッグするには、多くのサード パーティ製アプリケーションのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-122">You can use one of many third-party applications to test and debug Exchange Management Shell scripts.</span></span>  <br/> <span data-ttu-id="a19c9-123">管理対象の Exchange 管理シェルのアプリケーションをテストしてデバッグするには、Visual Studio とサードパーティ製のツールを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-123">You can use Visual Studio and third-party tools to test and debug managed Exchange Management Shell applications.</span></span>  <br/> |
|<span data-ttu-id="a19c9-124">サーバー プラットフォームの要件</span><span class="sxs-lookup"><span data-stu-id="a19c9-124">Server platform requirements</span></span>  <br/> |<span data-ttu-id="a19c9-125">Windows PowerShell 2.0 がインストールされているすべての Exchange サーバーで、Exchange 管理シェルを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a19c9-125">You can use the Exchange Management Shell on any Exchange server that has Windows PowerShell 2.0 installed.</span></span>  <br/> |
|<span data-ttu-id="a19c9-126">クライアント プラットフォームの要件</span><span class="sxs-lookup"><span data-stu-id="a19c9-126">Client platform requirements</span></span>  <br/> |<span data-ttu-id="a19c9-127">Exchange 管理シェルのクライアント アプリケーションでは、Windows PowerShell 2.0 が必要です。</span><span class="sxs-lookup"><span data-stu-id="a19c9-127">Exchange Management Shell client applications require Windows PowerShell 2.0.</span></span>  <br/> |
|<span data-ttu-id="a19c9-128">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a19c9-128">Permissions</span></span>  <br/> |<span data-ttu-id="a19c9-129">Exchange 管理シェルを実行しているアプリケーションは、ユーザーがある Exchange ストアの役割に基づくアクセス制御に影響を受けるデータ必要です。</span><span class="sxs-lookup"><span data-stu-id="a19c9-129">Running an Exchange Management Shell application requires that the user have role-based access control rights to the affected data on the Exchange store.</span></span><br/><span data-ttu-id="a19c9-130">役割ベースのアクセス制御の詳細については、[役割ベースのアクセス制御と](http://technet.microsoft.com/ja-jp/library/dd298183.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a19c9-130">For more information about role-based access control, see [Understanding Role Based Access Control](http://technet.microsoft.com/ja-jp/library/dd298183.aspx).</span></span>  <br/> |
   
<span data-ttu-id="a19c9-131">このセクションの記事では、Exchange 管理ツールを作成するための重要な Exchange 管理シェルの機能について説明します。</span><span class="sxs-lookup"><span data-stu-id="a19c9-131">The articles in this section describe Exchange Management Shell features that are important for creating Exchange management tools.</span></span> <span data-ttu-id="a19c9-132">Exchange の管理、計画、構成、または詳細については、 [Exchange](https://docs.microsoft.com/ja-jp/exchange/)サイトを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a19c9-132">For information about planning, configuring, or maintaining Exchange, see the [Exchange](https://docs.microsoft.com/ja-jp/exchange/) site.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="a19c9-133">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="a19c9-133">In this section</span></span>

- [<span data-ttu-id="a19c9-134">Exchange 管理シェルのツールを作成します。</span><span class="sxs-lookup"><span data-stu-id="a19c9-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)
    
- [<span data-ttu-id="a19c9-135">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="a19c9-135">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a><span data-ttu-id="a19c9-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="a19c9-136">See also</span></span>
  
- [<span data-ttu-id="a19c9-137">Windows PowerShell マニュアル</span><span class="sxs-lookup"><span data-stu-id="a19c9-137">Windows PowerShell documentation</span></span>](https://docs.microsoft.com/ja-jp/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [<span data-ttu-id="a19c9-138">PowerShell のスクリプト</span><span class="sxs-lookup"><span data-stu-id="a19c9-138">PowerShell scripting</span></span>](https://docs.microsoft.com/ja-jp/powershell/scripting/powershell-scripting?view=powershell-6)
    

