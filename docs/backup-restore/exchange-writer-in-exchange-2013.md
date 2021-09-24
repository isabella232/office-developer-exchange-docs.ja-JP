---
title: Exchange 2013 の Exchange ライター
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: バックアップと復元の操作に関する Exchange 2013 の Exchange ライターに関する情報を確認できます。
ms.openlocfilehash: 7c50c2aa014308b05bdbc1acf0f2a91e33717ed6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516238"
---
# <a name="exchange-writer-in-exchange-2013"></a>Exchange 2013 の Exchange ライター

バックアップと復元の操作に関する Exchange 2013 の Exchange ライターに関する情報を確認できます。 
  
**製品:** Exchange Server 2013 
  
2013 Exchange 2013 データベースのバックアップと復元は、Exchange Server作成者が担当します。 また、Exchange ライターは、データベースやトランザクション ログ ファイルのレプリケートされたインスタンスのシャドー コピーが作成される、選択したデータベースのバックアップ機能もサポートしています。 
  
## <a name="overview-of-the-exchange-writer"></a>Exchange ライターの概要
<a name="bk_Overview"> </a>

Exchange 2013 には、データベース モビリティ機能が含まれています。この機能を使用すると、データベースの可用性とサイトの復元性を向上Exchangeサーバー間でデータベースをレプリケートできます。 データベース可用性グループ (DAG) の他のデータベース コピーは、Exchange バックアップがコピー場所で利用可能な追加のリソースを使用する貴重な機会となります。 また、アクティブなデータベース マスターの代わりにコピーがバックアップされたため、バックアップ中にコピーを使用できなくなった期間が長くなります。 
  
Exchange ライターは Exchange サービス (リクエスターのために動作) と連携して、バックアップに備えてデータベース ファイルを準備し、データベースをバックアップする前に Exchange トランザクションの結果として生じる IO アクティビティを固定します。その後、バックアップが完了してから、ログ ファイルの固定を解除して切り詰めます。
  
復元中、バックアップと復元アプリケーションは、(リクエスターのために動作する) Exchange ストアと連携して、復元ターゲットの検証、データベース ファイルの名前変更 (必要な場合)、必要に応じてトランザクション ログの再生を行うよう Exchange ライターに指示します。Exchange ライターは、バックアップと復元の両方をサポートします。
  
Exchange ライターは、メールボックス サーバーの役割がインストールされている Exchange サーバーで利用できます。 
  
## <a name="exchange-writer-configuration-settings"></a>Exchange ライターの構成設定 
<a name="bk_ExchangeWriterConfig"> </a>

VSS 用の Exchange ライターは、正しく設定され、バックアップと復元の操作中に保持されることが必要な各種設定と値を使います。これらの構成設定は、Exchange ライターのメタデータ ドキュメントに格納されます。バックアップ アプリケーションがこれらの設定を保持しない場合、Exchange データベースのバックアップを試みると予期しないエラーが発生する可能性があります。  
  
以下の表は、データベース バックアップのコンポーネントに関するメタデータを公開する VSS インタ フェースを一覧表示します。これらのインターフェイスは、Exchange ストアのバックアップに使う Exchange ライター メタデータ ドキュメントを取得するときに必要です。
  
**表 1.VSS インターフェイス**

|**VSS インターフェイス**|**説明**|
|:-----|:-----|
|IVssWMComponent  <br/> |Exchange ライターに格納されているコンポーネント情報にアクセスできるようにします。  <br/> |
|IVssExamineWriterMetadata  <br/> |要求元のバックアップと復元アプリケーションが、アプリケーションライターのメタデータをExchangeします。 Exchangeライター メタデータ ドキュメントには、バックアップと復元を要求するアプリケーションが必要とする Exchange 2013 固有の値とパラメーターが含まれているので、バックアップに適切なコンポーネントを正しく指定できます。  <br/> |
|IVssComponent  <br/> |リクエスターのバックアップ コンポーネント ドキュメントに含まれるコンポーネントに関する情報を調べて変更するメソッドが含まれます。 オブジェクトは [、IVssBackupComponents::AddComponent](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx) メソッドによってこのドキュメントに明示的に追加されたコンポーネントに対してしか取得できません。  <br/> |
|IVssBackupComponents  <br/> |リクエスターのバックアップと復元アプリケーションが、ファイルの状態について Exchange ライターをポーリングし、バックアップと復元の操作を実行するために使います。 [IVssBackupComponents::SetBackupState](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx)メソッドは、バックアップ操作が完全バックアップ、コピーバックアップ、増分バックアップ、または差分バックアップであるかどうかを定義します。 [IVssBackupComponents::AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx)メソッドは、復元操作で選択できる Exchange 2013 データベースのサブコンポーネントを定義します。  <br/> |
   
