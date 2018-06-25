---
title: Exchange 2013 のデータベースを復元する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: 2013 の Exchange データベースを復元することができますさまざまな方法に関する情報を検索します。
ms.openlocfilehash: d3ca3a884b0ad30f7d7968a9ed435b02aaf205e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758891"
---
# <a name="restoring-exchange-2013-databases"></a>Exchange 2013 のデータベースを復元する

2013 の Exchange データベースを復元することができますさまざまな方法に関する情報を検索します。 
  
**に適用されます:** Exchange Server 2013 
  
含まれているでは、Exchange Server 2013 は、Exchange データベースを復元する方法のいくつかの柔軟性によって、Exchange ライター。 Exchange 書き込みプログラムを使用して、Exchange 2013 で、次の場所に、シャドウ コピー バックアップを復元できます。
  
- 元のデータベース。データベースやトランザクション ログ ファイルのパス構成が変更されているかどうかは関係ありません。
    
- 回復用データベース。
    
- 実稼働データベース。データベースの表示名が VSS バックアップ セットの名前と一致しているかどうかは関係ありません。
    
復元アプリケーションでは、元のデータベースに情報を復元、ときに、そのデータベースの Active Directory ドメイン サービス (AD DS) で指定されたディレクトリのパスにログ ファイルを復元しなければなりません。 場合は、アプリケーションでは、別の場所にデータベースを復元、データベースのログ ファイルのディレクトリ内にある **_restoredLogs**をという名前のフォルダーにログ ファイルを復元しなければなりません。 
  
