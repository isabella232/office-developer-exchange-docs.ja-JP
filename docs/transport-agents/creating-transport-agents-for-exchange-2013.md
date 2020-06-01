---
title: Exchange 2013 のトランスポート エージェントの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Exchange 2013 用のカスタムトランスポートエージェントを作成する方法、およびカスタムエージェントを作成するためのシステム要件について説明します。
ms.openlocfilehash: cb1cd180817524fe29a100a48d90444c75a77510
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462375"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="5812b-103">Exchange 2013 のトランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="5812b-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="5812b-104">Exchange 2013 用のカスタムトランスポートエージェントを作成する方法、およびカスタムエージェントを作成するためのシステム要件について説明します。</span><span class="sxs-lookup"><span data-stu-id="5812b-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="5812b-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5812b-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="5812b-106">Exchange Server 2013 には、メッセージの処理に使用できるいくつかのトランスポートエージェントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5812b-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="5812b-107">Exchange に付属しているアセンブリを使用すると、自分の組織のニーズに応じた特定のタスクを実行するための、独自のカスタム エージェントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="5812b-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="5812b-108">たとえば、SmtpReceiveAgent トランスポート エージェントを使用すると、SMTP プロトコルで受信されるメッセージをインターセプトして、そのメッセージを処理することで、あらかじめ書式設定されているテキストが含まれるように本文の書式を変換できます。</span><span class="sxs-lookup"><span data-stu-id="5812b-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="5812b-109">RoutingAgent トランスポート エージェントを使用すると、別のサーバーへのルート上にあるサーバーを通過するメッセージをログに記録できます。</span><span class="sxs-lookup"><span data-stu-id="5812b-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="5812b-110">また、さらに複雑な複数のエージェントを使用する機能を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="5812b-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="5812b-111">たとえば、ウイルス対策エージェントを作成する場合は、SmtpReceiveAgent エージェントと RoutingAgent エージェントを実装できます。</span><span class="sxs-lookup"><span data-stu-id="5812b-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="5812b-112">ネットワーク上に SMTP プロトコルをサポートしないコンポーネントがある場合は、Exchange サーバーと外部コンポーネントとの間の通信を処理するために、DeliveryAgent トランスポート エージェントを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5812b-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="5812b-113">この記事では、独自のトランスポート エージェントを作成するための前提条件と、それに関連するタスクに関する情報を示します。</span><span class="sxs-lookup"><span data-stu-id="5812b-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="5812b-114">特定のトランスポートエージェントを作成する方法については、「 [create a routingagent transport agent For exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)」、「 [Create An smtpreceiveagent Transport agent for exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)」、および「 [exchange 2013 の deliveryagent トランスポートエージェント](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)を作成する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5812b-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="5812b-115">トランスポートエージェントを作成するための前提条件</span><span class="sxs-lookup"><span data-stu-id="5812b-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="5812b-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="5812b-116"><a name="bk_prerequisites"> </a></span></span>

