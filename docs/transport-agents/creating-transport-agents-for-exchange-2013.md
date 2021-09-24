---
title: Exchange 2013 のトランスポート エージェントの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: 2013 年 2013 年にカスタム トランスポート エージェントを作成するExchange、カスタム エージェントを作成するためのシステム要件について説明します。
ms.openlocfilehash: ea5ae1fab85fde781cb365a21b7a40ccd52955b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520956"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Exchange 2013 のトランスポート エージェントの作成

2013 年 2013 年にカスタム トランスポート エージェントを作成するExchange、カスタム エージェントを作成するためのシステム要件について説明します。
  
**製品:** Exchange Server 2013
  
Exchange Server 2013 には、メッセージの処理に使用できるいくつかのトランスポート エージェントが含まれています。 Exchange に付属しているアセンブリを使用すると、自分の組織のニーズに応じた特定のタスクを実行するための、独自のカスタム エージェントを作成できます。 たとえば、SmtpReceiveAgent トランスポート エージェントを使用すると、SMTP プロトコルで受信されるメッセージをインターセプトして、そのメッセージを処理することで、あらかじめ書式設定されているテキストが含まれるように本文の書式を変換できます。 RoutingAgent トランスポート エージェントを使用すると、別のサーバーへのルート上にあるサーバーを通過するメッセージをログに記録できます。 また、さらに複雑な複数のエージェントを使用する機能を作成することもできます。 たとえば、ウイルス対策エージェントを作成する場合は、SmtpReceiveAgent エージェントと RoutingAgent エージェントを実装できます。 ネットワーク上に SMTP プロトコルをサポートしないコンポーネントがある場合は、Exchange サーバーと外部コンポーネントとの間の通信を処理するために、DeliveryAgent トランスポート エージェントを使用できます。 
  
この記事では、独自のトランスポート エージェントを作成するための前提条件と、それに関連するタスクに関する情報を示します。 特定のトランスポート エージェントの作成の詳細については、「create a RoutingAgent transport agent [for Exchange 2013」、「create](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)a SmtpReceiveAgent transport agent for [Exchange 2013」、および「create](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)a DeliveryAgent transport agent for [Exchange 2013」](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)を参照してください。
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>トランスポート エージェントを作成するための前提条件
<a name="bk_prerequisites"> </a>

トランスポート エージェントを実装するために必要な前提条件を次に示します。
  
- 2013 Exchangeクライアント アクセス サーバーまたはエッジ トランスポート サーバー上でフロントエンド トランスポート サービスを実行しているコンピューター、またはメールボックス サーバー上のトランスポート サービス。 2013 年 2013 年のサーバー役割アーキテクチャの詳細については、「Exchange [2013](transport-agent-concepts-in-exchange-2013.md)のトランスポート エージェントの概念」を参照Exchangeしてください。
    
- トランスポート エージェント クラスの次のアセンブリ。
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- 4.5 .NET Framework 4.5
    
また、2012 年Visual Studioすることをお勧めします。 トランスポート エージェントは、.NET または Visual Basicを使用して実装C#。
  
## <a name="referencing-the-assemblies"></a>アセンブリの参照
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 には、トランスポート動作の拡張をサポートするクラスのExchangeがあります。 これらのクラスには、.NET Framework 4.5 が必要です。 これらのクラスに基づいてトランスポート エージェントを実装する方法は、2012 年Visual Studio使用します。
  
2013 Exchangeインストーラーは、トランスポート エージェントの開発に使用されるアセンブリをインストールし、グローバル アセンブリ キャッシュ (GAC) に登録します。 トランスポート エージェントの実装を開始するには、Microsoft への参照を作成します。Exchange。クラス ライブラリ プロジェクトの Data.Transport アセンブリ。
  
## <a name="implementing-a-transport-agent"></a>トランスポート エージェントの実装
<a name="bk_implementationExample"> </a>

次の例は [、SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) クラスと [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) クラスから派生するクラスの最小限の実装を示しています。 
  
> [!CAUTION]
> 同じイベントに対して複数のトランスポート エージェントがインストールおよび登録されている場合、1 人のエージェントがメール アイテムからすべての受信者を削除した場合でも、すべてのエージェントが呼び出されます。 >未処理のエラーや予期しない動作を避けるために、トランスポート エージェントは、メール アイテムの受信者数が 0 に等しいケースを処理する必要があります。 
  
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

エージェントを DLL にコンパイルした後、開発サーバーにエージェントをインストールして有効にするExchangeがあります。 管理シェル[Exchange、Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx)コマンドレットを使用してエージェントをインストールし[、Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx)コマンドレットを使用してエージェントを有効にします。 管理シェルの使用方法については、「Exchange [PowerShell (Exchange Server管理シェルExchangeを参照してください](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)。
  
> [!CAUTION]
> トランスポート エージェントは、受信したすべての電子メール メッセージにフル アクセスできます。 Exchange 2013 では、トランスポート エージェントの動作は制限しません。 不安定なトランスポート エージェント、またはセキュリティ上の欠陥が含まれているトランスポート エージェントは、2013 年のセキュリティと安定性にExchangeがあります。 したがって、完全に信頼し、完全にテストされたトランスポート エージェントのみをインストールする必要があります。 
  
**Install-TransportAgent コマンドレットを使用して** エージェントをインストールすると、Exchange管理シェルはアセンブリのロックを保持します。 アセンブリのロックを解除するには、エージェントのインストールに使用Exchange管理シェルのインスタンスを閉じる必要があります。 ロックを解除するまで、アセンブリを更新できません。 
  
次の例は、myAgents.MyAgentFactory という名前の[SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)から派生したクラスを使用して、Exchange 管理シェルを使用して MyAgent という名前のエージェントをインストールして有効にする方法を示しています。 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
次の使用例は、エージェントがインストールされているサーバー上のエージェント MyCustomAgent に名前を付ける。 次の例は、MyCustomAgent という名前のエージェントを有効にする方法を示しています。
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
クライアント アクセス サーバーのフロント エンド トランスポート サービスでトランスポート エージェントを管理するには、次の値をコマンドに追加します  `-TransportService FrontEnd` 。 たとえば、フロント エンド トランスポート サービスでトランスポート エージェントを表示するには、次のコマンドを実行します。
  
 `Get-TransportAgent -TransportService FrontEnd`
  
エージェントのインストール、有効化、および管理の詳細については、「Manage [Transport Agent」を参照してください](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [2013 年の RoutingAgent トランスポート エージェントExchangeする](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [2013 年の SmtpReceiveAgent トランスポート エージェントExchangeする](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [2013 年の DeliveryAgent トランスポート エージェントExchangeする](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)   
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
    

