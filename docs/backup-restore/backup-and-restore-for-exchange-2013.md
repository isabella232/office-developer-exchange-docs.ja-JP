---
title: Exchange のバックアップと復元
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Exchange 2013 用のバックアップおよび復元アプリケーションの作成に関する情報を参照してください。
ms.openlocfilehash: 1c5d99be60501fd1c4414ea22294bd05645bb0a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455241"
---
# <a name="backup-and-restore-for-exchange"></a>Exchange のバックアップと復元
  
Exchange Server 2013 では、データベース可用性グループ (Dag) が提供されており、保存されたデータを安全かつ利用可能な状態に保つことができます。また、カスタムのバックアップおよび復元アプリケーションの必要性を減らすことができます。 Dag は、データが失われないようにするために、オフサイトデータの冗長性を有効にします。 しかし、多くの障害復旧計画には、DAG による冗長性を確保するために、従来のバックアップと復元の方法、およびカスタムアプリケーションを含むシステムが引き続き含まれています。 組織でデータの可用性と冗長性を確保するために、exchange Server および Windows Server オペレーティングシステムテクノロジを使用して Exchange データをバックアップおよび復元するカスタムアプリケーションを作成できます。

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Exchange 2013 バックアップ テクノロジ

Exchange 2013 には、管理者が Exchange データの VSS ベースのバックアップを作成するために使用できる Windows Server バックアップ用プラグインが含まれています。 また、管理者は Exchange データベースのバックアップと復元にも Windows Server バックアップを使用できます。 Exchange 2013 用のバックアップと復元アプリケーションを作成する場合は、exchange 2013 用の VSS writer をサポートする Exchange 対応アプリケーションを作成し、そのバックアップの整合性を検証するために CHKSGFILES API を使用する必要があります。 詳細については、「 [Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)する」を参照してください。

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Exchange 2013 の VSS ライター

Exchange 2013 では、exchange Server 2010 および Exchange Server 2007 の VSS writer アーキテクチャに大きな変更が導入されています。 Exchange 2010 と Exchange 2007 には、2つの VSS ライター (Exchange Information Store service (store.exe) 内と Exchange Replication サービス (msexchangerepl.exe) 内部に1つ) が含まれています。 Exchange 2013 では、VSS ライター機能は Exchange レプリケーションサービスにあります。 バックアップと復元のアプリケーションは、Microsoft Exchange Writer と呼ばれる新しい VSS writer を使用して、アクティブデータベースコピーとパッシブデータベースコピーをバックアップし、バックアップしたデータベースコピーを復元します。 新しい VSS writer は Exchange Replication サービスで実行されますが、ライターを使用できるようにするには、Exchange Information Store サービスが実行されている必要があります。 そのため、Exchange データベースのバックアップの作成や復元には両方のサービスが必要です。
  
VSS writer アーキテクチャは Exchange 2013 で更新されましたが、基礎となる機能は変更されていません。 Exchange 2010 用のバックアップと復元アプリケーションを作成した場合は、Exchange 2013 のアプリケーションを変更する必要はありません。 互換性を確保するために、最新のファイルを使用してカスタム アプリケーションを再コンパイルしてください。 Exchange 2007 以前のバージョン用に作成したバックアップおよび復元アプリケーションは、最新の CHKSGFILES API を使用するようにコードを書き直す必要があります。
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>VSS バックアップおよび復元について知っておくべき事項

|ご参考までに|説明|
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

- [ボリュームシャドウコピーサービス (Windows)](https://msdn.microsoft.com/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- 
  [Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange Management Shell](../management/exchange-management-shell.md)   
- [Exchange のトランスポート エージェント](../transport-agents/transport-agents-in-exchange-2013.md) 
    

