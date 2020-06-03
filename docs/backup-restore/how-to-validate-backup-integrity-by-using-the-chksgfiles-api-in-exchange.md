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
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="74d4c-103">Exchange 2013 で CHKSGFILES API を使用してバックアップの整合性を検証する</span><span class="sxs-lookup"><span data-stu-id="74d4c-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="74d4c-104">CHKSGFILES API を使用して exchange 2013 の Exchange ストアのバックアップを検証する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="74d4c-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="74d4c-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="74d4c-106">ボリュームシャドウコピーサービス (VSS) によって管理されるバックアップ操作では、Exchange Server 2013 は各データベースファイル全体を読み取り、そのチェックサムの整合性を確認することはできません。</span><span class="sxs-lookup"><span data-stu-id="74d4c-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="74d4c-107">そのため、データベースとトランザクション ログ ファイルの整合性を検証する独自のバックアップ アプリケーションが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="74d4c-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="74d4c-108">独自のバックアップ アプリケーションでは、Exchange ライターにバックアップの完了を通知する前に、シャドウ コピー セットの物理的な整合性を確認するようにしてください。</span><span class="sxs-lookup"><span data-stu-id="74d4c-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="74d4c-109">バックアップが正常に完了すると、Exchange ストアは、最後に成功したバックアップの時刻を反映するようにバックアップしたデータベースのヘッダーを更新して、最後に成功したバックアップからロールフォワードする必要のなくなったトランザクション ログをサーバーから削除します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="74d4c-110">バックアップ整合性を検証するための前提条件</span><span class="sxs-lookup"><span data-stu-id="74d4c-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="74d4c-111">独自のアプリケーションでバックアップの整合性を検証するには、次に示す項目にアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="74d4c-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="74d4c-112">Exchange ストアのバックアップのファイル。</span><span class="sxs-lookup"><span data-stu-id="74d4c-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="74d4c-113">Visual Studio 2010 以降のいずれかの Visual Studio のバージョン。</span><span class="sxs-lookup"><span data-stu-id="74d4c-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="74d4c-114">CHKSGFILES ライブラリ ファイルとヘッダー ファイル。</span><span class="sxs-lookup"><span data-stu-id="74d4c-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="74d4c-115">ライブラリとヘッダーファイルは、 [Microsoft ダウンロードセンター](https://www.microsoft.com/download/details.aspx?id=36802)からダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="74d4c-115">You can download the library and header files from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="74d4c-116">バックアップの整合性の検証</span><span class="sxs-lookup"><span data-stu-id="74d4c-116">Validate backup integrity</span></span>

<span data-ttu-id="74d4c-117">次の手順では、独自のバックアップおよび復元アプリケーションで、データ整合性を検証する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="74d4c-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="74d4c-118">バックアップの整合性を検証するには</span><span class="sxs-lookup"><span data-stu-id="74d4c-118">To validate backup integrity</span></span>

1. <span data-ttu-id="74d4c-119">**CChkSGFiles** クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
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

   <span data-ttu-id="74d4c-120">コードの最初の行では、error オブジェクトを作成し、その初期値を success に設定し、データベースの有効性をチェックするオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="74d4c-121">その後、 [CChkSGFiles 関数](cchksgfiles-new-function.md)は**CChkSGFiles**クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="74d4c-122">新しいオブジェクトのクイックチェックは、新しいインスタンスが作成されたときに問題が発生したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="74d4c-123">**CChkSGFiles** オブジェクトを初期化します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="74d4c-124">パラメーターの詳細については、「[CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74d4c-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="74d4c-125">[CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を使用して、データベースのヘッダーを確認することで、データベース整合性を検証します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
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
   
   <span data-ttu-id="74d4c-126">パラメーターの詳細については、「[CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74d4c-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="74d4c-127">エラーを処理し、[CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)を使用してメモリから **CChkSGFiles** クラスを削除します。</span><span class="sxs-lookup"><span data-stu-id="74d4c-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="74d4c-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="74d4c-128">See also</span></span>

- [<span data-ttu-id="74d4c-129">CChkSGFiles クラスの参照</span><span class="sxs-lookup"><span data-stu-id="74d4c-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="74d4c-130">Exchange 2013 のバックアップと復元アプリケーションの作成</span><span class="sxs-lookup"><span data-stu-id="74d4c-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="74d4c-131">Exchange 2013 のバックアップと復元の概念</span><span class="sxs-lookup"><span data-stu-id="74d4c-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

