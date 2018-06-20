---
title: Exchange 2013 のバックアップと復元の概念
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Exchange データベースのバックアップを作成し、Exchange 2013 のアプリケーションを復元するための情報を検索します。
ms.openlocfilehash: 5fa62c3d34ffbe8f0bab852c6d41c49220e2883a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758867"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Exchange 2013 のバックアップと復元の概念

Exchange データベースのバックアップを作成し、Exchange 2013 のアプリケーションを復元するための情報を検索します。
  
バックアップを作成して Exchange Server 2013 のアプリケーションを復元して、前に、Exchange データベース ファイルの構造を理解する必要があります。 Exchange ストアのデータベース ファイルを使用すると、ストアにデータをバックアップしは後で必要に応じて復元できます。 場合に、ディスク領域の制限は、循環ログは、実装、管理者、データベースのバックアップを作成する能力に影響を与えるこれは バックアップし、Exchange データを復元する Exchange 2013 のデータベースの移動機能を実行できます。 バックアップと復元のアプリケーションとの組み合わせで、データベースの移動は、災害復旧のための冗長性の優れた手段です。

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Exchange ストアのデータベース ファイル

Exchange 2013 には、最大 100 個のデータベースのサポートが含まれています。 各 Exchange 2013 のデータベースには、次の表に記載されているファイルが含まれています。 
  
**表 1 です。データベース ファイルを Exchange 2013**

|ファイルの種類|拡張子|説明|
|:-----|:-----|:-----|
|データベース ファイル  <br/> |\*.edb ファイル  <br/> |メモリ内のデータベースにコミットされたすべての変更を記録します。  <br/> |
|トランザクション ログ ストリーム  <br/> |\*.log  <br/> |データベースにコミットされる、メッセージの変更または作成などのレコードの操作。それぞれ 1 MB のサイズに制限されます。  <br/> |
|チェックポイント ファイル  <br/> |\*.chk  <br/> |トランザクションがログに記録されるレコードは、ディスク上のデータベース ファイルに記載されています。  <br/> |
   
Exchange 2013 では、各データベースのトランザクション ログ ファイルの 1 つのセットを保持します。 トランザクション ・ ログは、バックアップ/リカバリ ・ オペレーションの重要です。 バックアップを作成するボリューム シャドウ コピー サービス (VSS) を使用するアプリケーションを復元すると、これらのログを正しく処理することを確認する必要があります。 詳細については、[トランザクション ログとチェックポイント ・ ファイルのバックアップと復元では、Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)を参照してください。 データベースとそのログ ストリームをバックアップするためには、データベースとログを含むボリューム全体をバックアップする必要があります。 ログのトランケートまたは Exchange データベースを格納するフォルダーのフル ・ バックアップが正常に完了した後にのみ発生します。
  
各 Exchange サーバーで、同時に 1 つだけの回復用データベースをマウントできます。 **新しい MailboxRestoreRequest**などの Exchange 管理シェル コマンドレットを使用して回復データベースにアクセスすることができます。 Exchange 回復用データベースの詳細については、TechNet の「[回復用データベース](http://technet.microsoft.com/en-us/library/dd876954%28v=exchg.150%29.aspx)を参照してください。 Exchange 管理シェル コマンドレットの詳細については、TechNet の[Exchange 2013 のコマンドレット](http://technet.microsoft.com/en-us/library/bb124413.aspx)を参照してください。 
  
## <a name="circular-logging"></a>循環ログ
<a name="bk_circularlogging"> </a>

ストレージ容量に問題がある場合、管理者は、循環ログを有効可能性があります。 循環ログを有効にすると、Exchange は通常どおりには、トランザクション ・ ログに書き込みますが、チェックポイント ファイルを拡張すると、トランザクション ログのアクティブでない部分が切り捨てられます。 管理者は、VSS を使用して、ユーザー設定のバックアップを有効にして、復元の操作も行う場合は、循環ログを使用して Exchange 2013 のデータベースを構成しないでください。 循環ログは、次の制限を作成します。 
  
- バックアップ操作または回復操作中に循環ログが有効な場合、個々のデータベースを復元することはできません。
    
- ポイント ・ イン ・ タイムのリカバリ ・ オペレーションだけでは、可能です。 循環ログを有効にすると、削除できます同じディレクトリにトランザクション ・ ログ、データベースが復元されると、それらのログは別の Exchange 2013 データベースの一部である可能性があります。 
    
- 増分または差分のバックアップ ・ オペレーションを実行することはできません。 これらの種類のバックアップの詳細については、 [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)を参照してください。
    
循環ログが有効の場合は、管理者に無効に、VSS バックアップが失敗しないことを確認するには、できるだけ早くします。 詳細については、 [Exchange の循環ログ出力と VSS バックアップ](http://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx)は、ブログ記事をご覧ください。 
  
## <a name="exchange-database-mobility"></a>Exchange データベース モビリティ
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 メールボックスの信頼性と可用性を向上させるデータベースを移動をできます。 データベース モビリティでは、Exchange ストア データベースのコピーを作成して、サーバーからデータベースを切断して別のサーバーに保存することができます。 Exchange 2013 データベース可用性グループ (DAG)、データベースの複数のコピーは、別のコンピューターに格納されます。 ハードウェアまたはその他のシステム障害が発生したため、データベースの 1 つまたは複数のコピーがなくなったときは、通常のレプリケーション操作でデータベースを再シードするのには他のコピーからの情報を使用できます。
  
バックアップ ・ オペレーションの Exchange 2013 のデータベースをバックアップするのには、DAG で構成されている場合バックアップ ・ アプリケーション防ぐことができますよりスナップショットと、アクティブなサーバーのパフォーマンスとの間の干渉によって、スナップショットを非アクティブのいずれかのデータベースをコピーします。 データベースのコピーは同期の大部分は、バックアップ ・ アプリケーションは、データベースの別のコピーからスナップショットを取得し、後でその部分から再構築できます。
  
DAG のデータベースをバックアップ データから復元するための、唯一サポートされている方法は、同じバックアップ データを使用してデータベースのすべてのコピーを復元することです。データベースのログ ファイルはコピーの間でわずかに異なる可能性があるため、別のデータを使用して個々のデータベースのコピーを復元すると、データベースがマウントできなくなる場合があります。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [トランザクション ログとチェックポイント ファイルをバックアップおよび復元では、Exchange 2013 の](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 で Exchange ライター](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [オンラインの Exchange および Exchange の開発](../exchange-server-development.md) 
- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
- [2013 の Exchange データベースを復元します。](restoring-exchange-2013-databases.md)
    

