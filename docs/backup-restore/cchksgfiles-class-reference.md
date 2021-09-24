---
title: CChkSGFiles クラスの参照
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Exchange 2013 の CHKSGFILES API に関するリファレンス情報について紹介します。
ms.openlocfilehash: 2daf31c41a47684b85ede196b415884335c3ca79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510534"
---
# <a name="cchksgfiles-class-reference"></a>CChkSGFiles クラスの参照

Exchange 2013 の CHKSGFILES API に関するリファレンス情報について紹介します。
  
**製品:** Exchange Server 2013 
  
CHKSGFILES API を使用すると、アプリケーションのバックアップと復元を行って、Exchange Server 2013 トランザクション ログ ファイルとデータベースの整合性をプログラムで検証できます。 この API は、ボリューム シャドウ コピー サービス (VSS) を使用するバックアップおよび復元アプリケーションで使用できます。
  
> [!NOTE]
> Storageグループは 2013 年Exchangeできません。 ストレージ グループのサポートは、2010 年ExchangeバージョンExchange Serverされました。 Exchange のバージョンが Exchange 2010 より前のバージョンのデータベースおよびストレージ グループとの下位互換性を保つには、CHKSGFILES API を使用してストレージ グループを指定できます。 CHKSGFILES を 2013 Exchangeデータベースに対して実行する場合は、ストレージ グループ識別子を指定するパラメーターを空の文字列に設定する必要があります。 
  
## <a name="file-location"></a>ファイルの場所
<a name="bk_fileslocation"> </a>

CHKSGFILES API は、2013 年にExchangeされます。 この API は、メールボックス サーバーの役割をインストールしたコンピューター上で使用できます。 
  
既定では、CHKSGFILES DLL は C:\Program Files\Microsoft\Exchange\V15\Bin ディレクトリにインストールされます。
  
Exchange 2013 には、CHKSGFILES API の 64 ビット (amd64) バージョンだけが含まれています。 
  
カスタム アプリケーションで使用する CHKSGFILE.lib ライブラリと CHKSGFILES.hxx ヘッダー ファイルを含む .zip ファイルを [Microsoft](https://www.microsoft.com/download/details.aspx?id=36802)ダウンロード センターからダウンロードできます。
  
## <a name="development-languages"></a>開発言語
<a name="bk_developmentlanguages"> </a>

CHKSGFILES API は、ネイティブ C/C++ の Visual Studio 2005 Visual Studioバージョンで使用することを目的とします。 CHKSGFILES API は、マネージ コードでの使用を目的としていません。 CHKSGFILES を使用して COM 相互運用機能アセンブリを作成することもできますが、サポートされている COM 相互運用機能アセンブリは 2013 年Exchangeされません。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [CChkSGFiles.CMaxDbPerSG 関数](cchksgfiles-cmaxdbpersg-function.md)
    
- [CChkSGFiles.Delete 関数](cchksgfiles-delete-function.md)
    
- [CChkSGFiles.ERR 列挙型](cchksgfiles-err-enumeration.md)
    
- [CChkSGFiles.ErrCheckDbHeaders 関数](cchksgfiles-errcheckdbheaders-function.md)
    
- [CChkSGFiles.ErrCheckDbPages 関数](cchksgfiles-errcheckdbpages-function.md)
    
- [CChkSGFiles.ErrCheckLogs 関数](cchksgfiles-errchecklogs-function.md)
    
- [CChkSGFiles.ErrGetHeader 関数 (予約済み)](cchksgfiles-errgetheader-function-reserved.md)
    
- [CChkSGFiles.ErrInit 関数](cchksgfiles-errinit-function.md)
    
- [CChkSGFiles.ErrTerm 関数](cchksgfiles-errterm-function.md)
    
- [CChkSGFiles.iDbInvalid 列挙型](cchksgfiles-idbinvalid-enumeration.md)
    
- [CChkSGFiles.New 関数](cchksgfiles-new-function.md)
    
- [CChkSGFiles.NO_FLAGS 列挙型](cchksgfiles-no_flags-enumeration.md)
    
- [CChkSGFiles.PAGE_INFO 構造体](cchksgfiles-page_info-struct.md)
    
- [CChkSGFiles.PgnoFromFileOffset 関数](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>関連項目

- [Exchange Online と Exchange の開発](../exchange-server-development.md)
- [バックアップ、復元、および障害回復](https://technet.microsoft.com/library/dd876874)
    

