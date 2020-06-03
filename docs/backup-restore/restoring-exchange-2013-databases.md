---
title: Exchange 2013 のデータベースを復元する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Exchange 2013 データベースを復元するさまざまな方法についての情報を参照してください。
ms.openlocfilehash: 9fe417bda5dc728af619da02d62ada6e920f731d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528674"
---
# <a name="restoring-exchange-2013-databases"></a>Exchange 2013 のデータベースを復元する

Exchange 2013 データベースを復元するさまざまな方法についての情報を参照してください。 
  
**製品:** Exchange Server 2013 
  
Exchange Server 2013 に含まれている Exchange ライターを使用すると、Exchange データベースを柔軟に復元できます。 Exchange 2013 の Exchange ライターを使用すると、シャドウコピーバックアップを次の場所に復元できます。
  
- 元のデータベース。データベースやトランザクション ログ ファイルのパス構成が変更されているかどうかは関係ありません。
    
- 回復用データベース。
    
- 実稼働データベース。データベースの表示名が VSS バックアップ セットの名前と一致しているかどうかは関係ありません。
    
復元アプリケーションで元のデータベースに情報を復元する場合は、そのデータベースに対して Active Directory ドメイン サービス (AD DS) で指定されたディレクトリ パスにログ ファイルが復元されている必要があります。 復元アプリケーションで別の場所にデータベースを復元する場合は、データベース ログ ファイルのディレクト内に配置された **_restoredLogs** という名前のフォルダーにログ ファイルが復元されている必要があります。 
  
