---
title: CChkSGFiles クラスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Exchange 2013 に CHKSGFILES API のリファレンス情報を検索します。
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758863"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="40a11-103">CChkSGFiles クラスの参照</span><span class="sxs-lookup"><span data-stu-id="40a11-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="40a11-104">Exchange 2013 に CHKSGFILES API のリファレンス情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="40a11-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="40a11-105">**に適用されます:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="40a11-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="40a11-106">CHKSGFILES API では、プログラムを使用して Exchange Server 2013 のトランザクション ログ ファイルとデータベースの整合性を確認するのにはバックアップと復元のアプリケーションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="40a11-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="40a11-107">バックアップではこの API を使用し、ボリューム シャドウ コピー サービス (VSS) を使用するアプリケーションを復元できます。</span><span class="sxs-lookup"><span data-stu-id="40a11-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="40a11-108">ストレージ ・ グループは利用可能な Exchange 2013 です。</span><span class="sxs-lookup"><span data-stu-id="40a11-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="40a11-109">バージョンの Exchange が Exchange Server 2010 で始まるから、ストレージ ・ グループのサポートが削除されました。</span><span class="sxs-lookup"><span data-stu-id="40a11-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="40a11-110">CHKSGFILES API では、データベースと Exchange 2010 より前のバージョンの Exchange ストレージ ・ グループとの下位互換性のため、ストレージ ・ グループを指定できます。</span><span class="sxs-lookup"><span data-stu-id="40a11-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="40a11-111">Exchange 2013 のデータベースに対して CHKSGFILES を実行するときは、空の文字列にストレージ ・ グループの識別子を指定するパラメーターを設定してください。</span><span class="sxs-lookup"><span data-stu-id="40a11-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="40a11-112">ファイルの場所</span><span class="sxs-lookup"><span data-stu-id="40a11-112">File location</span></span>
<span data-ttu-id="40a11-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="40a11-113"></span></span>

<span data-ttu-id="40a11-114">CHKSGFILES API は、Exchange 2013 の一部として組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="40a11-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="40a11-115">メールボックス サーバーの役割がインストールされているコンピューターでは、この API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="40a11-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="40a11-116">既定では、CHKSGFILES DLL は C:\Program Files\Microsoft\Exchange\V15\Bin ディレクトリにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="40a11-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="40a11-117">Exchange 2013 には、CHKSGFILES api (amd64) の 64 ビット バージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="40a11-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="40a11-118">[Microsoft ダウンロード センター](http://www.microsoft.com/en-us/download/details.aspx?id=36802)から、カスタムのアプリケーションでは、CHKSGFILE.lib ライブラリが含まれている .zip ファイルと使用するための CHKSGFILES.hxx ヘッダー ファイルをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="40a11-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="40a11-119">開発言語</span><span class="sxs-lookup"><span data-stu-id="40a11-119">Development languages</span></span>
<span data-ttu-id="40a11-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="40a11-120"></span></span>

<span data-ttu-id="40a11-121">CHKSGFILES API は、ネイティブ C または C++ での Visual Studio 2005 以降で、Visual Studio のバージョンで使用する目的としています。</span><span class="sxs-lookup"><span data-stu-id="40a11-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="40a11-122">CHKSGFILES API は、マネージ コードで使用するためのものではありません。</span><span class="sxs-lookup"><span data-stu-id="40a11-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="40a11-123">CHKSGFILES と COM 相互運用機能アセンブリを作成できますが、配送は行っておりません Exchange 2013 で、サポートされている COM 相互運用機能アセンブリです。</span><span class="sxs-lookup"><span data-stu-id="40a11-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="40a11-124">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="40a11-124">In this section</span></span>
<span data-ttu-id="40a11-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="40a11-125"></span></span>

- [<span data-ttu-id="40a11-126">CChkSGFiles.CMaxDbPerSG 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="40a11-127">CChkSGFiles.Delete 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="40a11-128">CChkSGFiles.ERR 列挙型</span><span class="sxs-lookup"><span data-stu-id="40a11-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="40a11-129">CChkSGFiles.ErrCheckDbHeaders 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="40a11-130">CChkSGFiles.ErrCheckDbPages 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="40a11-131">CChkSGFiles.ErrCheckLogs 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="40a11-132">(予約済み) の CChkSGFiles.ErrGetHeader 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="40a11-133">CChkSGFiles.ErrInit 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="40a11-134">CChkSGFiles.ErrTerm 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="40a11-135">CChkSGFiles.iDbInvalid 列挙型</span><span class="sxs-lookup"><span data-stu-id="40a11-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="40a11-136">CChkSGFiles.New 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="40a11-137">CChkSGFiles.NO_FLAGS 列挙型</span><span class="sxs-lookup"><span data-stu-id="40a11-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="40a11-138">CChkSGFiles.PAGE_INFO 構造体</span><span class="sxs-lookup"><span data-stu-id="40a11-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="40a11-139">CChkSGFiles.PgnoFromFileOffset 関数</span><span class="sxs-lookup"><span data-stu-id="40a11-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="40a11-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="40a11-140">See also</span></span>

- [<span data-ttu-id="40a11-141">オンラインの Exchange および Exchange の開発</span><span class="sxs-lookup"><span data-stu-id="40a11-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="40a11-142">バックアップ、復元、および災害復旧</span><span class="sxs-lookup"><span data-stu-id="40a11-142">Backup, Restore, and Disaster Recovery</span></span>](http://technet.microsoft.com/en-us/library/dd876874)
    

