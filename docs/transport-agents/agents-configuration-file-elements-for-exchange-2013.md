---
title: Exchange 2013 のエージェント構成ファイルの要素
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Agents
api_type:
- schema
ms.assetid: 3047653b-d712-46c1-ae0a-73f3975f5e9d
description: XML 要素に関する情報は、agents.config 2013 fetagents.config構成ファイルExchangeします。
ms.openlocfilehash: bdf394130f7818c5b956e8b15eed86a6318b9698
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510422"
---
# <a name="agents-configuration-file-elements-for-exchange-2013"></a>Exchange 2013 のエージェント構成ファイルの要素

XML 要素に関する情報は、agents.config 2013 fetagents.config構成ファイルExchangeします。
  
**製品:** Exchange Server 2013
  
Exchange サーバーにクライアント アクセス サーバーの役割またはメールボックス サーバーの役割をインストールすると、サーバーにインストールされたエージェントに関する構成情報を格納する XML ファイルがインストーラーによって作成されます。このファイルに直接書き込むことはできません。  
  
フロント エンド トランスポート サービスはクライアント アクセス サーバー上で実行し、fetagents.config という名前のファイルに書き込みを行います。トランスポート サービスとメールボックス トランスポート サービスはメールボックス サーバー上で実行し、agents.config という名前のファイルに書き込みを行います。クライアント アクセス サーバーの役割とメールボックス サーバーの役割の両方を備えたコンピューターには、fetagents.config と agents.config の両方のファイルが存在することになります。  
  
これらのファイルへの書き込みは、Exchange 管理シェルでトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。 トランスポート エージェントコマンドレットの詳細については[、「Mail Flowコマンドレット on TechNet」](https://technet.microsoft.com/library/aa998553%28v=exchg.150%29.aspx)を参照してください。 
  
> [!NOTE]
> クライアント アクセス サーバー上のフロント エンド トランスポート サービスを拡張するエージェントとメールボックス サーバー上のトランスポート サービスを区別するために、トランスポート エージェントコマンドレットには、トランスポート サービスの値が "Hub"、フロントエンド トランスポート サービスの "FrontEnd" の  _TransportService_ パラメーターがあります。 
  
agents.config ファイルまたは fetagents.config ファイルを読み込むことで、サーバー上に 1 つ以上のエージェントが存在するかどうかと、そのエージェントの構成情報を確認できます。このドキュメントでは、agents.config ファイルまたは fetagents.config ファイルの情報を読み取るために使用できるリファレンスを提供します。これらのファイルの形式は、どちらも同じです。このドキュメントでは、これらのファイルへの書き込み方法に関する情報は提供していません。
  
> [!CAUTION]
> agents.config ファイルや fetagents.config ファイルへの書き込みにサポートされていない方法を使用すると、トランスポート サービスまたはトランスポート エージェントのどちらか、または両方に障害が発生するなど、予期できない結果を招くことになります。これらのファイルは、どちらも直接書き込んではいけません。これらのファイルへの書き込みは、Exchange 管理シェルのトランスポート エージェントのコマンドレットを使用する方法のみがサポートされています。 
  
## <a name="location-of-the-transport-agent-configuration-files"></a>トランスポート エージェント構成ファイルの場所
<a name="bk_ConfigLoc"> </a>

Exchange 2013 をインストールすると、インストールされているサーバーの役割に応じて、agents.config.template または fetagents.config.template という名前の XML ファイルが \<ExchangeInstallFolder\> \TransportRoles\Agents フォルダー (Exchange 2013 をインストールしたフォルダー) に作成されます。 \<ExchangeInstallFolder\> クライアント アクセス サーバーの役割をインストールする場合、Exchange 2013 は fetagents.config.template ファイルをコピーしてfetagents.config。メールボックス サーバーの役割をインストールする場合、Exchange 2013 は agents.config.template ファイルをコピーして、agents.config。Exchange 2013 では、サーバー上のトランスポート エージェント構成を変更すると、このファイルの読み取りと書き込みを行います。
  
## <a name="verifying-a-transport-agent-installation"></a>トランスポート エージェントのインストールの検証
<a name="bk_verifyinstall"> </a>

.NET Framework が提供する XML 機能を使用すると、XML ファイル (agents.config または fetagents.config) を読み取って検証できます。トランスポート エージェントのインストールと構成を検証するには、構成ファイルの XML を読み取って、トランスポート エージェントに対応する [agent](agent.md) 要素を見つけます。特定のトランスポート エージェントの **agent** 要素が存在しない場合、そのトラスポート エージェントはインストールされていません。トランスポート エージェントがインストールされている場合は、**agent** 要素の属性を読み取ることで、そのエージェントの構成を確認できます。 
  
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
- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
- [Exchange 2013 のトランスポート エージェントの名前空間](transport-agent-namespaces-in-exchange-2013.md)
- [メール Flowコマンドレット](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)
    

