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
ms.openlocfilehash: e8414460007f333e50c9d596bf977792977b1e4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759190"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="08081-103">Exchange 管理シェル ツールの作成</span><span class="sxs-lookup"><span data-stu-id="08081-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="08081-104">Exchange 用の Exchange 管理シェルのツールの作成を開始するための情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="08081-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="08081-105">**に適用されます:** オンライン交換 |Exchange Server 2013年 |Office 365</span><span class="sxs-lookup"><span data-stu-id="08081-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="08081-p101">Exchange 管理シェルは、Exchange Online、Office 365 の一部としての Exchange Online、Exchange 2013 以降のオンプレミス バージョンの Exchange を管理するため、Windows PowerShell のプラットフォームをベースにした豊富なコマンド セットを提供します。Exchange 管理シェル コマンドを使用して、コマンドを直接実行するか、コマンド スクリプトを使用して、サーバーの管理を自動化できます。</span><span class="sxs-lookup"><span data-stu-id="08081-p101">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013. You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="08081-108">管理者のデスクトップや Web ベースのアプリケーションで実行中の管理アプリケーションなど、ホスト アプリケーションから Exchange 管理シェルコマンドを使用する必要がある場合は、Exchange 管理シェルコマンドレットを Visual Basic または C# アプリケーションから呼び出して、Exchange サーバーを管理できます。</span><span class="sxs-lookup"><span data-stu-id="08081-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="08081-109">Exchange 管理シェル ツールの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="08081-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="08081-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="08081-110"></span></span>

<span data-ttu-id="08081-111">Windows PowerShell のホスト アプリケーションの作成に精通し、アプリケーションから Exchange 管理シェル コマンドレットを呼び出す、または、Exchange を使用して作成できるアプリケーションの種類の例を参照する方法を示す例を参照する場合管理シェルのコマンドレットでは、 [Exchange 管理シェルを使用してメール ユーザーの一覧を取得](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08081-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="08081-112">Exchange 管理シェル コマンドレットは、Windows PowerShell、タスク ・ ベースのコマンド ライン シェルおよびシステム管理専用に設計されているスクリプト言語の拡張機能です。</span><span class="sxs-lookup"><span data-stu-id="08081-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="08081-113">Windows PowerShell は、.NET Framework で、上に構築され、コマンドレット、プロバイダー、およびホスト アプリケーションの開発者は、オブジェクト指向の API が用意されています。</span><span class="sxs-lookup"><span data-stu-id="08081-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="08081-114">Windows PowerShell のプログラミングの詳細については、 [Windows PowerShell SDK](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08081-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="08081-115">Exchange 管理シェル コマンドレットを受け入れるし、オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08081-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="08081-116">Exchange 管理シェル コマンドレットとその入力と出力の種類の一覧を参照してください[Exchange 管理シェル コマンドレットの入力し、出力の種類](exchange-management-shell-cmdlet-input-and-output-types.md)。</span><span class="sxs-lookup"><span data-stu-id="08081-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="08081-117">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="08081-117">In this section</span></span>

- [<span data-ttu-id="08081-118">新規および更新された Exchange 管理シェル コマンドレット</span><span class="sxs-lookup"><span data-stu-id="08081-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="08081-119">Exchange 管理シェル コマンドレットの入力と出力タイプ</span><span class="sxs-lookup"><span data-stu-id="08081-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="08081-120">Exchange 管理シェルを使用してメール ユーザーの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="08081-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="08081-121">Exchange 管理シェル コマンドレットの応答を使用します。</span><span class="sxs-lookup"><span data-stu-id="08081-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="08081-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="08081-122">See also</span></span>

- [<span data-ttu-id="08081-123">Exchange 管理シェルの名前空間</span><span class="sxs-lookup"><span data-stu-id="08081-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="08081-124">Exchange Server PowerShell (Exchange 管理シェル)</span><span class="sxs-lookup"><span data-stu-id="08081-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="08081-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="08081-125">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

