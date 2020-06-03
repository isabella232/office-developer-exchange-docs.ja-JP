---
title: Exchange 2013 のバックアップと復元の概念
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Exchange 2013 のバックアップと復元アプリケーションの作成に役立つ Exchange データベースについての情報を参照してください。
ms.openlocfilehash: fd35699839af105dd3fe285776b071c1d03d58dd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44437985"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Exchange 2013 のバックアップと復元の概念

Exchange 2013 のバックアップと復元アプリケーションの作成に役立つ Exchange データベースについての情報を参照してください。
  
Exchange Server 2013 のバックアップと復元アプリケーションを作成する前に、Exchange データベースファイル構造について理解しておく必要があります。 Exchange ストアデータベースファイルを使用すると、ストア内のデータをバックアップし、必要に応じて後で復元することができます。 ディスク容量に制限がある場合は、管理者が循環ログを実装している可能性があります。これにより、データベースをバックアップすることができます。 Exchange 2013 のデータベースモビリティ機能を利用して、Exchange データのバックアップと復元を行うこともできます。 データベースモビリティは、バックアップと復元のアプリケーションと組み合わせて、障害復旧のための冗長な手段となります。

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Exchange ストアのデータベース ファイル

Exchange 2013 には、最大100データベースのサポートが含まれています。 各 Exchange 2013 データベースには、次の表に示すファイルが含まれています。 
  
**表1Exchange 2013 データベースファイル**

|ファイルの種類|拡張子|Description|
|:-----|:-----|:-----|
|データベース ファイル  <br/> |\*.edb  <br/> |メモリ内のデータベースにコミットされたすべての変更を記録します。  <br/> |
|トランザクション ログ ストリーム  <br/> |\*.log  <br/> |データベースにコミットされる、メッセージの変更または作成などのレコードの操作。それぞれ 1 MB のサイズに制限されます。  <br/> |
|チェックポイント ファイル  <br/> |\*.chk  <br/> |トランザクションがログに記録されるレコードは、ディスク上のデータベース ファイルに記載されています。  <br/> |
   
Exchange 2013 は、データベースごとに1つのトランザクションログファイルセットを保持します。 トランザクション ログは、バックアップ操作と回復操作において重要になります。 バックアップを作成するボリューム シャドウ コピー サービス (VSS) を使用するアプリケーションを復元する場合は、これらのログを正しく処理していることを確認する必要があります。 詳細については、「[Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)」を参照してください。 データベースと、データベースのログ ストリームをバックアップするには、そのデータベースとログが含まれているボリューム全体をバックアップする必要があります。 ログの切り捨ては、Exchange データベースを含むボリュームまたはフォルダーの完全バックアップが正常に完了した後にのみ行われます。
  
各 Exchange サーバーで同時にマウントできる回復用データベースは 1 つのみです。 回復用データベースには、**New-MailboxRestoreRequest** などの Exchange 管理シェル コマンドレットを使用してアクセスできます。 Exchange 回復データベースの詳細については、TechNet の「[回復用データベース](https://technet.microsoft.com/library/dd876954%28v=exchg.150%29.aspx)」を参照してください。 Exchange 管理シェルコマンドレットの詳細については、TechNet の「 [exchange 2013 コマンドレット](https://technet.microsoft.com/library/bb124413.aspx)」を参照してください。 
  
## <a name="circular-logging"></a>循環ログ
<a name="bk_circularlogging"> </a>

ストレージ容量に問題がある場合は、管理者が循環ログを有効にする可能性があります。 循環ログを有効にすると、Exchange は通常どおりにトランザクション ログを書き込みますが、チェックポイント ファイルを拡張すると、トランザクション ログのアクティブでない部分が切り捨てられます。 VSS を使用してカスタムのバックアップおよび復元操作を有効にする場合は、管理者は、循環ログを使用するように Exchange 2013 データベースを構成しないようにしてください。 循環ログには、次の制限があります。 
  
- バックアップ操作または回復操作中に循環ログが有効な場合、個々のデータベースを復元することはできません。
    
- ポイントインタイムの回復操作のみが可能です。 循環ログが有効になっている場合は、データベースを復元するときに、同じディレクトリのトランザクションログを削除できます。ただし、これらのログは別の Exchange 2013 データベースの一部である場合もあります。 
    
- 増分または差分のバックアップ操作は実行できません。 これらのバックアップの種類の詳細については、「 [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)」を参照してください。
    
循環ログが有効になっている場合、管理者はこれをできるだけ早く無効にして、VSS のバックアップが失敗しないようにする必要があります。 詳細については、ブログの「 [Exchange の循環ログおよび VSS バックアップ](https://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx)の投稿」を参照してください。 
  
## <a name="exchange-database-mobility"></a>Exchange データベース モビリティ
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 では、データベースのモビリティを使用して、メールボックスの信頼性と可用性を向上させることができます。 データベース モビリティにより、Exchange ストア データベースのコピーを作成し、サーバーからデータベースを切断して別のサーバーにコピーを保存できます。 Exchange 2013 データベース可用性グループ (DAG) では、データベースの複数のコピーが異なるコンピューターに格納されます。 ハードウェアまたはその他のシステム障害が発生したために、データベースの 1 つまたは複数のコピーが失われた場合は、他のコピーからの情報を使用して、通常のレプリケーション操作でデータベースを再シードできます。
  
バックアップ操作で、バックアップする Exchange 2013 データベースが DAG 内で構成されている場合、バックアップアプリケーションは、非アクティブなデータベースコピーのいずれかのスナップショットを使用することにより、スナップショットとアクティブなサーバーのパフォーマンスとの間の干渉を防ぐことができます。 データベースのコピーは同期の大部分にあたるため、バックアップ アプリケーションはデータベースの別のコピーからスナップショットを取得して、後にその部分から再構築することができます。
  
DAG のデータベースをバックアップ データから復元するための、唯一サポートされている方法は、同じバックアップ データを使用してデータベースのすべてのコピーを復元することです。データベースのログ ファイルはコピーの間でわずかに異なる可能性があるため、別のデータを使用して個々のデータベースのコピーを復元すると、データベースがマウントできなくなる場合があります。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 の Exchange ライター](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange Online と Exchange の開発](../exchange-server-development.md) 
- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
- [Exchange 2013 のデータベースを復元する](restoring-exchange-2013-databases.md)
    

