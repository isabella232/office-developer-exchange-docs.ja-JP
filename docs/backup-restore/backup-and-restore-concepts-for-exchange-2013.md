---
title: Exchange 2013 のバックアップと復元の概念
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: 2013 年Exchangeバックアップおよび復元アプリケーションの作成に役立つデータベースの詳細Exchangeします。
ms.openlocfilehash: c0b2e0269c3668779f980bf6984d84aff76573f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510520"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Exchange 2013 のバックアップと復元の概念

2013 年Exchangeバックアップおよび復元アプリケーションの作成に役立つデータベースの詳細Exchangeします。
  
2013 年 2013 年のバックアップおよび復元アプリケーションをExchange Server、データベース ファイルの構造をExchangeする必要があります。 データベース ファイルExchange使用すると、ストア内のデータをバックアップし、必要に応じて後で復元できます。 ディスク領域が制限されている場合、管理者は循環ログを実装する可能性があり、データベースをバックアップする機能に影響します。 また、2013 年 2013 年のデータベース モビリティ機能を利用して、Exchangeデータをバックアップおよび復元Exchangeできます。 データベース モビリティは、バックアップおよび復元アプリケーションと組み合わせて、障害復旧のための冗長性の優れた手段です。

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Exchange ストアのデータベース ファイル

Exchange 2013 には、最大 100 のデータベースのサポートが含まれています。 各Exchange 2013 データベースには、次の表に示すファイルが含まれます。 
  
**表 1.Exchange 2013 データベース ファイル**

|ファイルの種類|拡張子|説明|
|:-----|:-----|:-----|
|データベース ファイル  <br/> |\*.edb  <br/> |メモリ内のデータベースにコミットされたすべての変更を記録します。  <br/> |
|トランザクション ログ ストリーム  <br/> |\*.log  <br/> |データベースにコミットされる、メッセージの変更または作成などのレコードの操作。それぞれ 1 MB のサイズに制限されます。  <br/> |
|チェックポイント ファイル  <br/> |\*.chk  <br/> |トランザクションがログに記録されるレコードは、ディスク上のデータベース ファイルに記載されています。  <br/> |
   
Exchange 2013 では、データベースごとに 1 セットのトランザクション ログ ファイルが保持されます。 トランザクション ログは、バックアップ操作と回復操作において重要になります。 バックアップを作成するボリューム シャドウ コピー サービス (VSS) を使用するアプリケーションを復元する場合は、これらのログを正しく処理していることを確認する必要があります。 詳細については、「[Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)」を参照してください。 データベースと、データベースのログ ストリームをバックアップするには、そのデータベースとログが含まれているボリューム全体をバックアップする必要があります。 ログの切り捨ては、Exchange データベースを含むボリュームまたはフォルダーの完全バックアップが正常に完了した後にのみ行われます。
  
各 Exchange サーバーで同時にマウントできる回復用データベースは 1 つのみです。 回復用データベースには、**New-MailboxRestoreRequest** などの Exchange 管理シェル コマンドレットを使用してアクセスできます。 回復データベースの詳細についてはExchange TechNet[の「回復データベース」](https://technet.microsoft.com/library/dd876954%28v=exchg.150%29.aspx)を参照してください。 管理シェルコマンドレットのExchange詳細については[、「techNet Exchange 2013 コマンドレット」を](https://technet.microsoft.com/library/bb124413.aspx)参照してください。 
  
## <a name="circular-logging"></a>循環ログ
<a name="bk_circularlogging"> </a>

ストレージ容量に問題がある場合は、管理者が循環ログを有効にする可能性があります。 循環ログを有効にすると、Exchange は通常どおりにトランザクション ログを書き込みますが、チェックポイント ファイルを拡張すると、トランザクション ログのアクティブでない部分が切り捨てられます。 VSS を Exchange使用してカスタムのバックアップと復元操作を有効にする場合は、管理者は 2013 データベースで循環ログを使用する構成を行う必要があります。 循環ログには、次の制限があります。 
  
- バックアップ操作または回復操作中に循環ログが有効な場合、個々のデータベースを復元することはできません。
    
- ポイントインタイム回復操作のみ可能です。 循環ログを有効にすると、データベースが復元される際に同じディレクトリ内のトランザクション ログを削除できます。ただし、これらのログは 2013 年の別のデータベースの一部Exchangeできます。 
    
- 増分または差分のバックアップ操作は実行できません。 これらの種類のバックアップの詳細については[、「2013](types-of-backup-operations-for-exchange-2013.md)年のバックアップ操作の種類Exchange参照してください。
    
循環ログが有効な場合、管理者は VSS バックアップが失敗しなかねずにできるだけ早く無効にする必要があります。 詳細については、「循環ログと VSS バックアップ」[のブログExchangeを参照してください](https://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx)。 
  
## <a name="exchange-database-mobility"></a>Exchange データベース モビリティ
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 では、データベース モビリティによってメールボックスの信頼性と可用性が向上します。 データベース モビリティにより、Exchange ストア データベースのコピーを作成し、サーバーからデータベースを切断して別のサーバーにコピーを保存できます。 2013 Exchange可用性グループ (DAG) では、データベースの複数のコピーが異なるコンピューターに保存されます。 ハードウェアまたはその他のシステム障害が発生したために、データベースの 1 つまたは複数のコピーが失われた場合は、他のコピーからの情報を使用して、通常のレプリケーション操作でデータベースを再シードできます。
  
バックアップ操作の場合、バックアップする Exchange 2013 データベースが DAG で構成されている場合、バックアップ アプリケーションは、非アクティブなデータベース コピーの 1 つでスナップショットを取得することで、スナップショットとアクティブ サーバーのパフォーマンスの間の干渉を防止できます。 データベースのコピーは同期の大部分にあたるため、バックアップ アプリケーションはデータベースの別のコピーからスナップショットを取得して、後にその部分から再構築することができます。
  
DAG のデータベースをバックアップ データから復元するための、唯一サポートされている方法は、同じバックアップ データを使用してデータベースのすべてのコピーを復元することです。データベースのログ ファイルはコピーの間でわずかに異なる可能性があるため、別のデータを使用して個々のデータベースのコピーを復元すると、データベースがマウントできなくなる場合があります。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange 2013 のバックアップと復元のトランザクション ログとチェックポイント ファイル](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange 2013 の Exchange ライター](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>関連項目

- [Exchange Online と Exchange の開発](../exchange-server-development.md) 
- [Exchange 2013 のバックアップ操作の種類](types-of-backup-operations-for-exchange-2013.md)
- [Exchange 2013 のデータベースを復元する](restoring-exchange-2013-databases.md)
    

