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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462375"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの作成

Exchange 2013 用のカスタムトランスポートエージェントを作成する方法、およびカスタムエージェントを作成するためのシステム要件について説明します。
  
**製品:** Exchange Server 2013
  
Exchange Server 2013 には、メッセージの処理に使用できるいくつかのトランスポートエージェントが含まれています。 Exchange に付属しているアセンブリを使用すると、自分の組織のニーズに応じた特定のタスクを実行するための、独自のカスタム エージェントを作成できます。 たとえば、SmtpReceiveAgent トランスポート エージェントを使用すると、SMTP プロトコルで受信されるメッセージをインターセプトして、そのメッセージを処理することで、あらかじめ書式設定されているテキストが含まれるように本文の書式を変換できます。 RoutingAgent トランスポート エージェントを使用すると、別のサーバーへのルート上にあるサーバーを通過するメッセージをログに記録できます。 また、さらに複雑な複数のエージェントを使用する機能を作成することもできます。 たとえば、ウイルス対策エージェントを作成する場合は、SmtpReceiveAgent エージェントと RoutingAgent エージェントを実装できます。 ネットワーク上に SMTP プロトコルをサポートしないコンポーネントがある場合は、Exchange サーバーと外部コンポーネントとの間の通信を処理するために、DeliveryAgent トランスポート エージェントを使用できます。 
  
この記事では、独自のトランスポート エージェントを作成するための前提条件と、それに関連するタスクに関する情報を示します。 特定のトランスポートエージェントを作成する方法については、「 [create a routingagent transport agent For exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)」、「 [Create An smtpreceiveagent Transport agent for exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)」、および「 [exchange 2013 の deliveryagent トランスポートエージェント](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)を作成する」を参照してください。
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>トランスポートエージェントを作成するための前提条件
<a name="bk_prerequisites"> </a>

トランスポートエージェントを実装するために必要な前提条件は次のとおりです。
  
- クライアントアクセスサーバーまたはエッジトランスポートサーバー上のフロントエンドトランスポートサービス、またはメールボックスサーバー上のトランスポートサービスを実行している Exchange 2013 を実行しているコンピューター。 Exchange 2013 のサーバーの役割アーキテクチャの詳細については、「 [exchange 2013 のトランスポートエージェントの概念](transport-agent-concepts-in-exchange-2013.md)」を参照してください。
    
- トランスポートエージェントクラスの次のアセンブリ。
    
  - Microsoft Exchange. .dll
    
  - その他の. .dll
    
  - Microsoft Exchange. .dll
    
- .NET Framework 4.5
    
また、Visual Studio 2012 をインストールすることもお勧めします。 トランスポートエージェントを実装するには、Visual Basic .NET または C# を使用します。
  
## <a name="referencing-the-assemblies"></a>アセンブリの参照
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 には、Exchange トランスポート動作の拡張をサポートするクラスのライブラリが用意されています。 これらのクラスには、.NET Framework 4.5 が必要です。 これらのクラスに基づいてトランスポートエージェントを実装するには、Visual Studio 2012 を使用します。
  
Exchange 2013 インストーラーは、トランスポートエージェント開発に使用されるアセンブリをインストールし、それらをグローバルアセンブリキャッシュ (GAC) に登録します。 トランスポートエージェントの実装を開始するには、クラスライブラリプロジェクトで、Transport アセンブリへの参照を作成します。
  
## <a name="implementing-a-transport-agent"></a>トランスポートエージェントの実装
<a name="bk_implementationExample"> </a>

次の例は、 [Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)および[smtpreceiveagent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスから派生するクラスの最低限の実装を示しています。 
  
> [!CAUTION]
> 同じイベントに対して複数のトランスポートエージェントがインストールされ、登録されている場合は、1つのエージェントがメールアイテムからすべての受信者を削除しても、すべてのエージェントが呼び出されます。 > 処理不能なエラーや予期しない動作を避けるため、トランスポートエージェントは、メールアイテムの受信者数が0と等しいケースを処理する必要があります。 
  
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

## <a name="installing-and-enabling-an-agent"></a>エージェントのインストールと有効化
<a name="bk_InstallEnable"> </a>

エージェントを DLL にコンパイルした後、開発用 Exchange サーバーにエージェントをインストールして有効にする必要があります。 Exchange 管理シェルで、エージェントをインストールするには、 [transportagent](https://technet.microsoft.com/library/aa997998.aspx)コマンドレットを使用し、エージェントを有効にするには、 [Enable-transportagent](https://technet.microsoft.com/library/bb124921.aspx)コマンドレットを使用します。 Exchange 管理シェルの使用方法については、「 [Exchange Server PowerShell (Exchange Management shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。
  
> [!CAUTION]
> トランスポート エージェントは、受信したすべての電子メール メッセージにフル アクセスできます。 Exchange 2013 は、トランスポートエージェントの動作を制限しません。 不安定なトランスポートエージェントまたはセキュリティの欠陥が含まれている場合は、Exchange 2013 の安定性とセキュリティに影響を与える可能性があります。 そのため、完全に信頼され、完全にテストされているトランスポートエージェントのみをインストールする必要があります。 
  
エージェントをインストールするために**transportagent**コマンドレットを使用すると、Exchange 管理シェルはアセンブリのロックを保持します。 アセンブリのロックを解除するには、エージェントのインストールに使用した Exchange 管理シェルのインスタンスを閉じる必要があります。 ロックを解除するまで、アセンブリを更新することはできません。 
  
次の例は、Exchange 管理シェルを使用して MyAgent という名前のエージェントをインストールして有効にする方法を示しています。 MyAgentFactory という名前の[Smtpreceiveagentfactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)から派生したクラスを使用します。 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
この例では、エージェントがインストールされているサーバー上のエージェント MyCustomAgent の名前を指定します。 次の例は、MyCustomAgent という名前のエージェントを有効にする方法を示しています。
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
クライアントアクセスサーバー上のフロントエンドトランスポートサービスのトランスポートエージェントを管理するには、コマンドに次の値を追加 `-TransportService FrontEnd` します。 たとえば、フロントエンドトランスポートサービスのトランスポートエージェントを表示するには、次のコマンドを実行します。
  
 `Get-TransportAgent -TransportService FrontEnd`
  
エージェントのインストール、有効化、および管理の詳細については、「 [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)」を参照してください。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 用の RoutingAgent トランスポートエージェントの作成](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Exchange 2013 用の SmtpReceiveAgent トランスポートエージェントを作成する](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Exchange 2013 用の DeliveryAgent トランスポートエージェントの作成](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)   
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
    

