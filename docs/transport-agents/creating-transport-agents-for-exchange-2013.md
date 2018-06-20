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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759235"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの作成

Exchange 2013 では、カスタムのトランスポート エージェントおよびカスタム エージェントを作成するためのシステム要件を作成する方法に関する情報を検索します。
  
**に適用されます:** Exchange Server 2013
  
Exchange Server 2013 には、メッセージを処理するために使用できるいくつかのトランスポート エージェントが含まれています。 Exchange に付属しているアセンブリを使用すると、組織のニーズに応じて特定のタスクを実行する独自のカスタム エージェントを作成できます。 たとえば、SmtpReceiveAgent のメッセージの本文を書式設定済みテキストが含まれている形式に変換するメッセージの処理、SMTP プロトコル経由で受信したメッセージをインターセプトするトランスポート エージェントを使用できます。 RoutingAgent トランスポート エージェントを使用すると、別のサーバーに経路上のサーバーを通過するメッセージをログに記録します。 作成することもより複雑な複数のタイプのエージェントの機能を使用します。 たとえば、ウイルス対策エージェントを作成するには、SmtpReceiveAgent、RoutingAgent エージェントを実装できます。 SMTP プロトコルをサポートしていないネットワーク上にコンポーネントがある場合は、Exchange サーバーと外部コンポーネントとの間の通信を処理するために DeliveryAgent のトランスポート エージェントを使用できます。 
  
この資料では、前提条件と、独自のトランスポート エージェントを作成するのに関連するタスクに関する情報を提供します。 特定のトランスポート エージェントを作成する方法についてを参照してください[Exchange 2013 RoutingAgent トランスポート エージェントを作成する](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)、 [Exchange 2013 SmtpReceiveAgent トランスポート エージェントの作成](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)、および[DeliveryAgent のトランスポート エージェントを作成するためExchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)。
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>トランスポート エージェントを作成するための前提条件
<a name="bk_prerequisites"> </a>

次に、トランスポート エージェントを実装するために必要な前提条件を示します。
  
- クライアント アクセスまたはエッジ トランスポート サーバー、またはメールボックス サーバー上のトランスポート サービスのフロント エンド トランスポート サービスを実行している Exchange 2013 を実行するコンピューター。 サーバー ロール アーキテクチャでは、Exchange 2013 の詳細については、[トランスポート エージェントの概念の Exchange 2013](transport-agent-concepts-in-exchange-2013.md)を参照してください。
    
- 次に示すトランスポート エージェント クラスのアセンブリ
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- .NET Framework 4.5
    
また、Visual Studio 2012 をインストールすることをお勧めします。 トランスポート エージェントを実装するには、Visual Basic .NET または C# のいずれかを使用します。
  
## <a name="referencing-the-assemblies"></a>アセンブリの参照
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 には、Exchange トランスポートの動作の拡張機能をサポートするクラスのライブラリが用意されています。 これらのクラスは、.NET Framework 4.5 を必要とします。 Visual Studio 2012 を使用してこれらのクラスに基づいたトランスポート エージェントを実装することができます。
  
Exchange 2013 のインストーラーでは、トランスポート エージェントの開発に使用されるアセンブリをインストールし、それらをグローバル アセンブリ キャッシュ (GAC) に登録します。 トランスポート エージェントの実装を開始するには、クラス ライブラリ プロジェクトで Microsoft.Exchange.Data.Transport アセンブリへの参照を作成します。
  
## <a name="implementing-a-transport-agent"></a>トランスポート エージェントの実装 
<a name="bk_implementationExample"> </a>

次の例では、 [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) 、 [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)クラスから派生するクラスの最小限の実装を示します。 
  
> [!CAUTION]
> 同じイベントに対応するトランスポート エージェントが複数インストールされていて登録されていると、あるエージェントがメール アイテムからすべての受信者を削除したとしても、すべてのエージェントが呼び出されます。  > 未処理のエラーまたは予期しない動作を回避するには、トランスポート エージェントは、メール アイテムの受信者の数がゼロに等しい場合を処理します。 
  
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

エージェント、DLL をコンパイルした後は、インストールして開発 Exchange サーバーでエージェントを有効にする必要があります。 Exchange 管理シェルでは、[インストール TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx)コマンドレット、エージェントをインストールして、エージェントを有効にする[有効にする TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx)コマンドレットを使用します。 Exchange 管理シェルを使用する方法の詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。
  
> [!CAUTION]
> トランスポート エージェントでは、発生したすべての電子メール メッセージへのフル アクセスがあります。 Exchange 2013 では、トランスポート エージェントの動作は制限されません。 安定しているセキュリティ上の欠陥が含まれているトランスポート エージェントは、Exchange 2013 のセキュリティと安定性に影響します。 したがってを完全に信頼して、完全にテストされているトランスポート エージェントのみをインストールする必要があります。 
  
**インストール TransportAgent**コマンドレットを使用してエージェントをインストールすると、Exchange 管理シェルは、アセンブリのロックを保持します。 アセンブリのロックを解除するには、エージェントのインストールに使用した Exchange 管理シェルのインスタンスを閉じる必要があります。 ロックが解放されるまで、アセンブリを更新することはできません。 
  
次の例では、Exchange 管理シェルを使用してインストールし、という名前の MyAgent を[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)という名前の MyAgents.MyAgentFactory から派生したクラスを使用してエージェントを有効にする方法を示します。 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
この例では、エージェントがインストールされたサーバーで、エージェントに MyCustomAgent という名前を付けます。次の例は、MyCustomAgent という名前のエージェントを有効化する方法を示しています。
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
クライアント アクセス サーバーのフロント エンド トランスポート サービスのトランスポート エージェントを管理するためには、コマンドを次の値を追加: `-TransportService FrontEnd`。 など、フロント エンド トランスポート サービスのトランスポート エージェントを表示するには、次のコマンドを実行します。
  
 `Get-TransportAgent -TransportService FrontEnd`
  
インストールの詳細については、有効化、および管理、エージェントは、[トランスポート エージェントの管理](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx)を参照してください。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 RoutingAgent トランスポート エージェントを作成します。](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Exchange 2013 SmtpReceiveAgent トランスポート エージェントを作成します。](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Exchange 2013 DeliveryAgent トランスポート エージェントを作成します。](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
    

