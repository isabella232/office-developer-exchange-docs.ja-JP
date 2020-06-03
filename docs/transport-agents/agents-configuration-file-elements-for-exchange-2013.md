---
title: Exchange 2013 のエージェント構成ファイルの要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: Fetagents および Exchange 2013 の構成ファイルの XML 要素についての情報を参照してください。
ms.openlocfilehash: f19fe8316a78cef668db881e630562d3be8be64a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461570"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="22b7a-103">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="22b7a-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="22b7a-104">Fetagents および Exchange 2013 の構成ファイルの XML 要素についての情報を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22b7a-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="22b7a-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="22b7a-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="22b7a-p101">Exchange サーバーにクライアント アクセス サーバーの役割またはメールボックス サーバーの役割をインストールすると、サーバーにインストールされたエージェントに関する構成情報を格納する XML ファイルがインストーラーによって作成されます。このファイルに直接書き込むことはできません。 </span><span class="sxs-lookup"><span data-stu-id="22b7a-p101">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server. You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="22b7a-108">フロント エンド トランスポート サービスはクライアント アクセス サーバー上で実行し、fetagents.config という名前のファイルに書き込みを行います。トランスポート サービスとメールボックス トランスポート サービスはメールボックス サーバー上で実行し、agents.config という名前のファイルに書き込みを行います。クライアント アクセス サーバーの役割とメールボックス サーバーの役割の両方を備えたコンピューターには、fetagents.config と agents.config の両方のファイルが存在することになります。 </span><span class="sxs-lookup"><span data-stu-id="22b7a-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="22b7a-109">これらのファイルへの書き込みは、Exchange 管理シェルでトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="22b7a-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="22b7a-110">トランスポートエージェントのコマンドレットの詳細については、TechNet の「[メールフローのコマンドレット](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22b7a-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="22b7a-111">クライアントアクセスサーバー上のフロントエンドトランスポートサービスとメールボックスサーバー上のトランスポートサービスを拡張するエージェントを区別するために、トランスポートエージェントのコマンドレットにはトランスポートサービス用に "ハブ"、フロントエンドトランスポートサービスの場合は "フロントエンド" という値を持つ_Transportservice_パラメーターがあります。</span><span class="sxs-lookup"><span data-stu-id="22b7a-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="22b7a-p103">agents.config ファイルまたは fetagents.config ファイルを読み込むことで、サーバー上に 1 つ以上のエージェントが存在するかどうかと、そのエージェントの構成情報を確認できます。このドキュメントでは、agents.config ファイルまたは fetagents.config ファイルの情報を読み取るために使用できるリファレンスを提供します。これらのファイルの形式は、どちらも同じです。このドキュメントでは、これらのファイルへの書き込み方法に関する情報は提供していません。</span><span class="sxs-lookup"><span data-stu-id="22b7a-p103">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server. This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same. This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="22b7a-p104">agents.config ファイルや fetagents.config ファイルへの書き込みにサポートされていない方法を使用すると、トランスポート サービスまたはトランスポート エージェントのどちらか、または両方に障害が発生するなど、予期できない結果を招くことになります。これらのファイルは、どちらも直接書き込んではいけません。これらのファイルへの書き込みは、Exchange 管理シェルのトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="22b7a-p104">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both. Do not write directly to either of these files. The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="22b7a-118">トランスポート エージェント構成ファイルの場所</span><span class="sxs-lookup"><span data-stu-id="22b7a-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="22b7a-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="22b7a-119"><a name="bk_ConfigLoc"> </a></span></span>

<span data-ttu-id="22b7a-120">Exchange 2013 をインストールすると、インストールされているサーバーの役割に応じて、インストーラーによって \TransportRoles\Agents または fetagents という名前の XML ファイルが作成され \<ExchangeInstallFolder\> ます (ここで、 \<ExchangeInstallFolder\> は exchange 2013 をインストールしたフォルダーです)。</span><span class="sxs-lookup"><span data-stu-id="22b7a-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="22b7a-121">クライアントアクセスサーバーの役割をインストールすると、Exchange 2013 は fetagents ファイルを fetagents にコピーします。メールボックスサーバーの役割をインストールすると、Exchange 2013 によってエージェント web.config ファイルが agent.config にコピーされます。Exchange 2013 は、サーバー上のトランスポートエージェント構成を変更するときに、このファイルを読み取りおよび書き込みます。</span><span class="sxs-lookup"><span data-stu-id="22b7a-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="22b7a-122">トランスポート エージェントのインストールの検証</span><span class="sxs-lookup"><span data-stu-id="22b7a-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="22b7a-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="22b7a-123"><a name="bk_verifyinstall"> </a></span></span>

<span data-ttu-id="22b7a-124">.NET Framework が提供する XML 機能を使用すると、XML ファイル (agents.config または fetagents.config) を読み取って検証できます。</span><span class="sxs-lookup"><span data-stu-id="22b7a-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="22b7a-125">トランスポート エージェントのインストールと構成を検証するには、構成ファイルの XML を読み取って、トランスポート エージェントに対応する [agent](agent.md) 要素を見つけます。</span><span class="sxs-lookup"><span data-stu-id="22b7a-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="22b7a-126">特定のトランスポート エージェントの **agent** 要素が存在しない場合、そのトラスポート エージェントはインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="22b7a-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="22b7a-127">トランスポート エージェントがインストールされている場合は、**agent** 要素の属性を読み取ることで、そのエージェントの構成を確認できます。</span><span class="sxs-lookup"><span data-stu-id="22b7a-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="22b7a-128">構成ファイルの要素の階層構造</span><span class="sxs-lookup"><span data-stu-id="22b7a-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="22b7a-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="22b7a-129"><a name="bk_elementref"> </a></span></span>

<span data-ttu-id="22b7a-130">次のコードは、構成 XML ファイルの要素の階層構造を示しています。</span><span class="sxs-lookup"><span data-stu-id="22b7a-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
```XML
<configuration>
    <mexRuntime>
        <monitoring>
            <agentExecution/>
            <messageSnapshot/>
        </monitoring>
        <agentList>
            <agent/>
            <agent/>
            <agent />
        </agentList>
    </mexRuntim>
</configuration>
```

## <a name="in-this-section"></a><span data-ttu-id="22b7a-131">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="22b7a-131">In this section</span></span>
<span data-ttu-id="22b7a-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="22b7a-132"><a name="bk_elementreflist"> </a></span></span>

- [<span data-ttu-id="22b7a-133">agent</span><span class="sxs-lookup"><span data-stu-id="22b7a-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="22b7a-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="22b7a-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="22b7a-135">agentList</span><span class="sxs-lookup"><span data-stu-id="22b7a-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="22b7a-136">構成</span><span class="sxs-lookup"><span data-stu-id="22b7a-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="22b7a-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="22b7a-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="22b7a-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="22b7a-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="22b7a-139">管理</span><span class="sxs-lookup"><span data-stu-id="22b7a-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="22b7a-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="22b7a-140">See also</span></span>

- [<span data-ttu-id="22b7a-141">Exchange のトランスポート エージェント</span><span class="sxs-lookup"><span data-stu-id="22b7a-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="22b7a-142">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="22b7a-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="22b7a-143">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="22b7a-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="22b7a-144">Exchange 2013 のトランスポート エージェントの名前空間</span><span class="sxs-lookup"><span data-stu-id="22b7a-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="22b7a-145">メールフローのコマンドレット</span><span class="sxs-lookup"><span data-stu-id="22b7a-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

