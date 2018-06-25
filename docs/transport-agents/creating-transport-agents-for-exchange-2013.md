---
title: Exchange 2013 のトランスポート エージェントの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Exchange 2013 では、カスタムのトランスポート エージェントおよびカスタム エージェントを作成するためのシステム要件を作成する方法に関する情報を検索します。
ms.openlocfilehash: 6146e37c44441bed1d30d08f71ede255dba26440
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759235"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="06985-103">Exchange 2013 のトランスポート エージェントの作成</span><span class="sxs-lookup"><span data-stu-id="06985-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="06985-104">Exchange 2013 では、カスタムのトランスポート エージェントおよびカスタム エージェントを作成するためのシステム要件を作成する方法に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="06985-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="06985-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="06985-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="06985-106">Exchange Server 2013 には、メッセージを処理するために使用できるいくつかのトランスポート エージェントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="06985-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="06985-107">Exchange に付属しているアセンブリを使用すると、組織のニーズに応じて特定のタスクを実行する独自のカスタム エージェントを作成できます。</span><span class="sxs-lookup"><span data-stu-id="06985-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="06985-108">たとえば、SmtpReceiveAgent のメッセージの本文を書式設定済みテキストが含まれている形式に変換するメッセージの処理、SMTP プロトコル経由で受信したメッセージをインターセプトするトランスポート エージェントを使用できます。</span><span class="sxs-lookup"><span data-stu-id="06985-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="06985-109">RoutingAgent トランスポート エージェントを使用すると、別のサーバーに経路上のサーバーを通過するメッセージをログに記録します。</span><span class="sxs-lookup"><span data-stu-id="06985-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="06985-110">作成することもより複雑な複数のタイプのエージェントの機能を使用します。</span><span class="sxs-lookup"><span data-stu-id="06985-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="06985-111">たとえば、ウイルス対策エージェントを作成するには、SmtpReceiveAgent、RoutingAgent エージェントを実装できます。</span><span class="sxs-lookup"><span data-stu-id="06985-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="06985-112">SMTP プロトコルをサポートしていないネットワーク上にコンポーネントがある場合は、Exchange サーバーと外部コンポーネントとの間の通信を処理するために DeliveryAgent のトランスポート エージェントを使用できます。</span><span class="sxs-lookup"><span data-stu-id="06985-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="06985-113">この資料では、前提条件と、独自のトランスポート エージェントを作成するのに関連するタスクに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="06985-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="06985-114">特定のトランスポート エージェントを作成する方法についてを参照してください[Exchange 2013 RoutingAgent トランスポート エージェントを作成する](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)、 [Exchange 2013 SmtpReceiveAgent トランスポート エージェントの作成](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)、および[DeliveryAgent のトランスポート エージェントを作成するためExchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)。</span><span class="sxs-lookup"><span data-stu-id="06985-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="06985-115">トランスポート エージェントを作成するための前提条件</span><span class="sxs-lookup"><span data-stu-id="06985-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="06985-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="06985-116"></span></span>

