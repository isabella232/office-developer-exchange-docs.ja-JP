---
title: Exchange 2013 のバックアップと復元アプリケーションの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Exchange 2013 のバックアップと復元アプリケーションの、コンポーネントとアーキテクチャに関する情報と、バックアップと復元アプリケーションを作成するためのシステム要件に関する情報を確認できます。
ms.openlocfilehash: f8a332d0816792f8888c97a8394886b026f5204b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455278"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Exchange 2013 のバックアップと復元アプリケーションの作成

Exchange 2013 のバックアップと復元アプリケーションの、コンポーネントとアーキテクチャに関する情報と、バックアップと復元アプリケーションを作成するためのシステム要件に関する情報を確認できます。
  
**製品:** Exchange Server 2013 
  
Windows server 2008 以降のバージョンの Windows Server で[ボリュームシャドウコピーサービス (VSS)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx)を使用して、Exchange server 2013 データをバックアップおよび復元するアプリケーションを作成できます。 VSS は、サードパーティ製のストレージ管理システム、ビジネス アプリケーション、ハードウェアの間でシャドウ コピーを作成して管理できるようにするインフラストラクチャを提供します。 シャドウコピーを使用する VSS インフラストラクチャに基づいてソリューションを作成し、1つ以上の Exchange 2013 データベースをバックアップおよび復元できます。 
  
## <a name="backup-and-restore-application-prerequisites"></a>バックアップと復元アプリケーションの前提条件
<a name="bk_systemrequirements"> </a>

カスタムバックアップおよび復元アプリケーションと VSS が Exchange 2013 データベースをバックアップおよび復元するためには、環境に次のものが含まれている必要があります。
  
- Windows Server 2008 以降の Windows Server のバージョン 
    
- Exchange 2013
    
さらに、バックアップと復元アプリケーションを作成している場合、開発環境における次の制限に注意してください。
  
- VSS は、COM 相互運用アセンブリを経由して .NET Framework のマネージ コードからアクセスできる、アンマネージ COM API です。
    
- Exchange 管理シェルは、.NET Framework のマネージ コードを使ってアクセスするマネージ アプリケーションです。
    
- Exchange 2013 で提供される CHKSGFILES API は、ネイティブコードの64ビット DLL です。 Exchange 2013 データベースでの Exchange 2007 32 ビット CHKSGFILES DLL の使用はサポートされていません。
    
## <a name="backup-and-restore-application-overview"></a>バックアップと復元アプリケーションの概要
<a name="bk_components"> </a>

VSS は次のコンポーネント間の通信を調整します。 
  
- VSS リクエスターはバックアップ アプリケーションです
    
- VSS ライター
    
- VSS プロバイダーは、シャドウ コピーを作成するシステム、ソフトウェア、ハードウェア コンポーネントです
    
VSS を使用して Exchange 2013 データをバックアップするには、バックアップアプリケーションが Exchange 2013 対応の VSS リクエスターである必要があります。 Exchange 2013 には、Windows Server バックアッププログラム用に Microsoft Exchange ライターと呼ばれる VSS ライターが含まれています。ただし、Exchange ライターはボリューム全体のみをバックアップします。 個別の Exchange 2013 データベースはバックアップされません。 さらに柔軟性が必要な場合、個々の Exchange データベースを操作できる Exchange 対応の VSS ライターを備えたサード パーティ製バックアップ アプリケーションを使うか、カスタムの VSS リクエスターを作成できます。
  
