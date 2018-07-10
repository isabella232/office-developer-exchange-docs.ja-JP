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
description: Exchange 2013 の agents.config と fetagents.config の構成ファイルの XML 要素についての情報を検索します。
ms.openlocfilehash: dd58c4bc21a968db2ca5b13e0c53f7058b29f233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759236"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a><span data-ttu-id="d1dcd-103">Exchange 2013 のエージェント構成ファイルの要素</span><span class="sxs-lookup"><span data-stu-id="d1dcd-103">Agents configuration file elements for Exchange 2013</span></span>

<span data-ttu-id="d1dcd-104">Exchange 2013 の agents.config と fetagents.config の構成ファイルの XML 要素についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-104">Find information about the XML elements in the agents.config and fetagents.config configuration file in Exchange 2013.</span></span>
  
<span data-ttu-id="d1dcd-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="d1dcd-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="d1dcd-p101">Exchange サーバーにクライアント アクセス サーバーの役割またはメールボックス サーバーの役割をインストールすると、サーバーにインストールされたエージェントに関する構成情報を格納する XML ファイルがインストーラーによって作成されます。このファイルに直接書き込むことはできません。 </span><span class="sxs-lookup"><span data-stu-id="d1dcd-p101">When you install the Client Access or the Mailbox server role on an Exchange server, the installer creates an XML file that contains configuration information about agents that are installed on the server. You cannot write directly to this file.</span></span> 
  
<span data-ttu-id="d1dcd-108">フロント エンド トランスポート サービスはクライアント アクセス サーバー上で実行し、fetagents.config という名前のファイルに書き込みを行います。トランスポート サービスとメールボックス トランスポート サービスはメールボックス サーバー上で実行し、agents.config という名前のファイルに書き込みを行います。クライアント アクセス サーバーの役割とメールボックス サーバーの役割の両方を備えたコンピューターには、fetagents.config と agents.config の両方のファイルが存在することになります。 </span><span class="sxs-lookup"><span data-stu-id="d1dcd-108">The Front End Transport service runs on Client Access servers and writes to a file named fetagents.config. The Transport service and the Mailbox Transport service run on Mailbox servers, and write to a file named agents.config. A computer that has both the Client Access server role and the Mailbox server role will have both a fetagents.config and an agents.config file.</span></span> 
  
