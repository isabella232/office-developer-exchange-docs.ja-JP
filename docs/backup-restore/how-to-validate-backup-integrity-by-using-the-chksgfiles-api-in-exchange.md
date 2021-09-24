---
title: 2013 年に CHKSGFILES API を使用してバックアップExchangeする
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: CHKSGFILES API を使用して、2013 年 3 月に Exchange ストアのExchangeします。
ms.openlocfilehash: 7a12a0a8f66128970a782da50ba59f41767c60d3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516231"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>2013 年に CHKSGFILES API を使用してバックアップExchangeする

CHKSGFILES API を使用して、2013 年 3 月に Exchange ストアのExchangeします。
  
**製品:** Exchange Server 2013 
  
ボリューム シャドウ コピー サービス (VSS) によって管理されるバックアップ操作中に、Exchange Server 2013 は各データベース ファイル全体を読み取り、チェックサムの整合性を確認できません。 そのため、データベースとトランザクション ログ ファイルの整合性を検証する独自のバックアップ アプリケーションが必要になることがあります。 独自のバックアップ アプリケーションでは、Exchange ライターにバックアップの完了を通知する前に、シャドウ コピー セットの物理的な整合性を確認するようにしてください。 バックアップが正常に完了すると、Exchange ストアは、最後に成功したバックアップの時刻を反映するようにバックアップしたデータベースのヘッダーを更新して、最後に成功したバックアップからロールフォワードする必要のなくなったトランザクション ログをサーバーから削除します。
  
## <a name="prerequisites-for-validating-backup-integrity"></a>バックアップ整合性を検証するための前提条件

独自のアプリケーションでバックアップの整合性を検証するには、次に示す項目にアクセスできる必要があります。
  
- Exchange ストアのバックアップのファイル。
- Visual Studio 2010 以降のいずれかの Visual Studio のバージョン。
- CHKSGFILES ライブラリ ファイルとヘッダー ファイル。 ライブラリとヘッダー ファイルは、Microsoft ダウンロード センター [からダウンロードできます](https://www.microsoft.com/download/details.aspx?id=36802)。
    
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

   コードの冒頭の行では、エラー オブジェクトを作成して、そのオブジェクトの初期値を成功に設定します。また、データベースの妥当性を確認するオブジェクトも作成します。その後で、[CChkSGFiles.New 関数](cchksgfiles-new-function.md)によって、**CChkSGFiles** クラスの新しいインスタンスを作成します。新しいオブジェクトの簡易チェックにより、新しいインスタンスの作成時に問題が発生したかどうかがわかります。 
    
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
    

