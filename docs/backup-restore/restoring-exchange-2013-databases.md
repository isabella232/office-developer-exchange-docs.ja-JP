---
title: Exchange 2013 のデータベースを復元する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: 2013 年のデータベースを復元するさまざまな方法Exchangeします。
ms.openlocfilehash: 522128026bcbef893ce4909174d3fd9a95f1e8a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513277"
---
# <a name="restoring-exchange-2013-databases"></a>Exchange 2013 のデータベースを復元する

2013 年のデータベースを復元するさまざまな方法Exchangeします。 
  
**製品:** Exchange Server 2013 
  
2013 Exchange 2013 に含まれる Exchange Serverライターを使用すると、データベースの復元方法を柔軟にExchangeできます。 2013 Exchange 2013 で Exchangeライターを使用すると、シャドウ コピーのバックアップを次の場所に復元できます。
  
- 元のデータベース。データベースやトランザクション ログ ファイルのパス構成が変更されているかどうかは関係ありません。
    
- 回復用データベース。
    
- 実稼働データベース。データベースの表示名が VSS バックアップ セットの名前と一致しているかどうかは関係ありません。
    
復元アプリケーションで元のデータベースに情報を復元する場合は、そのデータベースに対して Active Directory ドメイン サービス (AD DS) で指定されたディレクトリ パスにログ ファイルが復元されている必要があります。復元アプリケーションで別の場所にデータベースを復元する場合は、データベース ログ ファイルのディレクト内に配置された **_restoredLogs** という名前のフォルダーにログ ファイルが復元されている必要があります。 
  
元のデータベースとは別のサーバーまたはデータベースに復元する場合は、VSS に指定されたデータベース ディレクトリのパスが AD DS のパスと一致していることを復元アプリケーションで確認する必要があります。 [get-MailboxDatabase コマンドレットを](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)Exchange既存のデータベースに関する情報を取得できます。 Exchange 管理シェルの詳細については、[「Exchange サーバー PowerShell (Exchange 管理シェル) 」](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)を参照してください。 
  
次の図は、ボリューム シャドウ コピー サービス (VSS) で管理されている Exchange データベースの一般的な復元でのイベントのシーケンスを示しています。
  
**図 1データベースを復元するためのイベントのシーケンス**

