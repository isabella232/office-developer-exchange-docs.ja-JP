---
title: Exchange 2013 の Exchange ライター
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Exchange 2013 のバックアップを Exchange ライターに関する情報を検索し、操作を復元します。
ms.openlocfilehash: a4dc5963ab24a83969efc6e425b38a35276f3aa3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758858"
---
# <a name="exchange-writer-in-exchange-2013"></a>Exchange 2013 の Exchange ライター

Exchange 2013 のバックアップを Exchange ライターに関する情報を検索し、操作を復元します。 
  
**に適用されます:** Exchange Server 2013 
  
Exchange 書き込みプログラムは、バックアップと Exchange Server 2013 のアクティブなデータベースの復元を担当します。 Exchange 書き込みプログラムには、シャドウ ・ コピーを取るようデータベースとトランザクションのレプリケートされたインスタンスに対してログ ファイルの選択したデータベースのバックアップ機能もサポートしています。 
  
## <a name="overview-of-the-exchange-writer"></a>Exchange ライターの概要
<a name="bk_Overview"> </a>

Exchange 2013 には、データベースの可用性とサイトの回復性を向上させるために別の Exchange サーバー間でレプリケートするデータベースを有効にするデータベースの移動の機能が含まれています。 他のデータベース コピー、データベース可用性グループ (DAG) では、Exchange のバックアップ コピーの場所で使用できる追加のリソースを使用するための貴重な機会を提供します。 さらに、アクティブなデータベースのマスターではなくコピーがバックアップされるため、コピーできます利用可能なバックアップ中に時間の長い期間。 
  
Exchange ライターは Exchange サービス (リクエスターのために動作) と連携して、バックアップに備えてデータベース ファイルを準備し、データベースをバックアップする前に Exchange トランザクションの結果として生じる IO アクティビティを固定します。その後、バックアップが完了してから、ログ ファイルの固定を解除して切り詰めます。
  
復元中、バックアップと復元アプリケーションは、(リクエスターのために動作する) Exchange ストアと連携して、復元ターゲットの検証、データベース ファイルの名前変更 (必要な場合)、必要に応じてトランザクション ログの再生を行うよう Exchange ライターに指示します。Exchange ライターは、バックアップと復元の両方をサポートします。
  
Exchange ライターは、メールボックス サーバーの役割がインストールされている Exchange サーバーで利用できます。  
  
## <a name="exchange-writer-configuration-settings"></a>Exchange ライターの構成設定 
<a name="bk_ExchangeWriterConfig"> </a>

VSS 用の Exchange ライターは、正しく設定され、バックアップと復元の操作中に保持されることが必要な各種設定と値を使います。これらの構成設定は、Exchange ライターのメタデータ ドキュメントに格納されます。バックアップ アプリケーションがこれらの設定を保持しない場合、Exchange データベースのバックアップを試みると予期しないエラーが発生する可能性があります。  
  
以下の表は、データベース バックアップのコンポーネントに関するメタデータを公開する VSS インタ フェースを一覧表示します。これらのインターフェイスは、Exchange ストアのバックアップに使う Exchange ライター メタデータ ドキュメントを取得するときに必要です。
  
**表 1 です。VSS インタ フェース**

|**VSS インタ フェース**|**説明**|
|:-----|:-----|
|IVssWMComponent  <br/> |Exchange ライターに格納されているコンポーネント情報にアクセスできるようにします。  <br/> |
|IVssExamineWriterMetadata  <br/> |Exchange ライターのメタデータを調べるには、要求元のバックアップと復元の次のアプリケーションを使用できます。 Exchange ライターのメタデータ ドキュメントには、Exchange 2013 に固有の値およびバックアップのための適切なコンポーネントを正しく指定することができるように、要求元のバックアップおよび復元アプリケーションが必要なパラメーターが含まれています。  <br/> |
|IVssComponent  <br/> |調べると、依頼者のバックアップ コンポーネント ドキュメントに含まれるコンポーネントについての情報を変更するためのメソッドが含まれています。 オブジェクトは、この文書に、 [IVssBackupComponents::AddComponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382646%28v=vs.85%29.aspx)メソッドによって明示的に追加されているコンポーネントにのみ取得できます。  <br/> |
|IVssBackupComponents  <br/> |ファイルのステータスに関する Exchange ライターをポーリングし、バックアップ操作と復元操作は、要求元のバックアップと復元のアプリケーションによって使用されます。 [IVssBackupComponents::SetBackupState](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382833%28v=vs.85%29.aspx)メソッドでは、バックアップ操作は、かどうか、フル ・ コピー、増分、または差分バックアップを定義します。 [IVssBackupComponents::AddRestoreSubcomponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382649%28v=vs.85%29.aspx)メソッドでは、Exchange 2013 のデータベース復元操作のために選択できるのサブコンポーネントを定義します。  <br/> |
   
