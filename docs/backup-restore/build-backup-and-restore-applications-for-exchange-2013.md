---
title: Exchange 2013 のバックアップと復元アプリケーションの作成
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e5e952a5-add1-417c-a3c2-230f4dc99b00
description: Exchange 2013 のバックアップと復元アプリケーションの、コンポーネントとアーキテクチャに関する情報と、バックアップと復元アプリケーションを作成するためのシステム要件に関する情報を確認できます。
ms.openlocfilehash: 590ac029e157196d370cbcbe54e5df75bc1a830b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513879"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Exchange 2013 のバックアップと復元アプリケーションの作成

Exchange 2013 のバックアップと復元アプリケーションの、コンポーネントとアーキテクチャに関する情報と、バックアップと復元アプリケーションを作成するためのシステム要件に関する情報を確認できます。
  
**製品:** Exchange Server 2013 
  
Windows Windows Server 2008 から始まるバージョンの Windows Server でボリューム シャドウ コピー サービス[(VSS)](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx)を使用して、Exchange Server 2013 データをバックアップおよび復元するアプリケーションを作成できます。 VSS は、サードパーティ製のストレージ管理システム、ビジネス アプリケーション、ハードウェアの間でシャドウ コピーを作成して管理できるようにするインフラストラクチャを提供します。 2013 年の 1 つ以上のデータベースをバックアップおよび復元するためにシャドウ コピーを使用する VSS インフラストラクチャに基Exchange作成できます。 
  
## <a name="backup-and-restore-application-prerequisites"></a>バックアップと復元アプリケーションの前提条件
<a name="bk_systemrequirements"> </a>

カスタム バックアップと復元アプリケーションと VSS が 2013 データベースのバックアップと復元を行Exchange、環境に次のものが含まれる必要があります。
  
- Windows Server 2008 以降の Windows Server のバージョン 
    
- Exchange 2013
    
さらに、バックアップと復元アプリケーションを作成している場合、開発環境における次の制限に注意してください。
  
- VSS は、COM 相互運用アセンブリを経由して .NET Framework のマネージ コードからアクセスできる、アンマネージ COM API です。
    
- Exchange 管理シェルは、.NET Framework のマネージ コードを使ってアクセスするマネージ アプリケーションです。
    
- 2013 年 2013 年に提供される CHKSGFILE Exchange S API は、ネイティブ コード 64 ビット DLL です。 2013 Exchangeを使用した 2007 32 ビット CHKSGFILES DLL Exchange使用はサポートされていません。
    
## <a name="backup-and-restore-application-overview"></a>バックアップと復元アプリケーションの概要
<a name="bk_components"> </a>

VSS は次のコンポーネント間の通信を調整します。 
  
- VSS リクエスターはバックアップ アプリケーションです
    
- VSS ライター
    
- VSS プロバイダーは、シャドウ コピーを作成するシステム、ソフトウェア、ハードウェア コンポーネントです
    
VSS を使用して 2013 Exchangeをバックアップするには、バックアップ アプリケーションが 2013 対応の VSS 要求Exchangeである必要があります。 Exchange 2013 には、Microsoft Exchange ライターと呼ばれる VSS ライターが含まれています。Windows サーバー のバックアップ プログラム。ただし、このExchangeはボリューム全体のみをバックアップします。 2013 データベースの個々Exchangeバックアップされません。 さらに柔軟性が必要な場合、個々の Exchange データベースを操作できる Exchange 対応の VSS ライターを備えたサード パーティ製バックアップ アプリケーションを使うか、カスタムの VSS リクエスターを作成できます。
  
アプリケーションが VSS を呼び出してバックアップを開始する前に、バックアップする Exchange 2013 システムのストレージ構成に関する情報を取得する必要があります。 その情報は Actice Directory ドメイン サービス (AD DS) に格納されています。 バックアップ アプリケーションは、Exchange 管理シェル コマンドを使って Exchange のストレージ構成データを取得できます。 詳細については[、「PowerShell Exchange Server (Exchange管理シェル) 」を参照してください](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)。 
  
Exchange 2013 バックアップ アプリケーションは、VSS COM API を呼び出して、データベースの完全バックアップ、コピーバックアップ、差分バックアップ、増分バックアップExchangeします。VSS ライターと直接対話しない。 Exchange のデータベース可用性グループ (DAG) の機能により、初回の完全バックアップと以降の増分バックアップが DAG の異なるサーバーからのものでも、アプリケーションで完全整合バックアップを作成できます。 VSS が Exchange データのコピーを作成した後、バックアップ アプリケーションはデータを目的のメディアに格納します。
  
Exchange 2013 データベースを復元するために、復元アプリケーションはバックアップ メディアからデータベースとログ ファイルを取得し、Exchange サーバーのアクティブ ディスク ストレージに格納します。 個々のデータベースは特定の Exchange サーバーに関連付けられていません。 
  
