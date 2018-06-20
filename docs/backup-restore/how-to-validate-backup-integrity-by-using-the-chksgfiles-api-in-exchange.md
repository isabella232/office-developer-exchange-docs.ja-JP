---
title: Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: CHKSGFILES API を使用して Exchange 2013 の Exchange ストアのバックアップを検証する方法を確認します。
ms.openlocfilehash: 968484cd5bb7439730685643683e1d850bec33ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758865"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。

CHKSGFILES API を使用して Exchange 2013 の Exchange ストアのバックアップを検証する方法を確認します。
  
**に適用されます:** Exchange Server 2013 
  
によって、ボリューム シャドウ コピー サービス (VSS) の管理、バックアップの処理中に Exchange Server 2013 は各データベース ファイル全体を読み取るし、チェックサムの整合性を確認できません。 したがって、データベースとトランザクション ログ ファイルの整合性を確認するのには、バックアップ ・ アプリケーションが必要な可能性があります。 バックアップ アプリケーションが Exchange ライターに、バックアップが完了していることを通知する前にシャドウ コピー セットの物理的な整合性を確認することをお勧めします。 バックアップの成功後は、Exchange ストアは、最後のバックアップからロール フォワードする必要はなくなりますが、最後のバックアップの時間し、サーバーからのトランザクション ログの削除を反映するようにバックアップ データベースのヘッダーを更新します。
  
## <a name="prerequisites-for-validating-backup-integrity"></a>バックアップ整合性を検証するための前提条件

独自のアプリケーションでバックアップの整合性を検証するには、次に示す項目にアクセスできる必要があります。
  
- Exchange ストアのバックアップのファイル。
- Visual Studio 2010 以降のいずれかの Visual Studio のバージョン。
- CHKSGFILES のライブラリとヘッダー ファイルです。 ライブラリとヘッダー ファイルは、 [Microsoft ダウンロード センター](http://www.microsoft.com/en-us/download/details.aspx?id=36802)からダウンロードできます。
    
## <a name="validate-backup-integrity"></a>バックアップの整合性の検証

次の手順では、独自のバックアップおよび復元アプリケーションで、データ整合性を検証する方法について説明しています。
  
### <a name="to-validate-backup-integrity"></a>バックアップの整合性を検証するには

1. **CChkSGFiles**クラスの新しいインスタンスを作成します。 
   
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

   最初の行のコードはエラー オブジェクトを作成に成功した場合、その初期値を設定し、データベースの妥当性を検査するオブジェクトを作成します。 次に、 [CChkSGFiles.New 関数](cchksgfiles-new-function.md)は、 **CChkSGFiles**クラスの新しいインスタンスを作成します。 新しいオブジェクトの簡単なチェックでは、新しいインスタンスが作成されたときに、問題が発生したかを示します。 
    
2. **CChkSGFiles**オブジェクトを初期化します。 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   パラメーターの詳細については、 [CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)を参照してください。
   
3. データベース ヘッダーを確認することでデータベースの整合性を検証するのにには、 [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を使用します。
   
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
   
   パラメーターの詳細については、 [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を参照してください。
   
4. エラーを処理し、 **CChkSGFiles**クラスをメモリから削除するのには、 [CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)を使用します。 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>関連項目

- [CChkSGFiles クラスの参照](cchksgfiles-class-reference.md)
- [バックアップを作成し、Exchange 2013 のアプリケーションを復元します。](build-backup-and-restore-applications-for-exchange-2013.md)
- [Exchange 2013 のバックアップと復元の概念](backup-and-restore-concepts-for-exchange-2013.md)
    

