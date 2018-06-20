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
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="5ac74-103">Exchange 2013 の CHKSGFILES API を使用してバックアップの整合性を検証します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="5ac74-104">CHKSGFILES API を使用して Exchange 2013 の Exchange ストアのバックアップを検証する方法を確認します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="5ac74-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5ac74-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="5ac74-106">によって、ボリューム シャドウ コピー サービス (VSS) の管理、バックアップの処理中に Exchange Server 2013 は各データベース ファイル全体を読み取るし、チェックサムの整合性を確認できません。</span><span class="sxs-lookup"><span data-stu-id="5ac74-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="5ac74-107">したがって、データベースとトランザクション ログ ファイルの整合性を確認するのには、バックアップ ・ アプリケーションが必要な可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5ac74-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="5ac74-108">バックアップ アプリケーションが Exchange ライターに、バックアップが完了していることを通知する前にシャドウ コピー セットの物理的な整合性を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5ac74-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="5ac74-109">バックアップの成功後は、Exchange ストアは、最後のバックアップからロール フォワードする必要はなくなりますが、最後のバックアップの時間し、サーバーからのトランザクション ログの削除を反映するようにバックアップ データベースのヘッダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="5ac74-110">バックアップ整合性を検証するための前提条件</span><span class="sxs-lookup"><span data-stu-id="5ac74-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="5ac74-111">独自のアプリケーションでバックアップの整合性を検証するには、次に示す項目にアクセスできる必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ac74-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="5ac74-112">Exchange ストアのバックアップのファイル。</span><span class="sxs-lookup"><span data-stu-id="5ac74-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="5ac74-113">Visual Studio 2010 以降のいずれかの Visual Studio のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5ac74-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="5ac74-114">CHKSGFILES のライブラリとヘッダー ファイルです。</span><span class="sxs-lookup"><span data-stu-id="5ac74-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="5ac74-115">ライブラリとヘッダー ファイルは、 [Microsoft ダウンロード センター](http://www.microsoft.com/en-us/download/details.aspx?id=36802)からダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="5ac74-115">You can download the library and header files from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="5ac74-116">バックアップの整合性の検証</span><span class="sxs-lookup"><span data-stu-id="5ac74-116">Validate backup integrity</span></span>

<span data-ttu-id="5ac74-117">次の手順では、独自のバックアップおよび復元アプリケーションで、データ整合性を検証する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="5ac74-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="5ac74-118">バックアップの整合性を検証するには</span><span class="sxs-lookup"><span data-stu-id="5ac74-118">To validate backup integrity</span></span>

1. <span data-ttu-id="5ac74-119">**CChkSGFiles**クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
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

   <span data-ttu-id="5ac74-120">最初の行のコードはエラー オブジェクトを作成に成功した場合、その初期値を設定し、データベースの妥当性を検査するオブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="5ac74-121">次に、 [CChkSGFiles.New 関数](cchksgfiles-new-function.md)は、 **CChkSGFiles**クラスの新しいインスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="5ac74-122">新しいオブジェクトの簡単なチェックでは、新しいインスタンスが作成されたときに、問題が発生したかを示します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="5ac74-123">**CChkSGFiles**オブジェクトを初期化します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="5ac74-124">パラメーターの詳細については、 [CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac74-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="5ac74-125">データベース ヘッダーを確認することでデータベースの整合性を検証するのにには、 [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
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
   
   <span data-ttu-id="5ac74-126">パラメーターの詳細については、 [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ac74-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="5ac74-127">エラーを処理し、 **CChkSGFiles**クラスをメモリから削除するのには、 [CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="5ac74-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ac74-128">See also</span></span>

- [<span data-ttu-id="5ac74-129">CChkSGFiles クラスの参照</span><span class="sxs-lookup"><span data-stu-id="5ac74-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="5ac74-130">バックアップを作成し、Exchange 2013 のアプリケーションを復元します。</span><span class="sxs-lookup"><span data-stu-id="5ac74-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="5ac74-131">Exchange 2013 のバックアップと復元の概念</span><span class="sxs-lookup"><span data-stu-id="5ac74-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