*拡張子を持つ 1 つのデータベース ファイルと、Windows サーバーのファイル システム内で、Exchange 2013 のデータベースが格納されている .edb ファイルです。Exchange 書き込みプログラムを公開、*トランザクション ・ ログの中に、データベース コンポーネントと、.edb ファイル (*.log) およびチェックポイント ファイル (*.chk) ログ コンポーネントと呼ばれる、1 つのコンポーネントに結合されます。 Exchange データベース ファイルの詳細については、 [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)を参照してください。
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Exchange ライター、VSS、VSS リクエスター間の相互作用
<a name="bk_interactions"> </a>

VSS では、Exchange ライターの間で高度な相互作用し、バックアップ処理中に Exchange 2013 は、次のようにします。
  
1. バックアップ プログラム (またはエージェント) がスケジュールされたジョブを実行します。 
    
2. バックアップと復元アプリケーションの VSS リクエスターでは、選択した Exchange 2013 データベースのシャドウ ・ コピーに VSS にコマンドを送ります。 
    
3. VSS は、スナップショット ・ バックアップ用に準備する Exchange 書き込みプログラムと通信します。 Exchange 2013 は、データベースに対する管理操作は禁止されています、ボリュームの依存関係をチェックし、読み取り専用アクセスを可能にしながら、データベースとトランザクション ログ ファイルの選択したインスタンスへのすべての書き込み操作を中断します。 
    
4. VSS は、Exchange 2013 のデータベースを含むストレージ ボリュームのシャドウ コピーを作成するのには適切なストレージ プロバイダーと通信します。 
    
5. VSS では、通常の処理を再開するのには、Exchange 2013 を解放します。 
    
6. VSS リクエスターは、バックアップが正常に完了したことを通知する前に設定のバックアップの物理的な整合性を検証します。 Exchange 2013 は、トランザクション ・ ログをトランケート (データベースが DAG の一部である場合は、ログの切り捨てはレプリケートされたすべてのコピーの間で) し、データベースの最後のバックアップの時間を記録します。
    
VSS は、 [OnPostSnapshot](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381568%28v=vs.85%29.aspx)メソッドで[OnPrepareBackup](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381571%28v=vs.85%29.aspx)メソッドを使用して開始および終了は、Exchange ライターに依頼者の操作をシリアル化します。 通常、シャドウ コピーの整合性がバックアップの完了前に確認すると Exchange writer がシャドウ コピーでの作業に費やす時間の大半に、 **OnPostSnapshot**メソッドでは後に、発生します。 Exchange 書き込みプログラムは、 **OnPostSnapshot**と[OnBackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381557%28v=vs.85%29.aspx)の並列バックアップをサポートしています。
  
Exchange 2013 では、同じデータベースのバックアップを同時実行が許可されていません。 バックアップ ジョブを 1 つだけが一度に 1 つの特定のデータベースに対して実行できます。 バックアップの実行中、Exchange ストアは、バックアップの進行中の状態にデータベースを配置します。 いずれかのバックアップ ・ プロセス、またはサービスを再起動すると完了した時点で、このメモリの状態がクリアされます。 オペレーティング システムを再起動すると、Exchange ライターをホストするサービスを再起動するとき、またはクラスターのフェイル オーバーが発生した場合、メモリ内の進行中のバックアップの状態とその関連データは失われます。 バックアップ ジョブが失敗するが、これらのイベントが発生します。
  
実行するバックアップの種類に基づいて、バックアップ開始トランザクション ログ ファイルの切り詰めがトリガーされます。DAG 以外の構成では、Exchange ライターは、完全バックアップや増分バックアップが正常に完了したときにトランザクション ログ ファイルを切り詰めます。DAG のレプリケートされた構成では、すべての必要なログ ファイルが他のすべてのコピーに再生されるまで、レプリケーション サービスによってログの切り詰めが遅延されます。レプリケーション サービスは、アクティブなログ ファイル パスとコピー ログ ファイル パスの両方からバックアップ ログ ファイルを削除します。この削除は、ログ ファイルがコピー データベースに正常に適用され、アクティブ データベースとデータベース コピー チェックポイントの両方が削除対象のログ ファイルを渡したことを確認した後に行われます。
  
## <a name="see-also"></a>関連項目

- [トランザクション ログとチェックポイント ファイルをバックアップおよび復元では、Exchange 2013 の](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