Windows Server ファイル システム内では、Exchange 2013 データベースは、拡張子が .edb の 1 つのデータベース ファイル *として格納されます。Exchangeライターは *.edb** をデータベース コンポーネントとして公開し、トランザクション ログ ( .log) とチェックポイント ファイル ( .chk) は、ログ コンポーネントと呼ばれる 1 つのコンポーネントに結合されます。 データベース ファイルの詳細については、「Exchange [2013](backup-and-restore-concepts-for-exchange-2013.md)のバックアップと復元のExchange参照してください。
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Exchange ライター、VSS、VSS リクエスター間の相互作用
<a name="bk_interactions"> </a>

バックアップ操作中の VSS、Exchangeライタ、および 2013 Exchangeの間の高レベルの相互作用は次のとおりです。
  
1. バックアップ プログラム (またはエージェント) がスケジュールされたジョブを実行します。 
    
2. バックアップおよび復元アプリケーションの VSS 要求元は、VSS にコマンドを送信して、2013 データベースで選択したデータベースのシャドウ コピー Exchangeします。 
    
3. VSS は、スナップショット バックアップExchange準備するために、作成者と通信します。 Exchange 2013 では、データベースに対する管理アクションを禁止し、ボリュームの依存関係をチェックし、読み取り専用アクセスを許可しながら、データベースおよびトランザクション ログ ファイルの選択したインスタンスへのすべての書き込み操作を中断します。 
    
4. VSS は、適切なストレージ プロバイダーと通信して、2013 データベースを含むストレージ ボリュームのシャドウ コピー Exchange作成します。 
    
5. VSS は、通常Exchange再開するために 2013 年にリリースされます。 
    
6. VSS リクエスターは、バックアップが正常に完了したことを通知する前にバックアップ セットの物理的な整合性を検証します。 Exchange 2013 では、トランザクション ログが切り捨てられ (データベースが DAG の一部である場合は、すべてのコピー間でログの切り捨てがレプリケートされます)、データベースの最後のバックアップの時刻が記録されます。
    
VSS は[、OnPrepareBackup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx)メソッドで始Exchange [OnPostSnapshot](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx)メソッドで終わる、要求者と Exchangeの対話をシリアル化します。 バックアップの完了前にシャドウ コピーの整合性が検証される際、通常、Exchange ライターは、**OnPostSnapshot** メソッドの後に発生するシャドウ コピーの処理にほとんどの時間を費やします。 このExchangeは **、OnPostSnapshot** と [OnBackupComplete の間の並列バックアップをサポートします](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx)。
  
Exchange 2013 では、同じデータベースの同時バックアップは許可されません。 特定のデータベースに対して一度に実行できるのは 1 つのバックアップ ジョブのみです。 バックアップの実行中、Exchange ストアにより、データベースはバックアップ進行中状態になります。 このメモリ内の状態は、バックアップ プロセスの完了時かサービスの再起動時のいずれかにクリアされます。 メモリ内のバックアップ進行中状態とその関連データは、Exchange ライターをホストするサービスを再起動するとき、オペレーティング システムを再起動するとき、クラスターのフェールオーバーが発生するときのいずれかの場合に失われます。 こうしたイベントは、バックアップ ジョブが失敗する原因となります。
  
実行するバックアップの種類に基づいて、バックアップ開始トランザクション ログ ファイルの切り詰めがトリガーされます。DAG 以外の構成では、Exchange ライターは、完全バックアップや増分バックアップが正常に完了したときにトランザクション ログ ファイルを切り詰めます。DAG のレプリケートされた構成では、すべての必要なログ ファイルが他のすべてのコピーに再生されるまで、レプリケーション サービスによってログの切り詰めが遅延されます。レプリケーション サービスは、アクティブなログ ファイル パスとコピー ログ ファイル パスの両方からバックアップ ログ ファイルを削除します。この削除は、ログ ファイルがコピー データベースに正常に適用され、アクティブ データベースとデータベース コピー チェックポイントの両方が削除対象のログ ファイルを渡したことを確認した後に行われます。
  
## <a name="see-also"></a>関連項目

- [Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