![復元プロセスのイベント シーケンスを示す図。シーケンスは、Exchange ストアの起動から始まり、Exchange ライター、VSS、およびクライアント アプリケーションの間での多くのステップが続きます。](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>元の場所への Exchange データベースの復元
<a name="bk_OriginalLocation"> </a>

Exchange ライターにより、アプリケーションで Exchange サーバー上のデータベースとトランザクション ログ ファイルをそれぞれの元の場所に復元できます。 既定では、Exchange作成者は[、OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中に復元が完了したと要求者が確認した後、トランザクション ログ ファイルを再生します。 ログ ファイルの再生を防止するには、復元アプリケーションで VSS [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) メソッドを使用する必要があります。 このログ ファイルは、復元したデータベースを Exchange 管理者またはアプリケーションが再マウントするときに後から再生できます。 
  
データベースを元のデータベース オブジェクト (データベースのターゲット GUID とバックアップ セットの GUID が同じになるもの) に復元するときに、ファイル パスを別のものにする場合は、アプリケーションで現在のファイル パスを判断して、それに対応するデータベースのプロパティで指定されたファイル パスにバックアップ ファイルを復元する必要があります。 要求者は[AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出して、Exchange ライターにファイルが復元される場所と通信してから、ライターが残りの復元プロセスを続行する必要があります。 **AddNewTarget** が呼び出されていないと、Exchange ライターはバックアップがバックアップ メタデータ ドキュメントで指定されたファイル パスに復元されると想定します。 
  
通常、カスタムのアプリケーションでは、データベース可用性グループ (DAG) のコピーから実行するバックアップに新しいパスを指定する必要はありません。Exchange 管理者は、通常はデータベースやログ ファイルのパスを変更しません。ただし、DAG 構成では、アクティブなデータベースとログのパスをバックアップ アプリケーションで指定することが必要になることがあります (それらのパスと DAG コピーのパスは常に異なるため)。
  
2013 Exchangeは、非アクティブな DAG データベース コピーの復元をサポートしていない点に注意してください。 DAG コピーは、アクティブなデータベース コピーが復元された場合にのみ、バックアップ データから復元できます。 異なるバックアップ データ セットを使用するか、データベース コピーのサブセットを復元しようとすると、データベースがマウントできない可能性があります。 バックアップ アプリケーションは、作成元の元のデータベース オブジェクトにバックアップが復元されるので、この場合は [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) 関数を呼び出す必要はありません。 ただし、バックアップ アプリケーションが **SetRestoreOptions** を呼び出し、XML メタデータ ドキュメントに正しいパラメーターがある場合、結果はエラーではありません。 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Exchange データベースの回復用データベースへの復元
<a name="bk_RecoveryDatabase"> </a>

Exchange ライターを使用すると、回復用のデータベースに直接データを復元できるようになります。回復したデータを回復用データベースとしてマウントすると、Exchange 管理者は個々のメールボックス (メールボックス内の個々のアイテムも) 復元できます。
  
回復用データベースが既に存在する場合、アプリケーションでデータベースのマウントを解除し、データを回復用データベースとログ ファイルに復元して、データベースを再度マウントできます。
  
各Exchange 2013 サーバーでは、一度にマウントできる回復データベースは 1 つのみです。 サーバーにはディスク容量に余裕がある限り多くの回復されたデータベースを格納できますが、回復用データベースとしては 1 つのみがマウントできます。 回復用データベースとしてマウントされたデータベースは、同時にマウントできるデータベースの最大数にカウントされます。 サーバーの回復データベースとしてマウントされた回復されたデータベースは、元のメールボックスに関連付けされません。
  
回復データベースに回復するには、アプリケーションで [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) メソッドを呼び出し、ソース データベースとターゲット データベースの GUID を示す XML ドキュメントを指定する必要があります。 ソースの GUID はバックアップ セットの GUID と一致する必要があり、ターゲットの GUID は AD DS の復元先データベースのエントリと一致している必要があります。 バックアップ アプリケーションでは [、AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) メソッドを呼び出して、ファイルの復元先のディレクトリ パスを指定する必要もあります。 データベース ファイルの名前を変更する必要がある場合は[、OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中Exchange書き込み元がデータベースの名前を変更します。 Exchange、トランザクション ログ ファイルを現在のトランザクション ログ ファイル パスのサブフォルダー (_restoredLogs) に復元する必要があります。 このログ ファイルが別の場所に復元されると、Exchange ライターはエラーを返します。 回復用データベースとしてマウントされるデータベースは元の場所には復元されないため、マウントする前にクリーン シャットダウン状態にする必要があります。 既定では、Exchange ライターは、復元したすべてのデータベースを復元後の手順でクリーン シャットダウン状態にします。 バックアップ アプリケーションが[SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx)メソッドを呼び出す場合、Exchange ライターはログ ファイルを再生しません。管理者またはバックアップ アプリケーションは、データベースをマウントする前に、データベースをクリーン シャットダウン状態に戻す必要があります。 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Exchange データベースの回復用サーバーへの復元
<a name="bk_RecoveryServer"> </a>

一部のシナリオでは、別のサーバーにバックアップ セットを回復する必要がある場合があります。たとえば、メールボックス データベースを同じ Exchange 組織内の別の Exchange 2013 サーバーに移植したり、実稼働環境外の専用サーバーに復元してメールボックスとパブリック フォルダーのデータを回復したりして、壊滅的なサーバー障害から回復する必要がある場合があります。 
  
このようなシナリオでは、ターゲット データベースのファイル パスとオブジェクト GUID は、どちらも元のものとは異なります。 したがって、アプリケーションは、ソースデータベースとターゲット データベース情報を示す XML ドキュメントを使用して [SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) メソッドを呼び出し [、AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) メソッドを呼び出してバックアップ ファイルを復元するディレクトリ パスを指定する必要があります。 Exchange ライターの場合、この復元は、回復用データベースへの復元と同じになります。 詳細については、この記事の[「Exchangeデータベースへの復元](restoring-exchange-2013-databases.md#bk_RecoveryDatabase)」を参照してください。 
  
## <a name="see-also"></a>関連項目
<a name="bk_AdditionalResources"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元アプリケーションの作成](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
    

