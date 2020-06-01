---
title: Exchange 2013 の Exchange ライター
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: バックアップと復元の操作に関する Exchange 2013 の Exchange ライターに関する情報を確認できます。
ms.openlocfilehash: 44270a87c38b08d274d389fa6e46f3864da13ed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452889"
---
# <a name="exchange-writer-in-exchange-2013"></a>Exchange 2013 の Exchange ライター

バックアップと復元の操作に関する Exchange 2013 の Exchange ライターに関する情報を確認できます。 
  
**製品:** Exchange Server 2013 
  
Exchange ライターは、アクティブな Exchange Server 2013 データベースのバックアップと復元を担当します。 また、Exchange ライターは、データベースやトランザクション ログ ファイルのレプリケートされたインスタンスのシャドー コピーが作成される、選択したデータベースのバックアップ機能もサポートしています。 
  
## <a name="overview-of-the-exchange-writer"></a>Exchange ライターの概要
<a name="bk_Overview"> </a>

Exchange 2013 にはデータベースのモビリティ機能が含まれており、データベースを異なる Exchange サーバー間でレプリケートして、データベースの可用性とサイトの復元性を向上させることができます。 データベース可用性グループ (DAG) 内の他のデータベースコピーは、コピー先で利用可能なその他のリソースを使用するための、Exchange バックアップの貴重な機会を提供します。 さらに、アクティブデータベースマスターの代わりにコピーがバックアップされるため、バックアップ中にコピーを使用できなくなることがあります。 
  
Exchange ライターは Exchange サービス (リクエスターのために動作) と連携して、バックアップに備えてデータベース ファイルを準備し、データベースをバックアップする前に Exchange トランザクションの結果として生じる IO アクティビティを固定します。その後、バックアップが完了してから、ログ ファイルの固定を解除して切り詰めます。
  
復元中、バックアップと復元アプリケーションは、(リクエスターのために動作する) Exchange ストアと連携して、復元ターゲットの検証、データベース ファイルの名前変更 (必要な場合)、必要に応じてトランザクション ログの再生を行うよう Exchange ライターに指示します。Exchange ライターは、バックアップと復元の両方をサポートします。
  
Exchange ライターは、メールボックス サーバーの役割がインストールされている Exchange サーバーで利用できます。 
  
## <a name="exchange-writer-configuration-settings"></a>Exchange ライターの構成設定 
<a name="bk_ExchangeWriterConfig"> </a>

VSS 用の Exchange ライターは、正しく設定され、バックアップと復元の操作中に保持されることが必要な各種設定と値を使います。これらの構成設定は、Exchange ライターのメタデータ ドキュメントに格納されます。バックアップ アプリケーションがこれらの設定を保持しない場合、Exchange データベースのバックアップを試みると予期しないエラーが発生する可能性があります。  
  
以下の表は、データベース バックアップのコンポーネントに関するメタデータを公開する VSS インタ フェースを一覧表示します。これらのインターフェイスは、Exchange ストアのバックアップに使う Exchange ライター メタデータ ドキュメントを取得するときに必要です。
  
**表1VSS インターフェイス**

|**VSS インターフェイス**|**説明**|
|:-----|:-----|
|IVssWMComponent  <br/> |Exchange ライターに格納されているコンポーネント情報にアクセスできるようにします。  <br/> |
|IVssExamineWriterMetadata  <br/> |要求したバックアップおよび復元アプリケーションが、Exchange ライターのメタデータを確認できるようにします。 Exchange ライターのメタデータドキュメントには、要求のバックアップと復元アプリケーションが必要とする Exchange 2013 固有の値とパラメーターが含まれています。これにより、バックアップに適切なコンポーネントを正しく指定することができます。  <br/> |
|IVssComponent  <br/> |リクエスターのバックアップ コンポーネント ドキュメントに含まれるコンポーネントに関する情報を調べて変更するメソッドが含まれます。 オブジェクトは、 [Ivssbackupcomponents:: AddComponent](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx)メソッドによってこのドキュメントに明示的に追加されたコンポーネントに対してのみ取得できます。  <br/> |
|IVssBackupComponents  <br/> |リクエスターのバックアップと復元アプリケーションが、ファイルの状態について Exchange ライターをポーリングし、バックアップと復元の操作を実行するために使います。 [Ivssbackupcomponents:: SetBackupState](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx)メソッドは、バックアップ操作がフル、コピー、増分、または差分バックアップのいずれであるかを定義します。 [Ivssbackupcomponents:: AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx)メソッドは、復元操作で選択できる Exchange 2013 データベースのサブコンポーネントを定義します。  <br/> |
   