バックアップおよび復元アプリケーションでは、2013 データベースに対して VSS が実行する操作を正しく制御および管理するために、Exchange 2013 固有のパラメーターを多数指定Exchange必要があります。 たとえば、Exchange 2013 では最大 100 の同時にアクティブなデータベースがサポートされているので、バックアップ アプリケーションはデータベース ファイル、トランザクション ログ ファイル、チェックポイント ファイル データベース コンポーネントを正しく指定して処理する必要があります。
  
最後の完全バックアップ以降に変更されたデータベースを再構築するには、リストア アプリケーションで別のバックアップからのデータベースとログ ファイルが必要です。 たとえば、毎週の完全バックアップと、毎日の 1 回以上の増分バックアップが必要になることがあります。 DAG Exchange 2013 システムでは、同じ DAG 内の異なるサーバー上の異なるデータベース コピーからのバックアップを使用して、復元アプリケーションでデータベースを再構築できます。 ただし、DAG データベースをバックアップから復元する方法として唯一サポートされているのは、同じデータを使ってデータベースのすべてのアクティブ コピーとパッシブ コピーを復元することです。
  
すべてのデータが設定されると、復元アプリケーションは、データベースとログ ファイルの整合性を確認するよう Exchange に通知します。データベースとログ ファイルが適切に復元されると、Exchange サーバーは、ログ ファイルを再生してデータベースを最新の状態にしてマウントできます。既にマウントされているデータベースのアクティブなコピーを持つサーバーにデータベースが復元された場合、データベースは回復データベースとして扱われます。別のサーバーにデータベースが復元された場合、データベースは個別にマウントされるか、そのレプリカを DAG に追加することができます。
  
## <a name="backup-and-restore-system-architecture"></a>バックアップと復元のシステム アーキテクチャ
<a name="bk_ExchangeVSS"> </a>

VSS は、サードパーティ (またはカスタム) プロバイダーを通して、Windows Server ファイル システムと大容量記憶装置ドライバーと通信します。ハードウェア プロバイダーは、シャドウ コピーが作成される場所を決定します。VSS は、ハードウェア実装に関する詳しい情報がない場合、バックアップと復元アプリケーションがシャドウ コピーにアクセスできるように、ハードウェア固有のシャドウ コピーを抽象化します。バックアップと復元アプリケーションが Exchange 2013 と Windows Server と通信する方法を次の図に示します。
  
**図 1バックアップと復元のシステム アーキテクチャ**

![バックアップおよび復元アプリケーションがやり取りする方法を示す図。Exchange、Windows Server とクライアント アプリケーションの間に双方向通信が存在します。Windows Server は大容量記憶装置またはバックアップ メディアともやり取りします。](media/VSS_architecture_E2k7.gif)
  
バックアップと復元アプリケーションは VSS リクエスターとして機能します。 要求者は VSS と通信して、Exchange 2013 に関する情報を取得し、シャドウ コピーの作成を開始し、バックアップ用のデータにアクセスします。 
  
このExchangeは 2013 年 2013 年Exchangeコンポーネントであり、Exchange Server ファイル システムをWindows 2013 データベースにアクセスします。 ファイル システム内で、各 Exchange サーバーは、最大 100 個のデータベースと、それに付属のデータベース (.edb) ファイル、トランザクション ログ ファイル、チェックポイント ファイルを同時にマウントできます。
  
VSS をサポートするために、Exchange 2013 には、Exchangeストアに組み込Exchangeがあります。 Exchange ライターは、Exchange ストア (要求者に代わって動作) を調整して、データベースをバックアップする前にデータベースをフリーズおよびマウント解除し、バックアップの完了後にデータベースの凍結とマウントを解除します。 復元中、バックアップと復元アプリケーションは、Exchange ライターに対して、Exchange ストアと調整してデータベースをマウント解除し、データベース ファイルを置き換え、データベースをマウントし、必要に応じてトランザクション ログを再生するように指示します。
  
またリクエスターは、復元時にも VSS と通信し、復元に対応するためにシステムの準備を整えてから、大容量記憶装置にデータを戻します。バックアップと復元アプリケーションも Windows Server と連携し、バックアップ記憶領域メディア (テープ アーカイブ、記憶域ネットワーク、その他のバックアップ メディア) からのデータの読み取りとデータの書き込みを行います。
  
復元されたデータベースは、通常のアクティブ なデータベースとして、または 2013 Exchangeとしてマウントできます。 各 Exchange サーバー上の回復用データベースとして指定できるのは、1 つのマウントされたデータベースのみです。
  
Exchange 2013、VSS、およびバックアップと復元アプリケーションの間でバックアップと復元の操作を正常に完了するために必要な情報は、Exchange ライター メタデータの一部として転送されます。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [Exchange 2013 のデータベースを復元する](restoring-exchange-2013-databases.md)
    
- [2013 年に CHKSGFILES API を使用してバックアップExchangeする](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [2013 年に Eseutil ツールを使用してバックアップの整合性Exchangeする](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange のバックアップと復元](backup-and-restore-for-exchange-2013.md) 
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md) 
- [ボリューム シャドウ コピー サービス](https://msdn.microsoft.com/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

