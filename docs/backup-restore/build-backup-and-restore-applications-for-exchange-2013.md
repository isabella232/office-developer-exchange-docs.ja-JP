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
ms.openlocfilehash: e85a5364c40c472c9e1ea9d1d3b4e89329b1676f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758870"
---
# <a name="build-backup-and-restore-applications-for-exchange-2013"></a>Exchange 2013 のバックアップと復元アプリケーションの作成

Exchange 2013 のバックアップと復元アプリケーションの、コンポーネントとアーキテクチャに関する情報と、バックアップと復元アプリケーションを作成するためのシステム要件に関する情報を確認できます。
  
**に適用されます:** Exchange Server 2013 
  
Windows サーバーが Windows Server 2008 以降のバージョンでは[ボリューム シャドウ コピー サービス (VSS)](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx)を使用するにはバックアップし、Exchange Server 2013 のデータを復元するアプリケーションを作成します。 VSS では、作成し、サードパーティ製のストレージ管理システム、ビジネス アプリケーション、およびハードウェアの間でシャドウ コピーを管理することを可能にするインフラストラクチャを提供します。 VSS インフラストラクチャに基づくソリューションのバックアップを作成し、1 つまたは複数の Exchange 2013 のデータベースを復元するシャドウ ・ コピーを使用するを作成することができます。 
  
## <a name="backup-and-restore-application-prerequisites"></a>バックアップと復元アプリケーションの前提条件
<a name="bk_systemrequirements"> </a>

ユーザー設定のバックアップと復元アプリケーションと VSS のバックアップを作成し、Exchange 2013 のデータベースを復元するためには、環境を次に含める必要があります。
  
- Windows Server 2008 以降の Windows Server のバージョン  
    
- Exchange 2013
    
さらに、バックアップと復元アプリケーションを作成している場合、開発環境における次の制限に注意してください。
  
- VSS は、COM 相互運用アセンブリを経由して .NET Framework のマネージ コードからアクセスできる、アンマネージ COM API です。
    
- Exchange 管理シェルは、.NET Framework のマネージ コードを使ってアクセスするマネージ アプリケーションです。
    
- Exchange 2013 で提供される CHKSGFILES API は、ネイティブ コードの 64 ビット DLL です。 2013 の Exchange データベースと Exchange 2007 の 32年ビット CHKSGFILES DLL の使用はサポートされていません。
    
## <a name="backup-and-restore-application-overview"></a>バックアップと復元アプリケーションの概要
<a name="bk_components"> </a>

VSS は次のコンポーネント間の通信を調整します。  
  
- VSS リクエスターはバックアップ アプリケーションです
    
- VSS ライター
    
- VSS プロバイダーは、シャドウ コピーを作成するシステム、ソフトウェア、ハードウェア コンポーネントです
    
VSS を使用すると、Exchange 2013 のデータのバックアップを作成して、バックアップ ・ アプリケーションは、Exchange 2013 に対応した VSS の依頼者する必要があります。 Exchange 2013 には、ライターと呼ばれる、Microsoft Exchange、Windows Server バックアップ プログラムの VSS ライターが含まれています。ただし、Exchange ライターは、ボリューム全体をのみバックアップします。 それはバックアップされません個々 の Exchange 2013 のデータベースです。 柔軟性が必要な場合、個々 の Exchange データベースを扱うことができる Exchange 対応の VSS ライターを持つサード ・ パーティ製バックアップ ・ アプリケーションを使用することができます。 またはカスタム VSS リクエスターを作成することができます。
  
アプリケーションを呼び出すと、VSS バックアップを開始する前のバックアップは、Exchange 2013 のシステムの記憶域の構成に関する情報を取得する必要があります。 その情報は、Active Directory ドメイン サービス (AD DS) に格納されます。 バックアップ ・ アプリケーションは、Exchange 管理シェル コマンドを使用して Exchange の記憶域の構成データを取得できます。 詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。 
  
コピー、差分バックアップと増分バックアップ Exchange データベースは、作成する VSS COM Api の呼び出しを Exchange 2013 のバックアップ ・ アプリケーション対話せず直接 VSS ライター。 Exchange のデータベース可用性グループ (DAG) の機能は、場合でも、初期の完全バックアップと増分バックアップ以降には、DAG 内の別のサーバーからも完全に一貫性のあるバックアップを作成するようにアプリケーションを使用できます。 VSS では、Exchange データのコピーが作成された後、バックアップ ・ アプリケーションは、目的のメディアにデータを格納します。
  
2013 の Exchange データベースを復元するのには復元アプリケーションはバックアップ メディアからデータベース ファイルとログ ファイルを取得し、Exchange サーバーのアクティブなディスク ・ ストレージ上に格納します。 個々 のデータベースは、特定の Exchange サーバーに関連付けられていません。 
  
バックアップと復元のアプリケーションでは、2013 の Exchange データベースに対する VSS を実行する操作の管理を正しく制御して Exchange 2013 に固有のパラメーターの番号を指定する必要があります。 などの Exchange 2013 では、最大 100 個までの同時にアクティブなデータベースをサポートするためバックアップ ・ アプリケーション必要があります正しくを指定し、データベース ファイル、トランザクション ログ ファイルとチェックポイント ファイルのデータベース コンポーネントを処理します。
  