Windows Server ファイルシステムでは、Exchange 2013 データベースは、拡張子 .edb を持つ単一のデータベースファイルとして保存されます *。Exchange ライターは*データベースコンポーネントとして .edb を公開し、トランザクションログ (*.log) とチェックポイントファイル (*.chk) は、1つのコンポーネント (ログコンポーネントと呼ばれる) に統合されます。 Exchange データベースファイルの詳細については、「 [exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)」を参照してください。
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Exchange ライター、VSS、VSS リクエスター間の相互作用
<a name="bk_interactions"> </a>

バックアップ操作時の VSS、Exchange ライター、Exchange 2013 間の高レベルの対話は、次のとおりです。
  
1. バックアップ プログラム (またはエージェント) がスケジュールされたジョブを実行します。 
    
2. バックアップおよび復元アプリケーションの VSS リクエスターは、VSS にコマンドを送信して、選択された Exchange 2013 データベースのシャドウコピーを取得します。 
    
3. VSS は、Exchange ライターと通信して、スナップショットバックアップを準備します。 Exchange 2013 は、データベースに対する管理操作を禁止し、ボリュームの依存関係をチェックし、読み取り専用アクセスを許可する一方で、データベースおよびトランザクションログファイルの選択されたインスタンスに対するすべての書き込み操作を中断します。 
    
4. VSS は適切なストレージプロバイダーと通信して、Exchange 2013 データベースが格納されているストレージボリュームのシャドウコピーを作成します。 
    
5. VSS は、Exchange 2013 を解放して、通常の操作を再開します。 
    
6. VSS リクエスターは、バックアップが正常に完了したことを通知する前にバックアップ セットの物理的な整合性を検証します。 Exchange 2013 は、トランザクションログを切り捨てます (データベースが DAG の一部である場合、ログの切り捨てがすべてのコピーでレプリケートされます)。データベースの最終バックアップ時刻を記録します。
    
VSS は、要求者の対話を、 [OnOnPostSnapshot backup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx)メソッドから始まり、 [OnPostSnapshot](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx)メソッドで終わる Exchange ライターとシリアル化します。 バックアップの完了前にシャドウ コピーの整合性が検証される際、通常、Exchange ライターは、**OnPostSnapshot** メソッドの後に発生するシャドウ コピーの処理にほとんどの時間を費やします。 Exchange ライターは、 **OnPostSnapshot**と[OnBackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx)の間の並行バックアップをサポートしています。
  
Exchange 2013 では、同じデータベースのバックアップを同時に実行することはできません。 特定のデータベースに対して一度に実行できるのは 1 つのバックアップ ジョブのみです。 バックアップの実行中、Exchange ストアにより、データベースはバックアップ進行中状態になります。 このメモリ内の状態は、バックアップ プロセスの完了時かサービスの再起動時のいずれかにクリアされます。 メモリ内のバックアップ進行中状態とその関連データは、Exchange ライターをホストするサービスを再起動するとき、オペレーティング システムを再起動するとき、クラスターのフェールオーバーが発生するときのいずれかの場合に失われます。 こうしたイベントは、バックアップ ジョブが失敗する原因となります。
  
実行するバックアップの種類に基づいて、バックアップ開始トランザクション ログ ファイルの切り詰めがトリガーされます。DAG 以外の構成では、Exchange ライターは、完全バックアップや増分バックアップが正常に完了したときにトランザクション ログ ファイルを切り詰めます。DAG のレプリケートされた構成では、すべての必要なログ ファイルが他のすべてのコピーに再生されるまで、レプリケーション サービスによってログの切り詰めが遅延されます。レプリケーション サービスは、アクティブなログ ファイル パスとコピー ログ ファイル パスの両方からバックアップ ログ ファイルを削除します。この削除は、ログ ファイルがコピー データベースに正常に適用され、アクティブ データベースとデータベース コピー チェックポイントの両方が削除対象のログ ファイルを渡したことを確認した後に行われます。
  
## <a name="see-also"></a>関連項目

- [Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

