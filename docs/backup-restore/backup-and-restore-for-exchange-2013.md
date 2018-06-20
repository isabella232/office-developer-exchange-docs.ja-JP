---
title: Exchange のバックアップ/リストア
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: バックアップの作成に関する情報を検索し、Exchange 2013 のアプリケーションを復元します。
ms.openlocfilehash: 9eceb3d512a73ad9cb07a01864fb8b029d5b5772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758859"
---
# <a name="backup-and-restore-for-exchange"></a>Exchange のバックアップ/リストア
  
Exchange Server 2013 には、セキュリティで保護され、保存されているデータを保持し、ユーザー設定のバックアップの必要性を減らすし、アプリケーションを復元するデータベース可用性グループ (Dag) が用意されています。 Dag は、確実にデータは失われず、オフサイトのデータの冗長性を有効にします。 ただし、多くの災害復旧プランは、従来のバックアップを含めるし、メソッドと、DAG での冗長性のためのカスタム アプリケーションなど、システムの復元に進みます。 データ可用性と、組織内の冗長性確保のため、バックアップし、Exchange データを復元する Exchange Server と Windows Server オペレーティング システムのテクノロジを使用するカスタム アプリケーションを作成できます。

<a name="bk_plugin"> </a>

## <a name="backup-technologies-in-exchange-2013"></a>Exchange 2013 バックアップ テクノロジ

Exchange 2013 には、Exchange データの VSS ベースのバックアップを作成する管理者が使用できる Windows Server バックアップのプラグインが含まれます。 管理者は、バックアップし、Exchange データベースの復元にも Windows Server バックアップを使用できます。 バックアップを作成し、Exchange 2013 のアプリケーションを復元する場合は、Exchange 2013 では、VSS ライターをサポートする Exchange 対応アプリケーションを作成し、そのバックアップの整合性を検証するために CHKSGFILES API を使用する必要があります。 詳細については、 [Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)を参照してください。

<a name="bk_vsswriter"> </a>

## <a name="vss-writer-in-exchange-2013"></a>Exchange 2013 の VSS ライター

Exchange 2013 では、VSS ライター アーキテクチャでは、Exchange Server 2010 と Exchange Server 2007 に大幅な変更が導入されています。 Exchange 2010 と Exchange 2007 には 2 つの VSS ライターが含まれます: Exchange インフォメーション ストア サービス (store.exe) と、Exchange レプリケーション サービス (msexchangerepl.exe) 内のいずれか 1 つです。 Exchange 2013 では、VSS ライターの機能にある Exchange レプリケーション ・ サービスです。 バックアップと復元アプリケーションは、アクティブおよびパッシブのデータベースのコピーをバックアップする、Microsoft Exchange ライターと呼ばれる新しい VSS ライターを使用し、データベースのコピー バックアップを復元します。 Exchange レプリケーション サービスの新しい VSS ライターが実行されると、ライターを使用するために Exchange インフォメーション ストア サービスを実行する必要があります。 その結果、両方のサービスは、バックアップまたは Exchange データベースを復元する必要があります。
  
VSS ライターのアーキテクチャは、Exchange 2013 に更新された、基になる機能は変更されていません。 Exchange 2010 のバックアップと復元のアプリケーションを作成する場合は、Exchange 2013 のアプリケーションに変更を加える必要はありません。 互換性を確保するのには、最新のファイルで、アプリケーションを再コンパイルすることを確認します。 Exchange 2007 または以前のバージョン用に作成されたバックアップと復元のアプリケーションでは、最新の CHKSGFILES API を使用するようにコードを書き直す必要があります。
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a>VSS バックアップおよび復元について知っておくべき事項

|についてわからない場合.|説明|
|:-----|:-----|
|アプリケーション アーキテクチャ  <br/> |Exchange データベースのバックアップに VSS を使用するバックアップおよび復元アプリケーションは、通常、バックアップを実行するバックグラウンド サービス、スケジュール サービス、およびバックアップと復元システムを制御および構成する Windows GUI アプリケーション コンソールで成り立っています。  <br/> |
|リモート使用  <br/> |Exchange サーバーのバックアップに VSS を使用するアプリケーションは、Exchange ストア プロセスを実行している Windows Server 2008 コンピューター上で実行する必要があります。大規模なストレージ システムの柔軟性を確保するために、Windows Server 2008 を実行するコンピューターには、ストレージ ボリュームをホストするハードウェアが物理的に含まれないようにします。  <br/> |
|言語とツール  <br/> |VSS の使用には、COM 準拠の任意の言語を使用できます。C++ で記述されたアプリケーションで、最も多く使用されています。シャドウ コピーの作成には、Exchange ストアをオフラインにすることが必要になるため、通常、バックアップ アプリケーションは時間が重要になります。そのため、Visual Basic や VBScript などの言語の使用は現実的ではありません。  <br/> |
|マネージ実装  <br/> |VSS API は、COM 相互運用機能アセンブリを通じて、マネージ コード環境で使用できます。  <br/> |
|スクリプトで使用可能  <br/> |はい。ただし、お勧めしません。  <br/> |
|利用可能なテスト ツールとデバッグ ツール  <br/> |Windows VSS を使用するアプリケーションのデバッグに、特別なツールは必要ありません。  <br/> |
   
## <a name="in-this-section"></a>このセクションの内容

- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    
- [バックアップを作成し、Exchange 2013 のアプリケーションを復元します。](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a>関連項目

- [ボリューム シャドウ コピー サービス (Windows)](http://msdn.microsoft.com/en-us/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [Exchange の EWS Managed API、EWS、および Web サービスについて学ぶ](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [Exchange 管理シェル](../management/exchange-management-shell.md)   
- [Exchange のトランスポート エージェント](../transport-agents/transport-agents-in-exchange-2013.md) 
    

