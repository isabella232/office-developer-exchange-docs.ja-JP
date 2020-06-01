---
title: Exchange 管理シェル ツールの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Exchange 用の Exchange 管理シェルのツールの作成を開始するための情報を検索します。
ms.openlocfilehash: c6e11fa5b55aa514b12f4f52bc9346ac213d3781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463728"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="1dd81-103">Exchange 管理シェル ツールの作成</span><span class="sxs-lookup"><span data-stu-id="1dd81-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="1dd81-104">Exchange 用の Exchange 管理シェルのツールの作成を開始するための情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="1dd81-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="1dd81-105">**適用対象:** Exchange Online |Exchange Server 2013 |Office 365</span><span class="sxs-lookup"><span data-stu-id="1dd81-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="1dd81-p101">Exchange 管理シェルは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースにした豊富なコマンド セットを提供します。Exchange 管理シェル コマンドを使用して、コマンドを直接実行するか、コマンド スクリプトを使用して、サーバーの管理を自動化できます。</span><span class="sxs-lookup"><span data-stu-id="1dd81-p101">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013. You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="1dd81-108">管理者のデスクトップや Web ベースのアプリケーションで実行中の管理アプリケーションなど、ホスト アプリケーションから Exchange 管理シェルコマンドを使用する必要がある場合は、Exchange 管理シェルコマンドレットを Visual Basic または C# アプリケーションから呼び出して、Exchange サーバーを管理できます。</span><span class="sxs-lookup"><span data-stu-id="1dd81-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="1dd81-109">Exchange 管理シェル ツールの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="1dd81-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="1dd81-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="1dd81-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span></span>

<span data-ttu-id="1dd81-111">Windows PowerShell ホストアプリケーションの作成に精通しており、exchange 管理シェルコマンドレットをアプリケーションから呼び出す方法を示す例や、Exchange 管理シェルコマンドレットを使用して作成できるアプリケーションの種類の例については、「 [Exchange 管理シェルを使用してメールユーザーのリストを取得](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd81-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="1dd81-112">Exchange 管理シェル コマンドレットは、Windows PowerShell の拡張機能で、システム管理専用に設計されているタスクベースのコマンド ライン シェルおよびスクリプト言語です。</span><span class="sxs-lookup"><span data-stu-id="1dd81-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="1dd81-113">Windows PowerShell は、.NET Framework 上に構築され、コマンドレット、プロバイダー、ホスト アプリケーション開発者のためのオブジェクト指向の API を提供します。</span><span class="sxs-lookup"><span data-stu-id="1dd81-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="1dd81-114">Windows PowerShell プログラミングの詳細については、 [Windows POWERSHELL SDK](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd81-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="1dd81-115">Exchange 管理シェル コマンドレットは、オブジェクトを受け入れますし、オブジェクトを戻します。</span><span class="sxs-lookup"><span data-stu-id="1dd81-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="1dd81-116">Exchange 管理シェルのコマンドレットとその入力と出力の種類の一覧については、「 [Exchange Management shell コマンドレットの入力と出力の種類](exchange-management-shell-cmdlet-input-and-output-types.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1dd81-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="1dd81-117">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="1dd81-117">In this section</span></span>

- [<span data-ttu-id="1dd81-118">新規および更新された Exchange 管理シェル コマンドレット</span><span class="sxs-lookup"><span data-stu-id="1dd81-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="1dd81-119">Exchange 管理シェル コマンドレットの入力と出力の種類</span><span class="sxs-lookup"><span data-stu-id="1dd81-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="1dd81-120">Exchange 管理シェルを使用してメールユーザーの一覧を取得する</span><span class="sxs-lookup"><span data-stu-id="1dd81-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="1dd81-121">Exchange 管理シェルコマンドレットの応答を使用する</span><span class="sxs-lookup"><span data-stu-id="1dd81-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="1dd81-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="1dd81-122">See also</span></span>

- [<span data-ttu-id="1dd81-123">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="1dd81-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- <span data-ttu-id="1dd81-124">
  [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="1dd81-124">[Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)</span></span>  
- [<span data-ttu-id="1dd81-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="1dd81-125">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

