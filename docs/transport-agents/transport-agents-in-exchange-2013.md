---
title: Exchange のトランスポート エージェント
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 36d63aa6-1b72-4670-b5c3-da685f3017cb
description: Exchange 2013 のトランスポートエージェントに関する情報を参照してください。
ms.openlocfilehash: 62fb259672c47242a57b939deb4887e1e5519e2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461759"
---
# <a name="transport-agents-in-exchange"></a>Exchange のトランスポート エージェント
  
Exchange 2013 には、Exchange トランスポート動作の拡張をサポートし、コンテンツタイプの読み取り、書き込み、および変換を可能にするクラスのライブラリが用意されています。 これらのクラスを使用すると、トランスポート パイプライン内でメッセージの読み取り、書き込み、および処理を行う Exchange トランスポート アプリケーションを作成できます。
  
## <a name="what-you-need-to-know-about-transport-agents"></a>トランスポート エージェントについて知っておくべき事項

|ご参考までに|説明|
|:-----|:-----|
|Availability  <br/> |トランスポートエージェントは、Exchange 2007 以降のバージョンの Exchange で使用できます。 トランスポートエージェントは、Office 365 または Exchange Online ではサポートされていません。  <br/> |
|リモート使用  <br/> |トランスポート エージェントは Exchange サーバー上で実行し、リモート使用をサポートしていません。  <br/> |
|サポートされている言語  <br/> |トランスポート エージェントには、任意の .NET Framework 言語を使用できます。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |トランスポート エージェントのデバッグには、Visual Studio 2012 以降の Visual Studio の各バージョンを使用してください。  <br/> |
|展開の方法  <br/> |トランスポート エージェント アプリケーションは、[Exchange 管理シェル](../management/exchange-management-shell.md) スクリプトを使用してインストールできます。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 2013 の新規および更新されたトランスポート エージェント API](new-and-updated-transport-agent-apis-in-exchange-2013.md)
    
- [Exchange 2013 のトランスポート エージェントのコード サンプル](transport-agent-code-samples-for-exchange-2013.md)
    
- [Exchange 2013 におけるトランスポート エージェントの概念](transport-agent-concepts-in-exchange-2013.md)
    
- [Exchange 2013 トランスポート パイプライン内のメッセージの読み取りおよび変更](reading-and-modifying-messages-in-the-exchange-2013-transport-pipeline.md)
    
- [Exchange 2013 のトランスポート エージェントの作成](creating-transport-agents-for-exchange-2013.md)
    
- [Exchange 2013 のトランスポート エージェントのリファレンス](transport-agent-reference-for-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange Online と Exchange の開発](../exchange-server-development.md)    
- 
  [Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)   
- [Exchange のバックアップと復元](../backup-restore/backup-and-restore-for-exchange-2013.md) 
    

