---
title: Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: CHKSGFILES API を使用して exchange 2013 の Exchange ストアのバックアップを検証する方法について説明します。
ms.openlocfilehash: c101413793cf3b952d3db3e0f792c8bcf2dd9fc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452861"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証する

CHKSGFILES API を使用して exchange 2013 の Exchange ストアのバックアップを検証する方法について説明します。
  
**製品:** Exchange Server 2013 
  
ボリュームシャドウコピーサービス (VSS) によって管理されるバックアップ操作では、Exchange Server 2013 は各データベースファイル全体を読み取り、そのチェックサムの整合性を確認することはできません。 そのため、データベースとトランザクション ログ ファイルの整合性を検証する独自のバックアップ アプリケーションが必要になることがあります。 独自のバックアップ アプリケーションでは、Exchange ライターにバックアップの完了を通知する前に、シャドウ コピー セットの物理的な整合性を確認するようにしてください。 バックアップが正常に完了すると、Exchange ストアは、最後に成功したバックアップの時刻を反映するようにバックアップしたデータベースのヘッダーを更新して、最後に成功したバックアップからロールフォワードする必要のなくなったトランザクション ログをサーバーから削除します。
  
## <a name="prerequisites-for-validating-backup-integrity"></a>バックアップ整合性を検証するための前提条件

独自のアプリケーションでバックアップの整合性を検証するには、次に示す項目にアクセスできる必要があります。
  
- Exchange ストアのバックアップのファイル。
- Visual Studio 2010 以降のいずれかの Visual Studio のバージョン。
- CHKSGFILES ライブラリ ファイルとヘッダー ファイル。 ライブラリとヘッダーファイルは、 [Microsoft ダウンロードセンター](https://www.microsoft.com/download/details.aspx?id=36802)からダウンロードできます。
    
## <a name="validate-backup-integrity"></a>バックアップの整合性の検証

次の手順では、独自のバックアップおよび復元アプリケーションで、データ整合性を検証する方法について説明しています。
  
### <a name="to-validate-backup-integrity"></a>バックアップの整合性を検証するには

1. **CChkSGFiles** クラスの新しいインスタンスを作成します。 
   
   ```cpp
   CCheckSGFiles::ERRerr = CCheckSGFiles::errSuccess;
   ULONGiDbError = (ULONG)CCheckSGFiles::iDbInvalid;
   CCheckSGFiles * const pcchecksgfiles = CCheckSGFiles::New();
   if ( NULL == pcchecksgfiles )
   {
     err = CCheckSGFiles::errOutOfMemory;
     printf( "ERROR: Could not allocate CCheckSGFiles object.\n" );
     goto HandleError;
   }
   ```

   コードの最初の行では、error オブジェクトを作成し、その初期値を success に設定し、データベースの有効性をチェックするオブジェクトを作成します。 その後、 [CChkSGFiles 関数](cchksgfiles-new-function.md)は**CChkSGFiles**クラスの新しいインスタンスを作成します。 新しいオブジェクトのクイックチェックは、新しいインスタンスが作成されたときに問題が発生したかどうかを示します。 
    
2. **CChkSGFiles** オブジェクトを初期化します。 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   パラメーターの詳細については、「[CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)」を参照してください。
   
3. [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を使用して、データベースのヘッダーを確認することで、データベース整合性を検証します。
   
   ```cpp
   err = pcchecksgfiles->ErrCheckDbHeaders(
   &amp;cbDbPageSize,
   &amp;cDbHeaderPages,
   &amp;iDbError );
   if ( CCheckSGFiles::errSuccess != err )
   {
   if ( CCheckSGFiles::iDbInvalid != iDbError )
   {
   printf(
   "ERROR: Database header validation for '%S' failed with error %d (0x%x)\n",
   rgwszDb[ iDbError ],
   err,
   err );
   }
   goto HandleError;
   }
   ```
   
   パラメーターの詳細については、「[CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)」を参照してください。
   
4. エラーを処理し、[CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)を使用してメモリから **CChkSGFiles** クラスを削除します。 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>関連項目

- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
- [Exchange 2013 のバックアップと復元アプリケーションの作成](build-backup-and-restore-applications-for-exchange-2013.md)
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