<span data-ttu-id="d1dcd-109">これらのファイルへの書き込みをサポートされている唯一の方法は、Exchange 管理シェルでトランスポート エージェントのコマンドレットを使用してです。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-109">The only supported way to write to these files is by using the transport agent cmdlets in the Exchange Management Shell.</span></span> <span data-ttu-id="d1dcd-110">トランスポート エージェントのコマンドレットの詳細については、TechNet の[メール フローのコマンドレット](http://technet.microsoft.com/ja-jp/library/aa998553%28v=exchg.150%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-110">For information about the transport agent cmdlets, see [Mail Flow Cmdlets](http://technet.microsoft.com/ja-jp/library/aa998553%28v=exchg.150%29.aspx) on TechNet.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d1dcd-111">区別するクライアント アクセス サーバーのフロント エンド トランスポート サービスを拡張するためのエージェント メールボックス サーバーのトランスポート サービス、トランスポート エージェントのコマンドレットは、トランスポートの「ハブ」の値を持つ_TransportService_パラメーターを持つサービスとフロント エンド トランスポート サービスの「フロント エンド」です。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-111">To distinguish between agents that extend the Front End Transport service on the Client Access server and the Transport service on the Mailbox server, transport agent cmdlets have a  _TransportService_ parameter with a value of "Hub" for the Transport service and "FrontEnd" for the Front End Transport service.</span></span> 
  
<span data-ttu-id="d1dcd-p103">agents.config ファイルまたは fetagents.config ファイルを読み込むことで、サーバー上に 1 つ以上のエージェントが存在するかどうかと、そのエージェントの構成情報を確認できます。このドキュメントでは、agents.config ファイルまたは fetagents.config ファイルの情報を読み取るために使用できるリファレンスを提供します。これらのファイルの形式は、どちらも同じです。このドキュメントでは、これらのファイルへの書き込み方法に関する情報は提供していません。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-p103">You can read the agents.config or fetagents.config file to determine the presence of and configuration information for one or more agents on the server. This documentation provides a reference that you can use to read the information in either the agents.config file or the fetagents.config. The format for both of these files is the same. This documentation does not provide information about how to write to the files.</span></span>
  
> [!CAUTION]
> <span data-ttu-id="d1dcd-p104">agents.config ファイルや fetagents.config ファイルへの書き込みにサポートされていない方法を使用すると、トランスポート サービスまたはトランスポート エージェントのどちらか、または両方に障害が発生するなど、予期できない結果を招くことになります。これらのファイルは、どちらも直接書き込んではいけません。これらのファイルへの書き込みは、Exchange 管理シェルのトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-p104">Using unsupported methods to write to the agents.config file or fetagents.config can produce unexpected results, including failure of the transport service or transport agents, or both. Do not write directly to either of these files. The only supported method for writing to these files is by using the Exchange Management Shell transport agent cmdlets.</span></span> 
  
## <a name="location-of-the-transport-agent-configuration-files"></a><span data-ttu-id="d1dcd-118">トランスポート エージェント構成ファイルの場所</span><span class="sxs-lookup"><span data-stu-id="d1dcd-118">Location of the transport agent configuration files</span></span>
<span data-ttu-id="d1dcd-119"><a name="bk_ConfigLoc"> </a></span><span class="sxs-lookup"><span data-stu-id="d1dcd-119"></span></span>

<span data-ttu-id="d1dcd-120">インストーラーが agents.config.template か、インストール、サーバーの役割によって、fetagents.config.template という XML ファイルを作成する Exchange 2013 をインストールすると、 \<ExchangeInstallFolder\>\TransportRoles\Agentsフォルダー (位置\<ExchangeInstallFolder\>は、Exchange 2013 をインストールしたフォルダー)。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-120">When you install Exchange 2013, the installer creates an XML file that is named either agents.config.template or fetagents.config.template, depending on the server role installed, in the \<ExchangeInstallFolder\>\TransportRoles\Agents folder (where \<ExchangeInstallFolder\> is the folder in which you installed Exchange 2013).</span></span> <span data-ttu-id="d1dcd-121">クライアント アクセス サーバー ロールをインストールする場合、Exchange 2013 は、fetagents.config に fetagents.config.template ファイルをコピーします。メールボックス サーバーの役割をインストールする場合、Exchange 2013 は agents.config に agents.config.template ファイルをコピーします。Exchange 2013 では、読み取り、サーバー上のトランスポート エージェントの構成を変更するときにこのファイルを書き込みます。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-121">If you install the Client Access server role, Exchange 2013 copies the fetagents.config.template file to fetagents.config. If you install the Mailbox server role, Exchange 2013 copies the agents.config.template file to agents.config. Exchange 2013 reads and writes this file when you change the transport agents configuration on the server.</span></span>
  
## <a name="verifying-a-transport-agent-installation"></a><span data-ttu-id="d1dcd-122">トランスポート エージェントのインストールの検証</span><span class="sxs-lookup"><span data-stu-id="d1dcd-122">Verifying a transport agent installation</span></span>
<span data-ttu-id="d1dcd-123"><a name="bk_verifyinstall"> </a></span><span class="sxs-lookup"><span data-stu-id="d1dcd-123"></span></span>

<span data-ttu-id="d1dcd-124">読み取りおよび、agents.config または fetagents.config の XML ファイルを検証するのには.NET Framework が提供する XML 機能を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-124">You can use the XML capabilities that the .NET Framework provides to read and validate the agents.config or the fetagents.config XML file.</span></span> <span data-ttu-id="d1dcd-125">インストールとトランスポート エージェントの構成を確認するに構成ファイル内の XML の読み取りし、トランスポート エージェントに対応する[エージェント](agent.md)の要素を検索します。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-125">To verify the installation and configuration of a transport agent, read the XML in the configuration file and find the [agent](agent.md) element that corresponds to the transport agent.</span></span> <span data-ttu-id="d1dcd-126">特定のトランスポート エージェントの**エージェント**の要素が存在しない場合は、トランスポート エージェントがインストールされていません。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-126">If an **agent** element for the specific transport agent does not exist, the transport agent is not installed.</span></span> <span data-ttu-id="d1dcd-127">トランスポート エージェントがインストールされている場合は、その構成を決定する**エージェント**の要素の属性を読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-127">If the transport agent is installed, you can read the attributes of the **agent** element to determine its configuration.</span></span> 
  
## <a name="configuration-file-element-hierarchy"></a><span data-ttu-id="d1dcd-128">構成ファイルの要素の階層構造</span><span class="sxs-lookup"><span data-stu-id="d1dcd-128">Configuration file element hierarchy</span></span>
<span data-ttu-id="d1dcd-129"><a name="bk_elementref"> </a></span><span class="sxs-lookup"><span data-stu-id="d1dcd-129"></span></span>

<span data-ttu-id="d1dcd-130">次のコードは、構成 XML ファイルの要素の階層構造を示しています。</span><span class="sxs-lookup"><span data-stu-id="d1dcd-130">The following code shows the element hierarchy in the configuration XML file.</span></span>
  
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

## <a name="in-this-section"></a><span data-ttu-id="d1dcd-131">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="d1dcd-131">In this section</span></span>
<span data-ttu-id="d1dcd-132"><a name="bk_elementreflist"> </a></span><span class="sxs-lookup"><span data-stu-id="d1dcd-132"></span></span>

- [<span data-ttu-id="d1dcd-133">エージェント</span><span class="sxs-lookup"><span data-stu-id="d1dcd-133">agent</span></span>](agent.md)
    
- [<span data-ttu-id="d1dcd-134">agentExecution</span><span class="sxs-lookup"><span data-stu-id="d1dcd-134">agentExecution</span></span>](agentexecution.md)
    
- [<span data-ttu-id="d1dcd-135">agentList</span><span class="sxs-lookup"><span data-stu-id="d1dcd-135">agentList</span></span>](agentlist.md)
    
- [<span data-ttu-id="d1dcd-136">構成</span><span class="sxs-lookup"><span data-stu-id="d1dcd-136">configuration</span></span>](configuration.md)
    
- [<span data-ttu-id="d1dcd-137">messageSnapshot</span><span class="sxs-lookup"><span data-stu-id="d1dcd-137">messageSnapshot</span></span>](messagesnapshot.md)
    
- [<span data-ttu-id="d1dcd-138">mexRuntime</span><span class="sxs-lookup"><span data-stu-id="d1dcd-138">mexRuntime</span></span>](mexruntime.md)
    
- [<span data-ttu-id="d1dcd-139">監視</span><span class="sxs-lookup"><span data-stu-id="d1dcd-139">monitoring</span></span>](monitoring.md)
    
## <a name="see-also"></a><span data-ttu-id="d1dcd-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1dcd-140">See also</span></span>

- [<span data-ttu-id="d1dcd-141">Exchange のトランスポート エージェント</span><span class="sxs-lookup"><span data-stu-id="d1dcd-141">Transport agents in Exchange</span></span>](transport-agents-in-exchange-2013.md)
- [<span data-ttu-id="d1dcd-142">トランスポート エージェントの概念には、Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d1dcd-142">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="d1dcd-143">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="d1dcd-143">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
- [<span data-ttu-id="d1dcd-144">トランスポート エージェントの名前空間では、Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d1dcd-144">Transport agent namespaces in Exchange 2013</span></span>](transport-agent-namespaces-in-exchange-2013.md)
- [<span data-ttu-id="d1dcd-145">メール フローのコマンドレット</span><span class="sxs-lookup"><span data-stu-id="d1dcd-145">Mail Flow Cmdlets</span></span>](https://docs.microsoft.com/ja-jp/powershell/exchange/?view=exchange-ps)
    