<span data-ttu-id="06985-117">次に、トランスポート エージェントを実装するために必要な前提条件を示します。</span><span class="sxs-lookup"><span data-stu-id="06985-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="06985-118">クライアント アクセスまたはエッジ トランスポート サーバー、またはメールボックス サーバー上のトランスポート サービスのフロント エンド トランスポート サービスを実行している Exchange 2013 を実行するコンピューター。</span><span class="sxs-lookup"><span data-stu-id="06985-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="06985-119">サーバー ロール アーキテクチャでは、Exchange 2013 の詳細については、[トランスポート エージェントの概念の Exchange 2013](transport-agent-concepts-in-exchange-2013.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06985-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="06985-120">次に示すトランスポート エージェント クラスのアセンブリ</span><span class="sxs-lookup"><span data-stu-id="06985-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="06985-121">Microsoft.Exchange.Data.dll</span><span class="sxs-lookup"><span data-stu-id="06985-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="06985-122">Microsoft.Exchange.Data.Common.dll</span><span class="sxs-lookup"><span data-stu-id="06985-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="06985-123">Microsoft.Exchange.Transport.dll</span><span class="sxs-lookup"><span data-stu-id="06985-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="06985-124">.NET Framework 4.5</span><span class="sxs-lookup"><span data-stu-id="06985-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="06985-125">また、Visual Studio 2012 をインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="06985-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="06985-126">トランスポート エージェントを実装するには、Visual Basic .NET または C# のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="06985-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="06985-127">アセンブリの参照</span><span class="sxs-lookup"><span data-stu-id="06985-127">Referencing the assemblies</span></span>
<span data-ttu-id="06985-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="06985-128"></span></span>

<span data-ttu-id="06985-129">Exchange 2013 には、Exchange トランスポートの動作の拡張機能をサポートするクラスのライブラリが用意されています。</span><span class="sxs-lookup"><span data-stu-id="06985-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="06985-130">これらのクラスは、.NET Framework 4.5 を必要とします。</span><span class="sxs-lookup"><span data-stu-id="06985-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="06985-131">Visual Studio 2012 を使用してこれらのクラスに基づいたトランスポート エージェントを実装することができます。</span><span class="sxs-lookup"><span data-stu-id="06985-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="06985-132">Exchange 2013 のインストーラーでは、トランスポート エージェントの開発に使用されるアセンブリをインストールし、それらをグローバル アセンブリ キャッシュ (GAC) に登録します。</span><span class="sxs-lookup"><span data-stu-id="06985-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="06985-133">トランスポート エージェントの実装を開始するには、クラス ライブラリ プロジェクトで Microsoft.Exchange.Data.Transport アセンブリへの参照を作成します。</span><span class="sxs-lookup"><span data-stu-id="06985-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="06985-134">トランスポート エージェントの実装 </span><span class="sxs-lookup"><span data-stu-id="06985-134">Implementing a transport agent</span></span>
<span data-ttu-id="06985-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="06985-135"></span></span>

<span data-ttu-id="06985-136">次の例では、 [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) 、 [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスから派生するクラスの最小限の実装を示します。</span><span class="sxs-lookup"><span data-stu-id="06985-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="06985-137">同じイベントに対応するトランスポート エージェントが複数インストールされていて登録されていると、あるエージェントがメール アイテムからすべての受信者を削除したとしても、すべてのエージェントが呼び出されます。 </span><span class="sxs-lookup"><span data-stu-id="06985-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="06985-138">> 未処理のエラーまたは予期しない動作を回避するには、トランスポート エージェントは、メール アイテムの受信者の数がゼロに等しい場合を処理します。</span><span class="sxs-lookup"><span data-stu-id="06985-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
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

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="06985-139">エージェントのインストールと有効化</span><span class="sxs-lookup"><span data-stu-id="06985-139">Installing and enabling an agent</span></span>
<span data-ttu-id="06985-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="06985-140"></span></span>

<span data-ttu-id="06985-141">エージェント、DLL をコンパイルした後は、インストールして開発 Exchange サーバーでエージェントを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="06985-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="06985-142">Exchange 管理シェルでは、[インストール TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx)コマンドレット、エージェントをインストールして、エージェントを有効にする[有効にする TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx)コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="06985-142">In the Exchange Management Shell, use the [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="06985-143">Exchange 管理シェルを使用する方法の詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06985-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="06985-144">トランスポート エージェントでは、発生したすべての電子メール メッセージへのフル アクセスがあります。</span><span class="sxs-lookup"><span data-stu-id="06985-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="06985-145">Exchange 2013 では、トランスポート エージェントの動作は制限されません。</span><span class="sxs-lookup"><span data-stu-id="06985-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="06985-146">安定しているセキュリティ上の欠陥が含まれているトランスポート エージェントは、Exchange 2013 のセキュリティと安定性に影響します。</span><span class="sxs-lookup"><span data-stu-id="06985-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="06985-147">したがってを完全に信頼して、完全にテストされているトランスポート エージェントのみをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="06985-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="06985-148">**インストール TransportAgent**コマンドレットを使用してエージェントをインストールすると、Exchange 管理シェルは、アセンブリのロックを保持します。</span><span class="sxs-lookup"><span data-stu-id="06985-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="06985-149">アセンブリのロックを解除するには、エージェントのインストールに使用した Exchange 管理シェルのインスタンスを閉じる必要があります。</span><span class="sxs-lookup"><span data-stu-id="06985-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="06985-150">ロックが解放されるまで、アセンブリを更新することはできません。</span><span class="sxs-lookup"><span data-stu-id="06985-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="06985-151">次の例では、Exchange 管理シェルを使用してインストールし、という名前の MyAgent を[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)という名前の MyAgents.MyAgentFactory から派生したクラスを使用してエージェントを有効にする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="06985-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="06985-p111">この例では、エージェントがインストールされたサーバーで、エージェントに MyCustomAgent という名前を付けます。次の例は、MyCustomAgent という名前のエージェントを有効化する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="06985-p111">This example names the agent MyCustomAgent on the server on which the agent is installed. The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="06985-154">クライアント アクセス サーバーのフロント エンド トランスポート サービスのトランスポート エージェントを管理するためには、コマンドを次の値を追加: `-TransportService FrontEnd`。</span><span class="sxs-lookup"><span data-stu-id="06985-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="06985-155">など、フロント エンド トランスポート サービスのトランスポート エージェントを表示するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="06985-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="06985-156">インストールの詳細については、有効化、および管理、エージェントは、[トランスポート エージェントの管理](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06985-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="06985-157">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="06985-157">In this section</span></span>
<span data-ttu-id="06985-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="06985-158"></span></span>

- [<span data-ttu-id="06985-159">Exchange 2013 RoutingAgent トランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="06985-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="06985-160">Exchange 2013 SmtpReceiveAgent トランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="06985-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="06985-161">Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。</span><span class="sxs-lookup"><span data-stu-id="06985-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="06985-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="06985-162">See also</span></span>

- [<span data-ttu-id="06985-163">トランスポート エージェントの概念には、Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="06985-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="06985-164">Exchange 2013 のトランスポート エージェントのリファレンス</span><span class="sxs-lookup"><span data-stu-id="06985-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