最後の完全バックアップ以降の変更があったデータベースを再構築するのには、リストア ・ アプリケーションには、別のバックアップからのデータベースとログ ファイルが必要です。 など、毎週のフル ・ バックアップと 1 つまたは複数の毎日の増分バックアップを必要ことがあります。 Exchange 2013 の Dag を使用するシステム、復元アプリケーションことができますデータベースを再構築、同じ DAG 内の別のサーバー上の別のデータベースのコピーからのバックアップを使用しています。 ただし、DAG のデータベースをバックアップから復元する唯一のサポートされている方法は、同じデータを使用してデータベースのすべてのアクティブおよびパッシブ ・ コピーを復元します。
  
すべてのデータが設定されると、復元アプリケーションは、データベースとログ ファイルの整合性を確認するよう Exchange に通知します。データベースとログ ファイルが適切に復元されると、Exchange サーバーは、ログ ファイルを再生してデータベースを最新の状態にしてマウントできます。既にマウントされているデータベースのアクティブなコピーを持つサーバーにデータベースが復元された場合、データベースは回復データベースとして扱われます。別のサーバーにデータベースが復元された場合、データベースは個別にマウントされるか、そのレプリカを DAG に追加することができます。
  
## <a name="backup-and-restore-system-architecture"></a>バックアップと復元のシステム アーキテクチャ
<a name="bk_ExchangeVSS"> </a>

VSS は、Windows サーバーのファイル システムとサードパーティ (またはカスタム) プロバイダーを通して大容量記憶装置ドライバーと通信します。 ハードウェア プロバイダーは、シャドウ コピーが作成される場所を決定します。 VSS は、ハードウェア実装の詳細に関する情報がない場合、シャドウ ・ コピーをバックアップおよび復元アプリケーションがアクセスできるように、ハードウェア固有のシャドウ ・ コピーを抽象化します。 Exchange 2013 と Windows Server バックアップと復元アプリケーションが対話する方法を次の図に示します。
  
**図 1 です。バックアップと復元システムのアーキテクチャ**

![バックアップおよび復元アプリケーションがやり取りする方法を示す図。Exchange、Windows Server とクライアント アプリケーションの間に双方向通信が存在します。Windows Server は大容量記憶装置またはバックアップ メディアともやり取りします。](media/VSS_architecture_E2k7.gif)
  
バックアップと復元のアプリケーションは、VSS リクエスターとして機能します。 依頼者は、VSS シャドウ ・ コピーの作成を開始して、バックアップ用のデータにアクセスするのには、Exchange 2013 の情報を取得すると通信します。 
  
Exchange ストアは Exchange 2013 のコンポーネントであり、Windows サーバーのファイル システムを介して Exchange 2013 のデータベースにアクセスします。 ファイル ・ システム内の各 Exchange サーバーは、付属のデータベース (.edb) ファイル、トランザクション ログ ファイルおよびチェックポイント ファイルに最大 100 個のデータベースを同時にマウントできます。
  
VSS をサポートするためには、Exchange 2013 には、Exchange ストアに組み込まれている Exchange ライターが含まれています。 Exchange 書き込みプログラムを凍結し、それをバックアップする前にデータベースのマウントを解除 (依頼者の代理として動作)、Exchange ストアと連携してと、固定を解除して、バックアップ後のデータベースのマウントを完了します。 復元中は、バックアップと復元アプリケーションは、Exchange ストア データベースのマウントを解除、データベース ファイルを交換して、データベースをマウントおよび (必要に応じて) にトランザクション ログを再生するを調整するための Exchange ライターを指示します。
  
またリクエスターは、復元時にも VSS と通信し、復元に対応するためにシステムの準備を整えてから、大容量記憶装置にデータを戻します。バックアップと復元アプリケーションも Windows Server と連携し、バックアップ記憶領域メディア (テープ アーカイブ、記憶域ネットワーク、その他のバックアップ メディア) からのデータの読み取りとデータの書き込みを行います。
  
復元されたデータベースは、通常、アクティブなデータベース、または Exchange 2013 の回復用データベースとしてマウントできます。 1 つだけマウントされたデータベースは、各 Exchange サーバー上の回復用データベースとして指定できます。
  
バックアップを完了し、VSS では、Exchange 2013 の間での操作を復元するために必要な情報と、バックアップと復元のアプリケーションは、Exchange ライターのメタデータの一部として転送されます。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [2013 の Exchange データベースを復元します。](restoring-exchange-2013-databases.md)
    
- [Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Exchange 2013 の Eseutil ツールを使用してバックアップの整合性を検証します。](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange のバックアップ/リストア](backup-and-restore-for-exchange-2013.md) 
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md) 
- [ボリューム シャドウ コピー サービス](http://msdn.microsoft.com/en-us/library/bb968832%28VS.85%29.aspx) 
- [Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

