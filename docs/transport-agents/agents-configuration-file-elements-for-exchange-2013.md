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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759236"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Exchange 2013 のエージェント構成ファイルの要素

Exchange 2013 の agents.config と fetagents.config の構成ファイルの XML 要素についての情報を検索します。
  
**に適用されます:** Exchange Server 2013
  
Exchange サーバーにクライアント アクセス サーバーの役割またはメールボックス サーバーの役割をインストールすると、サーバーにインストールされたエージェントに関する構成情報を格納する XML ファイルがインストーラーによって作成されます。このファイルに直接書き込むことはできません。  
  
フロント エンド トランスポート サービスはクライアント アクセス サーバー上で実行し、fetagents.config という名前のファイルに書き込みを行います。トランスポート サービスとメールボックス トランスポート サービスはメールボックス サーバー上で実行し、agents.config という名前のファイルに書き込みを行います。クライアント アクセス サーバーの役割とメールボックス サーバーの役割の両方を備えたコンピューターには、fetagents.config と agents.config の両方のファイルが存在することになります。  
  
これらのファイルへの書き込みをサポートされている唯一の方法は、Exchange 管理シェルでトランスポート エージェントのコマンドレットを使用してです。 トランスポート エージェントのコマンドレットの詳細については、TechNet の[メール フローのコマンドレット](http://technet.microsoft.com/en-us/library/aa998553%28v=exchg.150%29.aspx)を参照してください。 
  
> [!NOTE]
> 区別するクライアント アクセス サーバーのフロント エンド トランスポート サービスを拡張するためのエージェント メールボックス サーバーのトランスポート サービス、トランスポート エージェントのコマンドレットは、トランスポートの「ハブ」の値を持つ_TransportService_パラメーターを持つサービスとフロント エンド トランスポート サービスの「フロント エンド」です。 
  
agents.config ファイルまたは fetagents.config ファイルを読み込むことで、サーバー上に 1 つ以上のエージェントが存在するかどうかと、そのエージェントの構成情報を確認できます。このドキュメントでは、agents.config ファイルまたは fetagents.config ファイルの情報を読み取るために使用できるリファレンスを提供します。これらのファイルの形式は、どちらも同じです。このドキュメントでは、これらのファイルへの書き込み方法に関する情報は提供していません。
  
> [!CAUTION]
> agents.config ファイルや fetagents.config ファイルへの書き込みにサポートされていない方法を使用すると、トランスポート サービスまたはトランスポート エージェントのどちらか、または両方に障害が発生するなど、予期できない結果を招くことになります。これらのファイルは、どちらも直接書き込んではいけません。これらのファイルへの書き込みは、Exchange 管理シェルのトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>トランスポート エージェント構成ファイルの場所
<a name="bk_ConfigLoc"> </a>

インストーラーが agents.config.template か、インストール、サーバーの役割によって、fetagents.config.template という XML ファイルを作成する Exchange 2013 をインストールすると、 \<ExchangeInstallFolder\>\TransportRoles\Agentsフォルダー (位置\<ExchangeInstallFolder\>は、Exchange 2013 をインストールしたフォルダー)。 クライアント アクセス サーバー ロールをインストールする場合、Exchange 2013 は、fetagents.config に fetagents.config.template ファイルをコピーします。メールボックス サーバーの役割をインストールする場合、Exchange 2013 は agents.config に agents.config.template ファイルをコピーします。Exchange 2013 では、読み取り、サーバー上のトランスポート エージェントの構成を変更するときにこのファイルを書き込みます。
  
## <a name="verifying-a-transport-agent-installation"></a>トランスポート エージェントのインストールの検証
<a name="bk_verifyinstall"> </a>

読み取りおよび、agents.config または fetagents.config の XML ファイルを検証するのには.NET Framework が提供する XML 機能を使用することができます。 インストールとトランスポート エージェントの構成を確認するに構成ファイル内の XML の読み取りし、トランスポート エージェントに対応する[エージェント](agent.md)の要素を検索します。 特定のトランスポート エージェントの**エージェント**の要素が存在しない場合は、トランスポート エージェントがインストールされていません。 トランスポート エージェントがインストールされている場合は、その構成を決定する**エージェント**の要素の属性を読み取ることができます。 
  
## <a name="configuration-file-element-hierarchy"></a>構成ファイルの要素の階層構造
<a name="bk_elementref"> </a>

次のコードは、構成 XML ファイルの要素の階層構造を示しています。
  
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

## <a name="in-this-section"></a>このセクションの内容
<a name="bk_elementreflist"> </a>

- [エージェント](agent.md)
    
- [agentExecution](agentexecution.md)
    
- [agentList](agentlist.md)
    
- [構成](configuration.md)
    
- [messageSnapshot](messagesnapshot.md)
    
- [mexRuntime](mexruntime.md)
    
- [監視](monitoring.md)
    
## <a name="see-also"></a>関連項目

- [Exchange のトランスポート エージェント](transport-agents-in-exchange-2013.md)
- [トランスポート エージェントの概念には、Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
- [トランスポート エージェントの名前空間では、Exchange 2013](transport-agent-namespaces-in-exchange-2013.md)
- [メール フローのコマンドレット](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)
    

