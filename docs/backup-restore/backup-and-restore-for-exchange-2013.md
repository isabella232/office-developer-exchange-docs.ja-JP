---
title: Exchange のバックアップと復元
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: 2013 年のバックアップおよび復元アプリケーションの作成に関するExchangeします。
ms.openlocfilehash: 2be8295985651319860ab2d2a143d69f663bf932
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514901"
---
# <a name="backup-and-restore-for-exchange"></a>Exchange のバックアップと復元
  
Exchange Server 2013 にはデータベース可用性グループ (DAG) が用意されています。 DAG を使用すると、オフサイト のデータ冗長性が有効になります。 ただし、多くの障害復旧計画には、DAG の冗長性を確保するために、カスタム アプリケーションを含む従来のバックアップと復元の方法とシステムが引き続き含まれます。 組織内のデータの可用性と冗長性を確保するために、Exchange Server および Windows Server オペレーティング システム テクノロジを使用して Exchange データをバックアップおよび復元するカスタム アプリケーションを作成できます。

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Exchange 2013 バックアップ テクノロジ

Exchange 2013 には、管理者が VSS ベースのデータのバックアップを作成するために使用できる Windows Server Backup 用のプラグインExchangeがあります。 また、管理者は Exchange データベースのバックアップと復元にも Windows Server バックアップを使用できます。 Exchange 2013 のバックアップと復元アプリケーションを作成する場合は、Exchange 2013 の VSS ライターをサポートする Exchange 対応アプリケーションを作成し、CHKSGFILES API を使用してそのバックアップの整合性を検証する必要があります。 詳細については[、「CHKSGFILES API](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)を使用してバックアップ整合性を検証する」を参照Exchangeしてください。

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Exchange 2013 の VSS ライター

Exchange 2013 では、2010 年および 2007 年の VSS ライター アーキテクチャに大きなExchange Serverが導入Exchange Serverされています。 Exchange 2010 および Exchange 2007 には、Exchange Information Store サービス (store.exe) 内と Exchange レプリケーション サービス (msexchangerepl.exe) 内の 2 つの VSS ライターが含まれます。 2013 Exchangeでは、VSS ライター機能はレプリケーション サービスExchangeにあります。 バックアップと復元アプリケーションでは、Microsoft Exchange Writer と呼ばれる新しい VSS ライターを使用して、アクティブおよびパッシブ データベース コピーをバックアップし、バックアップされたデータベース コピーを復元します。 新しい VSS ライターは Exchange レプリケーション サービスで実行しますが、ライターを使用するには、Exchange Information Store サービスが実行されている必要があります。 そのため、Exchange データベースのバックアップの作成や復元には両方のサービスが必要です。
  
VSS ライター アーキテクチャは 2013 年Exchange更新されましたが、基になる機能は変更されません。 Exchange 2010 のバックアップおよび復元アプリケーションを作成した場合は、Exchange 2013 のアプリケーションに変更を加える必要があります。 互換性を確保するために、最新のファイルを使用してカスタム アプリケーションを再コンパイルしてください。 Exchange 2007 以前のバージョン用に作成したバックアップおよび復元アプリケーションは、最新の CHKSGFILES API を使用するようにコードを書き直す必要があります。
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>VSS バックアップおよび復元について知っておくべき事項

|疑問に思っている場合...|説明|
|:-----|:-----|
|アプリケーション アーキテクチャ  <br/> |Exchange データベースのバックアップに VSS を使用するバックアップおよび復元アプリケーションは、通常、バックアップを実行するバックグラウンド サービス、スケジュール サービス、およびバックアップと復元システムを制御および構成する Windows GUI アプリケーション コンソールで成り立っています。  <br/> |
|リモート使用  <br/> |Exchange サーバーのバックアップに VSS を使用するアプリケーションは、Exchange ストア プロセスを実行している Windows Server 2008 コンピューター上で実行する必要があります。大規模なストレージ システムの柔軟性を確保するために、Windows Server 2008 を実行するコンピューターには、ストレージ ボリュームをホストするハードウェアが物理的に含まれないようにします。  <br/> |
|言語とツール  <br/> |VSS の使用には、COM 準拠の任意の言語を使用できます。C++ で記述されたアプリケーションで、最も多く使用されています。シャドウ コピーの作成には、Exchange ストアをオフラインにすることが必要になるため、通常、バックアップ アプリケーションは時間が重要になります。そのため、Visual Basic や VBScript などの言語の使用は現実的ではありません。  <br/> |
|マネージ実装  <br/> |VSS API は、COM 相互運用機能アセンブリを通じて、マネージ コード環境で使用できます。  <br/> |
|スクリプトで使用可能  <br/> |はい。ただし、お勧めしません。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |Windows VSS を使用するアプリケーションのデバッグに、特別なツールは必要ありません。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元アプリケーションの作成](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>関連項目

- [ボリューム シャドウ コピー サービス (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Exchange の EWS マネージ API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Exchange のトランスポート エージェント](../transport-agents/transport-agents-in-exchange-2013.md) 
    