元のデータベースとは別のサーバーまたはデータベースに復元する場合は、VSS に指定されたデータベース ディレクトリのパスが AD DS のパスと一致していることを復元アプリケーションで確認する必要があります。 [Set-mailboxdatabase](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)Exchange 管理シェルコマンドレットを使用して、既存のデータベースに関する情報を取得できます。 Exchange 管理シェルの詳細については、「 [Exchange Server PowerShell (Exchange Management shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)」を参照してください。 
  
次の図は、ボリューム シャドウ コピー サービス (VSS) で管理されている Exchange データベースの一般的な復元でのイベントのシーケンスを示しています。
  
**図 1データベースを復元するためのイベントのシーケンス**

![復元プロセスのイベント シーケンスを示す図。シーケンスは、Exchange ストアの起動から始まり、Exchange ライター、VSS、およびクライアント アプリケーションの間での多くのステップが続きます。](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>元の場所への Exchange データベースの復元
<a name="bk_OriginalLocation"> </a>

Exchange ライターにより、アプリケーションで Exchange サーバー上のデータベースとトランザクション ログ ファイルをそれぞれの元の場所に復元できます。 既定では、Exchange ライターは、要求者が[Onpostrestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中に復元が完了したことを確認した後、トランザクションログファイルを再生します。 復元アプリケーションでは、ログファイルが再生されないように VSS [Setadditionalrestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx)メソッドを使用する必要があります。 このログ ファイルは、復元したデータベースを Exchange 管理者またはアプリケーションが再マウントするときに後から再生できます。 
  
データベースを元のデータベース オブジェクト (データベースのターゲット GUID とバックアップ セットの GUID が同じになるもの) に復元するときに、ファイル パスを別のものにする場合は、アプリケーションで現在のファイル パスを判断して、それに対応するデータベースのプロパティで指定されたファイル パスにバックアップ ファイルを復元する必要があります。 リクエスターは、ファイルの復元先として Exchange ライターと通信するために、 [Addnewtarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出して、残りの復元プロセスでライターを続行できるようにする必要があります。 **AddNewTarget** が呼び出されていないと、Exchange ライターはバックアップがバックアップ メタデータ ドキュメントで指定されたファイル パスに復元されると想定します。 
  
通常、カスタムのアプリケーションでは、データベース可用性グループ (DAG) のコピーから実行するバックアップに新しいパスを指定する必要はありません。Exchange 管理者は、通常はデータベースやログ ファイルのパスを変更しません。ただし、DAG 構成では、アクティブなデータベースとログのパスをバックアップ アプリケーションで指定することが必要になることがあります (それらのパスと DAG コピーのパスは常に異なるため)。
  
Exchange 2013 では、非アクティブな DAG データベースコピーの復元がサポートされていないことに注意してください。 DAG コピーは、アクティブデータベースコピーが復元された場合にのみ、バックアップデータから復元できます。 異なるバックアップデータセットを使用するか、データベースコピーのサブセットを復元しようとすると、データベースが unmountable になることがあります。 バックアップアプリケーションは、作成元のデータベースオブジェクトに復元されるため、この場合、 [Setrestoreoptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx)関数を呼び出す必要はありません。 ただし、バックアップアプリケーションが**Setrestoreoptions**を呼び出し、XML メタデータドキュメントに正しいパラメーターがある場合、結果はエラーではありません。 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Exchange データベースの回復用データベースへの復元
<a name="bk_RecoveryDatabase"> </a>

Exchange ライターを使用すると、回復用のデータベースに直接データを復元できるようになります。回復したデータを回復用データベースとしてマウントすると、Exchange 管理者は個々のメールボックス (メールボックス内の個々のアイテムも) 復元できます。
  
回復用データベースが既に存在する場合、アプリケーションでデータベースのマウントを解除し、データを回復用データベースとログ ファイルに復元して、データベースを再度マウントできます。
  
各 Exchange 2013 サーバーは、一度に1つの回復用データベースのみをマウントできます。 サーバーにはディスク容量に余裕がある限り多くの回復されたデータベースを格納できますが、回復用データベースとしては 1 つのみがマウントできます。 回復用データベースとしてマウントされたデータベースは、同時にマウントできるデータベースの最大数にカウントされます。 回復用データベースがサーバーの回復用データベースとしてマウントされている場合、どのような方法でも元のメールボックスには関連付けられていません。
  
回復用データベースに回復するには、アプリケーションで[Setrestoreoptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx)メソッドを呼び出し、ソースデータベースとターゲットデータベースの guid を示す XML ドキュメントを指定する必要があります。 ソースの GUID はバックアップ セットの GUID と一致する必要があり、ターゲットの GUID は AD DS の復元先データベースのエントリと一致している必要があります。 また、バックアップアプリケーションは、ファイルの復元先のディレクトリパスを指定するために、 [Addnewtarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出す必要があります。 データベースファイルの名前を変更する必要がある場合、Exchange ライターは[Onpostrestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx)操作中にデータベースの名前を変更します。 Exchange では、トランザクションログファイルを現在のトランザクションログファイルパスの下にあるサブフォルダー ( **_restoredLogs**) に復元する必要があります。 このログ ファイルが別の場所に復元されると、Exchange ライターはエラーを返します。 回復用データベースとしてマウントされるデータベースは元の場所には復元されないため、マウントする前にクリーン シャットダウン状態にする必要があります。 既定では、Exchange ライターは、復元したすべてのデータベースを復元後の手順でクリーン シャットダウン状態にします。 バックアップアプリケーションが[Setadditionalrestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx)方法を呼び出した場合、Exchange ライターはログファイルを再生しないで、管理者またはバックアップアプリケーションはデータベースをマウントする前に、データベースをクリーンシャットダウン状態にする必要があります。 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Exchange データベースの回復用サーバーへの復元
<a name="bk_RecoveryServer"> </a>

シナリオによっては、バックアップセットを別のサーバーに復元する必要があります。たとえば、メールボックスデータベースを同じ Exchange 組織内の別の Exchange 2013 サーバーに移行することによって、またはメールボックスとパブリックフォルダーのデータを回復するために、運用環境外の専用サーバーに復元することによって、致命的なサーバー障害から回復する必要がある場合があります。 
  
このようなシナリオでは、ターゲット データベースのファイル パスとオブジェクト GUID は、どちらも元のものとは異なります。 そのため、アプリケーションでは、ソースデータベースとターゲットデータベースの情報を示す XML ドキュメントを使用して[Setrestoreoptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx)メソッドを呼び出し、 [addnewtarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx)メソッドを呼び出して、バックアップファイルの復元先のディレクトリパスを指定する必要があります。 Exchange ライターの場合、この復元は、回復用データベースへの復元と同じになります。 詳細については、この記事の「 [Exchange データベースの回復用データベースへの復元](restoring-exchange-2013-databases.md#bk_RecoveryDatabase)」を参照してください。 
  
## <a name="see-also"></a>関連項目
<a name="bk_AdditionalResources"> </a>

- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元アプリケーションの作成](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    
- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
    

