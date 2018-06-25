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
# <a name="cchksgfiles-class-reference"></a>CChkSGFiles クラスの参照

Exchange 2013 に CHKSGFILES API のリファレンス情報を検索します。
  
**に適用されます:** Exchange Server 2013 
  
CHKSGFILES API では、プログラムを使用して Exchange Server 2013 のトランザクション ログ ファイルとデータベースの整合性を確認するのにはバックアップと復元のアプリケーションを使用できます。 バックアップではこの API を使用し、ボリューム シャドウ コピー サービス (VSS) を使用するアプリケーションを復元できます。
  
> [!NOTE]
> ストレージ ・ グループは利用可能な Exchange 2013 です。 バージョンの Exchange が Exchange Server 2010 で始まるから、ストレージ ・ グループのサポートが削除されました。 CHKSGFILES API では、データベースと Exchange 2010 より前のバージョンの Exchange ストレージ ・ グループとの下位互換性のため、ストレージ ・ グループを指定できます。 Exchange 2013 のデータベースに対して CHKSGFILES を実行するときは、空の文字列にストレージ ・ グループの識別子を指定するパラメーターを設定してください。 
  
## <a name="file-location"></a>ファイルの場所
<a name="bk_fileslocation"> </a>

CHKSGFILES API は、Exchange 2013 の一部として組み込まれています。 メールボックス サーバーの役割がインストールされているコンピューターでは、この API を使用できます。 
  
既定では、CHKSGFILES DLL は C:\Program Files\Microsoft\Exchange\V15\Bin ディレクトリにインストールされます。
  
Exchange 2013 には、CHKSGFILES api (amd64) の 64 ビット バージョンのみが含まれています。 
  
[Microsoft ダウンロード センター](http://www.microsoft.com/en-us/download/details.aspx?id=36802)から、カスタムのアプリケーションでは、CHKSGFILE.lib ライブラリが含まれている .zip ファイルと使用するための CHKSGFILES.hxx ヘッダー ファイルをダウンロードできます。
  
## <a name="development-languages"></a>開発言語
<a name="bk_developmentlanguages"> </a>

CHKSGFILES API は、ネイティブ C または C++ での Visual Studio 2005 以降で、Visual Studio のバージョンで使用する目的としています。 CHKSGFILES API は、マネージ コードで使用するためのものではありません。 CHKSGFILES と COM 相互運用機能アセンブリを作成できますが、配送は行っておりません Exchange 2013 で、サポートされている COM 相互運用機能アセンブリです。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [CChkSGFiles.CMaxDbPerSG 関数](cchksgfiles-cmaxdbpersg-function.md)
    
- [CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)
    
- [CChkSGFiles.ERR 列挙型](cchksgfiles-err-enumeration.md)
    
- [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)
    
- [CChkSGFiles.ErrCheckDbPages 関数](cchksgfiles-errcheckdbpages-function.md)
    
- [CChkSGFiles.ErrCheckLogs 関数](cchksgfiles-errchecklogs-function.md)
    
- [(予約済み) の CChkSGFiles.ErrGetHeader 関数](cchksgfiles-errgetheader-function-reserved.md)
    
- [CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)
    
- [CChkSGFiles.ErrTerm 関数](cchksgfiles-errterm-function.md)
    
- [CChkSGFiles.iDbInvalid 列挙型](cchksgfiles-idbinvalid-enumeration.md)
    
- [CChkSGFiles.New 関数](cchksgfiles-new-function.md)
    
- [CChkSGFiles.NO_FLAGS 列挙型](cchksgfiles-no_flags-enumeration.md)
    
- [CChkSGFiles.PAGE_INFO 構造体](cchksgfiles-page_info-struct.md)
    
- [CChkSGFiles.PgnoFromFileOffset 関数](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>関連項目

- [オンラインの Exchange および Exchange の開発](../exchange-server-development.md)
- [バックアップ、復元、および災害復旧](http://technet.microsoft.com/en-us/library/dd876874)
    