サーバーまたは元のデータベースとは異なるデータベースを復元して、復元アプリケーションは必ず VSS に用意されているデータベース ・ ディレクトリ ・ パスと一致している AD DS の。 [Get MailboxDatabase](http://technet.microsoft.com/en-us/library/bb124924%28v=exchg.150%29.aspx)Exchange 管理シェル コマンドレットを使用すると、既存のデータベースに関する情報を取得します。 Exchange 管理シェルの詳細については、 [Exchange Server PowerShell (Exchange 管理シェル)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。 
  
次の図は、ボリューム シャドウ コピー サービス (VSS) で管理されている Exchange データベースの一般的な復元でのイベントのシーケンスを示しています。
  
**図 1 です。データベースを復元するためのイベントの順序**

![復元プロセスのイベント シーケンスを示す図。シーケンスは、Exchange ストアの起動から始まり、Exchange ライター、VSS、およびクライアント アプリケーションの間での多くのステップが続きます。](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>元の場所への Exchange データベースの復元
<a name="bk_OriginalLocation"> </a>

Exchange 書き込みプログラムは、Exchange サーバー上の元の場所にデータベースとトランザクション ログ ファイルを復元するアプリケーションを有効にします。 既定では、Exchange ライターは、依頼者は、 [OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中に復元が完了したことを確認した後にトランザクション ログ ファイルを再生します。 リストア ・ アプリケーションは、ログ ファイルを再生することを防ぐために、VSS の[SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx)メソッドを使用する必要があります。 Exchange 管理者またはアプリケーションが復元されたデータベースを再マウントすると後でログ ファイルを再生することができます。 
  
(バックアップ セットのデータベース内のターゲットの Guid と一致) するようにオブジェクトの元のデータベースにデータベースを復元するが、別のファイルのパスにアプリケーションし必要があります現在のファイル パスを決定するバックアップ ファイルを復元します対応するファイルのパスがデータベースのプロパティで指定します。 依頼者は、Exchange ライターに、ファイルのリストア ・ プロセスの残りの部分とライターを続行するに復元する場所を通信するために[AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出す必要があります。 **AddNewTarget**が呼び出されない場合、Exchange 書き込みプログラムはバックアップ メタデータ ドキュメントで指定されたファイルのパスをバックアップを復元することと仮定します。 
  
通常、カスタムのアプリケーションでは、データベース可用性グループ (DAG) のコピーから実行するバックアップに新しいパスを指定する必要はありません。Exchange 管理者は、通常はデータベースやログ ファイルのパスを変更しません。ただし、DAG 構成では、アクティブなデータベースとログのパスをバックアップ アプリケーションで指定することが必要になることがあります (それらのパスと DAG コピーのパスは常に異なるため)。
  
非アクティブな DAG のデータベースのコピーを復元するをサポートしていない Exchange 2013 ことに注意してください。 DAG のコピーは、アクティブなデータベースのコピーが復元されたときにのみバックアップ データから復元できます。 別のバックアップ データ セットを使用するか、データベースのコピーの一部を復元しようとしています。 データベースをマウントが発生することができます。 作成された元のデータベース オブジェクトを復元するためのバックアップ ・ アプリケーションではこの例では、 [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx)関数を呼び出す必要はありません。 ただし、バックアップ ・ アプリケーションは、 **SetRestoreOptions**を呼び出して、XML メタデータ ドキュメントは、適切なパラメーターを持つ場合は、エラーが発生しない、します。 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Exchange データベースの回復用データベースへの復元
<a name="bk_RecoveryDatabase"> </a>

Exchange ライターを使用すると、回復用のデータベースに直接データを復元できるようになります。回復したデータを回復用データベースとしてマウントすると、Exchange 管理者は個々のメールボックス (メールボックス内の個々のアイテムも) 復元できます。
  
回復用データベースが既に存在する場合、アプリケーションでデータベースのマウントを解除し、データを回復用データベースとログ ファイルに復元して、データベースを再度マウントできます。
  
各 Exchange 2013 サーバーでは、1 つだけの回復用データベースを同時にマウントします。 サーバーは、ディスクの空き領域が許可されているが、1 つだけは、回復用データベースとしてマウントできるよう多くのリカバリされたデータベースを含めることができます。 回復用データベースとしてマウントされているデータベースは、一度にマウントできるデータベースの最大数にカウントされます。 サーバーの回復用データベースがどのような方法で元のメールボックスに関連付けられているではないために、復元されたデータベースがマウントされます。
  
回復用データベースに復元するに、アプリケーション必要があります[SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx)メソッドを呼び出すソースを示す XML ドキュメントを提供してデータベース Guid を対象とします。 ソース Guid と一致しなければなりません、バックアップ ・ セットからとターゲット Guid が AD DS に転送先データベースのエントリと一致する必要があります。 バックアップ ・ アプリケーションでは、ディレクトリのパスにファイルを復元する場所を指定する[AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出す必要がありますもします。 データベース ファイルの名前を変更する場合は、Exchange ライターは[OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中にデータベースを変更します。 Exchange では、現在のトランザクション ログ ファイルのパスの下にある ( **_restoredLogs**) のサブフォルダーに復元するトランザクション ログ ファイルが必要です。 ログ ファイルは、他の任意の場所に復元は、Exchange 書き込みプログラムはエラーを返します。 回復用データベースとしてマウントされているデータベースが元の場所に復元されないため、それらをマウントする前にクリーン シャット ダウン状態になる必要があります。 既定では、Exchange 書き込みプログラムが表示されます復元されたすべてのデータベースをクリーン シャット ダウン状態に post-restore の中に。 バックアップ ・ アプリケーションは、 [SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx)メソッドを呼び出し、Exchange ライターは、ログ ファイルを再生、および、管理者またはバックアップ ・ アプリケーション、データベースをマウントする前にクリーン シャット ダウン状態に移動する必要があります場合、。データベースです。 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Exchange データベースの回復用サーバーへの復元
<a name="bk_RecoveryServer"> </a>

一部のシナリオでは別のサーバーにバックアップ セットを復元する必要があります。などに、同じ Exchange 組織内の別の Exchange 2013 サーバーにメールボックス データベースの移植で致命的なサーバー障害から回復するか、メールボックスを回復するのには本番環境の外部の専用のサーバーに復元する必要があり、パブリック フォルダーのデータです。 
  
これらのシナリオでそのオブジェクトの Guid だけでなく、ターゲット データベースのファイル パスが元のデータベースのものとは異なる。 したがって、アプリケーションがソースとターゲット データベースの情報を復元するバックアップ ファイルへのディレクトリ パスを指定するのには、 [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドの呼び出しを示す XML ドキュメントで[SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx)メソッドを呼び出し、します。. Exchange ライターの場合、このリストアとは、回復用データベースを復元すると同じです。 詳細については、この資料の以前のバージョン[を復元する Exchange データベースの回復用データベース](restoring-exchange-2013-databases.md#bk_RecoveryDatabase)を参照してください。 
  
## <a name="see-also"></a>関連項目
<a name="bk_AdditionalResources"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [バックアップを作成し、Exchange 2013 のアプリケーションを復元します。](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
    