<span data-ttu-id="5812b-117">トランスポートエージェントを実装するために必要な前提条件は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="5812b-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="5812b-118">クライアントアクセスサーバーまたはエッジトランスポートサーバー上のフロントエンドトランスポートサービス、またはメールボックスサーバー上のトランスポートサービスを実行している Exchange 2013 を実行しているコンピューター。</span><span class="sxs-lookup"><span data-stu-id="5812b-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="5812b-119">Exchange 2013 のサーバーの役割アーキテクチャの詳細については、「 [exchange 2013 のトランスポートエージェントの概念](transport-agent-concepts-in-exchange-2013.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5812b-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="5812b-120">トランスポートエージェントクラスの次のアセンブリ。</span><span class="sxs-lookup"><span data-stu-id="5812b-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="5812b-121">Microsoft Exchange. .dll</span><span class="sxs-lookup"><span data-stu-id="5812b-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="5812b-122">その他の. .dll</span><span class="sxs-lookup"><span data-stu-id="5812b-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="5812b-123">Microsoft Exchange. .dll</span><span class="sxs-lookup"><span data-stu-id="5812b-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="5812b-124">.NET Framework 4.5</span><span class="sxs-lookup"><span data-stu-id="5812b-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="5812b-125">また、Visual Studio 2012 をインストールすることもお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5812b-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="5812b-126">トランスポートエージェントを実装するには、Visual Basic .NET または C# を使用します。</span><span class="sxs-lookup"><span data-stu-id="5812b-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="5812b-127">アセンブリの参照</span><span class="sxs-lookup"><span data-stu-id="5812b-127">Referencing the assemblies</span></span>
<span data-ttu-id="5812b-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="5812b-128"><a name="bk_ReferenceAssemblies"> </a></span></span>

<span data-ttu-id="5812b-129">Exchange 2013 には、Exchange トランスポート動作の拡張をサポートするクラスのライブラリが用意されています。</span><span class="sxs-lookup"><span data-stu-id="5812b-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="5812b-130">これらのクラスには、.NET Framework 4.5 が必要です。</span><span class="sxs-lookup"><span data-stu-id="5812b-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="5812b-131">これらのクラスに基づいてトランスポートエージェントを実装するには、Visual Studio 2012 を使用します。</span><span class="sxs-lookup"><span data-stu-id="5812b-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="5812b-132">Exchange 2013 インストーラーは、トランスポートエージェント開発に使用されるアセンブリをインストールし、それらをグローバルアセンブリキャッシュ (GAC) に登録します。</span><span class="sxs-lookup"><span data-stu-id="5812b-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="5812b-133">トランスポートエージェントの実装を開始するには、クラスライブラリプロジェクトで、Transport アセンブリへの参照を作成します。</span><span class="sxs-lookup"><span data-stu-id="5812b-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="5812b-134">トランスポートエージェントの実装</span><span class="sxs-lookup"><span data-stu-id="5812b-134">Implementing a transport agent</span></span>
<span data-ttu-id="5812b-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="5812b-135"><a name="bk_implementationExample"> </a></span></span>

<span data-ttu-id="5812b-136">次の例は、 [Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスから派生するクラスの最低限の実装を示しています。</span><span class="sxs-lookup"><span data-stu-id="5812b-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="5812b-137">同じイベントに対して複数のトランスポートエージェントがインストールされ、登録されている場合は、1つのエージェントがメールアイテムからすべての受信者を削除しても、すべてのエージェントが呼び出されます。</span><span class="sxs-lookup"><span data-stu-id="5812b-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="5812b-138">> 処理不能なエラーや予期しない動作を避けるため、トランスポートエージェントは、メールアイテムの受信者数が0と等しいケースを処理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5812b-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
```cs
using System;
using System.Collections.Generic;
using System.Text;
using Microsoft.Exchange.Data.Transport;
using Microsoft.Exchange.Data.Transport.Smtp;
namespace MyAgents
{
    public sealed class MyAgentFactory : SmtpReceiveAgentFactory
    {
        public override SmtpReceiveAgent CreateAgent(SmtpServer server)
        {
            return new MyAgent();
        }
    }
    public class MyAgent : SmtpReceiveAgent
    {
        public MyAgent()
        {
            this.OnEndOfData += new EndOfDataEventHandler(MyEndOfDataHandler);
        }
        private void MyEndOfDataHandler (ReceiveMessageEventSource source, EndOfDataEventArgs e)
        {
            // The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject += " - this text appended by MyAgent";
        }
    }
}
```

```vb
Imports System
Imports System.Collections.Generic
Imports System.Text
Imports Microsoft.Exchange.Data.Transport
Imports Microsoft.Exchange.Data.Transport.Smtp
Namespace MyAgents
    NotInheritable Class MyAgentFactory
        Inherits SmtpReceiveAgentFactory
        Public Overrides Function CreateAgent(ByVal server as SmtpServer) As SmtpReceiveAgent
            Return New MyAgent
        End Function
    End Class
    Public Class MyAgent
        Inherits SmtpReceiveAgent
        Private Sub MyEndOfDataHandler(ByVal source As ReceiveMessageEventSource, ByVal e As EndOfDataEventArgs) Handles Me.OnEndOfData
            ' The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject &amp;= e.MailItem.Message.Subject + " - this text appended by MyAgent"
        End Sub
    End Class
End Namespace
```

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="5812b-139">エージェントのインストールと有効化</span><span class="sxs-lookup"><span data-stu-id="5812b-139">Installing and enabling an agent</span></span>
<span data-ttu-id="5812b-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="5812b-140"><a name="bk_InstallEnable"> </a></span></span>

<span data-ttu-id="5812b-141">エージェントを DLL にコンパイルした後、開発用 Exchange サーバーにエージェントをインストールして有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5812b-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="5812b-142">Exchange 管理シェルで、エージェントをインストールするには、 [transportagent](https://technet.microsoft.com/library/aa997998.aspx)コマンドレットを使用し、エージェントを有効にするには、 [Enable-transportagent](https://technet.microsoft.com/library/bb124921.aspx)コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="5812b-142">In the Exchange Management Shell, use the [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="5812b-143">Exchange 管理シェルの使用方法については、「 [Exchange Server PowerShell (Exchange Management shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5812b-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="5812b-144">トランスポート エージェントは、受信したすべての電子メール メッセージにフル アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="5812b-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="5812b-145">Exchange 2013 は、トランスポートエージェントの動作を制限しません。</span><span class="sxs-lookup"><span data-stu-id="5812b-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="5812b-146">不安定なトランスポートエージェントまたはセキュリティの欠陥が含まれている場合は、Exchange 2013 の安定性とセキュリティに影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5812b-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="5812b-147">そのため、完全に信頼され、完全にテストされているトランスポートエージェントのみをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5812b-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="5812b-148">エージェントをインストールするために**transportagent**コマンドレットを使用すると、Exchange 管理シェルはアセンブリのロックを保持します。</span><span class="sxs-lookup"><span data-stu-id="5812b-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="5812b-149">アセンブリのロックを解除するには、エージェントのインストールに使用した Exchange 管理シェルのインスタンスを閉じる必要があります。</span><span class="sxs-lookup"><span data-stu-id="5812b-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="5812b-150">ロックを解除するまで、アセンブリを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="5812b-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="5812b-151">次の例は、Exchange 管理シェルを使用して MyAgent という名前のエージェントをインストールして有効にする方法を示しています。 MyAgentFactory という名前の[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)から派生したクラスを使用します。</span><span class="sxs-lookup"><span data-stu-id="5812b-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="5812b-152">この例では、エージェントがインストールされているサーバー上のエージェント MyCustomAgent の名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="5812b-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="5812b-153">次の例は、MyCustomAgent という名前のエージェントを有効にする方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5812b-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="5812b-154">クライアントアクセスサーバー上のフロントエンドトランスポートサービスのトランスポートエージェントを管理するには、コマンドに次の値を追加 `-TransportService FrontEnd` します。</span><span class="sxs-lookup"><span data-stu-id="5812b-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="5812b-155">たとえば、フロントエンドトランスポートサービスのトランスポートエージェントを表示するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="5812b-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="5812b-156">エージェントのインストール、有効化、および管理の詳細については、「 [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5812b-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="5812b-157">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="5812b-157">In this section</span></span>
<span data-ttu-id="5812b-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="5812b-158"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="5812b-159">Exchange 2013 用の RoutingAgent トランスポートエージェントの作成</span><span class="sxs-lookup"><span data-stu-id="5812b-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="5812b-160">Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する</span><span class="sxs-lookup"><span data-stu-id="5812b-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="5812b-161">Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成</span><span class="sxs-lookup"><span data-stu-id="5812b-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="5812b-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="5812b-162">See also</span></span>

- [<span data-ttu-id="5812b-163">Exchange 2013 におけるトランスポート エージェントの概念</span><span class="sxs-lookup"><span data-stu-id="5812b-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="5812b-164">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="5812b-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

