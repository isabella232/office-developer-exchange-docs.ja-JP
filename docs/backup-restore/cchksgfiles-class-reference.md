---
title: CChkSGFiles クラスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Exchange 2013 の CHKSGFILES API に関するリファレンス情報について紹介します。
ms.openlocfilehash: 38b1f2c900767c22594636f0c6ddf4855961aec4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526733"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="07a85-103">CChkSGFiles クラスの参照</span><span class="sxs-lookup"><span data-stu-id="07a85-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="07a85-104">Exchange 2013 の CHKSGFILES API に関するリファレンス情報について紹介します。</span><span class="sxs-lookup"><span data-stu-id="07a85-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="07a85-105">**製品:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="07a85-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="07a85-106">CHKSGFILES API を使用すると、バックアップおよび復元アプリケーションで、Exchange Server 2013 トランザクションログファイルとデータベースの整合性をプログラムによって確認できます。</span><span class="sxs-lookup"><span data-stu-id="07a85-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="07a85-107">この API は、ボリューム シャドウ コピー サービス (VSS) を使用するバックアップおよび復元アプリケーションで使用できます。</span><span class="sxs-lookup"><span data-stu-id="07a85-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="07a85-108">ストレージグループは、Exchange 2013 では使用できません。</span><span class="sxs-lookup"><span data-stu-id="07a85-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="07a85-109">ストレージグループのサポートは、Exchange Server 2010 以降のバージョンの Exchange から削除されました。</span><span class="sxs-lookup"><span data-stu-id="07a85-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="07a85-110">Exchange 2010 より前のバージョンの Exchange でデータベースおよびストレージグループとの下位互換性を維持するために、CHKSGFILES API ではストレージグループを指定できます。</span><span class="sxs-lookup"><span data-stu-id="07a85-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="07a85-111">Exchange 2013 データベースに対して CHKSGFILES を実行するときは、ストレージグループ識別子を指定するパラメーターを空の文字列に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="07a85-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="07a85-112">ファイルの場所</span><span class="sxs-lookup"><span data-stu-id="07a85-112">File location</span></span>
<span data-ttu-id="07a85-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="07a85-113"><a name="bk_fileslocation"> </a></span></span>

<span data-ttu-id="07a85-114">CHKSGFILES API は、Exchange 2013 の一部として出荷されます。</span><span class="sxs-lookup"><span data-stu-id="07a85-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="07a85-115">この API は、メールボックス サーバーの役割をインストールしたコンピューター上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="07a85-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="07a85-116">既定では、CHKSGFILES DLL は C:\Program Files\Microsoft\Exchange\V15\Bin ディレクトリにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="07a85-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="07a85-117">Exchange 2013 には、CHKSGFILES API の64ビット (amd64) バージョンのみが含まれています。</span><span class="sxs-lookup"><span data-stu-id="07a85-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="07a85-118">CHKSGFILE ライブラリおよび CHKSGFILES のヘッダーファイルを含む .zip ファイルは、 [Microsoft ダウンロードセンター](https://www.microsoft.com/download/details.aspx?id=36802)からカスタムアプリケーションで使用するためにダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="07a85-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="07a85-119">開発言語</span><span class="sxs-lookup"><span data-stu-id="07a85-119">Development languages</span></span>
<span data-ttu-id="07a85-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="07a85-120"><a name="bk_developmentlanguages"> </a></span></span>

<span data-ttu-id="07a85-121">CHKSGFILES API は、visual studio 2005 (ネイティブ C/c + +) 以降のバージョンの Visual Studio で使用することを目的としています。</span><span class="sxs-lookup"><span data-stu-id="07a85-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="07a85-122">CHKSGFILES API は、マネージ コードでの使用を目的としていません。</span><span class="sxs-lookup"><span data-stu-id="07a85-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="07a85-123">COM 相互運用機能アセンブリは CHKSGFILES を使用して作成できますが、Exchange 2013 でサポートされている COM 相互運用機能アセンブリは提供していません。</span><span class="sxs-lookup"><span data-stu-id="07a85-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="07a85-124">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="07a85-124">In this section</span></span>
<span data-ttu-id="07a85-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="07a85-125"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="07a85-126">CChkSGFiles.CMaxDbPerSG 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="07a85-127">CChkSGFiles.Delete 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="07a85-128">CChkSGFiles.ERR 列挙型</span><span class="sxs-lookup"><span data-stu-id="07a85-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="07a85-129">CChkSGFiles.ErrCheckDbHeaders 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="07a85-130">CChkSGFiles.ErrCheckDbPages 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="07a85-131">CChkSGFiles.ErrCheckLogs 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="07a85-132">CChkSGFiles.ErrGetHeader 関数 (予約済み)</span><span class="sxs-lookup"><span data-stu-id="07a85-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="07a85-133">CChkSGFiles.ErrInit 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="07a85-134">CChkSGFiles.ErrTerm 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="07a85-135">CChkSGFiles.iDbInvalid 列挙型</span><span class="sxs-lookup"><span data-stu-id="07a85-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="07a85-136">CChkSGFiles.New 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="07a85-137">CChkSGFiles.NO_FLAGS 列挙型</span><span class="sxs-lookup"><span data-stu-id="07a85-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="07a85-138">CChkSGFiles.PAGE_INFO 構造体</span><span class="sxs-lookup"><span data-stu-id="07a85-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="07a85-139">CChkSGFiles.PgnoFromFileOffset 関数</span><span class="sxs-lookup"><span data-stu-id="07a85-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="07a85-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="07a85-140">See also</span></span>

- [<span data-ttu-id="07a85-141">Exchange Online と Exchange の開発</span><span class="sxs-lookup"><span data-stu-id="07a85-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="07a85-142">バックアップ、復元、および障害回復</span><span class="sxs-lookup"><span data-stu-id="07a85-142">Backup, Restore, and Disaster Recovery</span></span>](https://technet.microsoft.com/library/dd876874)
    