アプリケーションが VSS を呼び出してバックアップを開始する前に、バックアップする Exchange 2013 システムのストレージ構成に関する情報を取得する必要があります。 その情報は Actice Directory ドメイン サービス (AD DS) に格納されています。 バックアップ アプリケーションは、Exchange 管理シェル コマンドを使って Exchange のストレージ構成データを取得できます。 詳細については、「 [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。 
  
Exchange 2013 のバックアップアプリケーションは、VSS COM Api を呼び出して、Exchange データベースのフル、コピー、差分、および増分バックアップを作成します。VSS ライターと直接やり取りすることはありません。 Exchange のデータベース可用性グループ (DAG) の機能により、初回の完全バックアップと以降の増分バックアップが DAG の異なるサーバーからのものでも、アプリケーションで完全整合バックアップを作成できます。 VSS が Exchange データのコピーを作成した後、バックアップ アプリケーションはデータを目的のメディアに格納します。
  
Exchange 2013 データベースを復元するには、復元アプリケーションはバックアップメディアからデータベースとログファイルを取得し、それらを Exchange サーバーのアクティブなディスクストレージに格納します。 個々のデータベースは特定の Exchange サーバーに関連付けられていません。 
  
バックアップおよび復元アプリケーションは、exchange 2013 データベースに対して VSS によって実行される操作を正しく制御および管理するために、Exchange 2013 固有のパラメーターをいくつか指定する必要があります。 たとえば、Exchange 2013 は最大で100の同時アクティブなデータベースをサポートしているため、バックアップアプリケーションはデータベースファイル、トランザクションログファイル、チェックポイントファイルデータベースコンポーネントを正確に指定して処理する必要があります。
  
最後の完全バックアップ以降に変更されたデータベースを再構築するには、リストア アプリケーションで別のバックアップからのデータベースとログ ファイルが必要です。 たとえば、毎週の完全バックアップと、毎日の 1 回以上の増分バックアップが必要になることがあります。 Dag を使用する Exchange 2013 システムでは、復元アプリケーションは、同じ DAG 内の異なるサーバー上の異なるデータベースコピーからのバックアップを使用してデータベースを再構築できます。 ただし、DAG データベースをバックアップから復元する方法として唯一サポートされているのは、同じデータを使ってデータベースのすべてのアクティブ コピーとパッシブ コピーを復元することです。
  
すべてのデータが設定されると、復元アプリケーションは、データベースとログ ファイルの整合性を確認するよう Exchange に通知します。データベースとログ ファイルが適切に復元されると、Exchange サーバーは、ログ ファイルを再生してデータベースを最新の状態にしてマウントできます。既にマウントされているデータベースのアクティブなコピーを持つサーバーにデータベースが復元された場合、データベースは回復データベースとして扱われます。別のサーバーにデータベースが復元された場合、データベースは個別にマウントされるか、そのレプリカを DAG に追加することができます。
  
## <a name="backup-and-restore-system-architecture"></a>バックアップと復元のシステム アーキテクチャ
<a name="bk_ExchangeVSS"> </a>

VSS は、サードパーティ (またはカスタム) プロバイダーを通して、Windows Server ファイル システムと大容量記憶装置ドライバーと通信します。 ハードウェア プロバイダーは、シャドウ コピーが作成される場所を決定します。 VSS は、ハードウェア実装に関する詳しい情報がない場合、バックアップと復元アプリケーションがシャドウ コピーにアクセスできるように、ハードウェア固有のシャドウ コピーを抽象化します。 バックアップと復元アプリケーションが Exchange 2013 と Windows Server と通信する方法を次の図に示します。
  
**図 1バックアップと復元のシステム アーキテクチャ**

![バックアップおよび復元アプリケーションがやり取りする方法を示す図。Exchange、Windows Server とクライアント アプリケーションの間に双方向通信が存在します。Windows Server は大容量記憶装置またはバックアップ メディアともやり取りします。](media/VSS_architecture_E2k7.gif)
  
バックアップと復元アプリケーションは VSS リクエスターとして機能します。 リクエスターは VSS と通信して、Exchange 2013 に関する情報を取得し、シャドウコピーの作成を開始し、バックアップのためにデータにアクセスできるようにします。 
  
Exchange ストアは、Exchange 2013 のコンポーネントであり、Windows Server ファイルシステムを使用して Exchange 2013 データベースにアクセスします。 ファイル システム内で、各 Exchange サーバーは、最大 100 個のデータベースと、それに付属のデータベース (.edb) ファイル、トランザクション ログ ファイル、チェックポイント ファイルを同時にマウントできます。
  
VSS をサポートするために、exchange 2013 には exchange ストアに組み込まれた Exchange ライターが含まれています。 Exchange ライターは、バックアップの前にデータベースを停止およびマウント解除し、バックアップの完了後にデータベースを解放してマウントを解除するために、(リクエスターの代わりに動作する) Exchange ストアと連携します。 復元中に、バックアップと復元アプリケーションは、exchange ストアと連携してデータベースのマウントを解除し、データベースファイルを置き換え、データベースをマウントして、トランザクションログを (必要に応じて) 再生するように Exchange ライターに指示します。
  
またリクエスターは、復元時にも VSS と通信し、復元に対応するためにシステムの準備を整えてから、大容量記憶装置にデータを戻します。バックアップと復元アプリケーションも Windows Server と連携し、バックアップ記憶領域メディア (テープ アーカイブ、記憶域ネットワーク、その他のバックアップ メディア) からのデータの読み取りとデータの書き込みを行います。
  
復元されたデータベースは、通常のアクティブなデータベースとして、または Exchange 2013 の回復用データベースとしてマウントできます。 各 Exchange サーバー上の回復用データベースとして指定できるのは、1 つのマウントされたデータベースのみです。
  
Exchange 2013、VSS、およびバックアップと復元アプリケーション間でバックアップと復元の操作を正常に完了するために必要な情報は、Exchange ライターのメタデータの一部として転送されます。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [Exchange 2013 のデータベースを復元する](restoring-exchange-2013-databases.md)
    
- [Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Exchange 2013 で Eseutil ツールを使用してバックアップの整合性を検証する](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange のバックアップと復元](backup-and-restore-for-exchange-2013.md) 
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md) 
- [ボリューム シャドウ コピー サービス](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

