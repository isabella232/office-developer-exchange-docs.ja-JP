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
# <a name="cchksgfiles-class-reference"></a>CChkSGFiles クラスの参照

Exchange 2013 の CHKSGFILES API に関するリファレンス情報について紹介します。
  
**製品:** Exchange Server 2013 
  
CHKSGFILES API を使用すると、バックアップおよび復元アプリケーションで、Exchange Server 2013 トランザクションログファイルとデータベースの整合性をプログラムによって確認できます。 この API は、ボリューム シャドウ コピー サービス (VSS) を使用するバックアップおよび復元アプリケーションで使用できます。
  
> [!NOTE]
> ストレージグループは、Exchange 2013 では使用できません。 ストレージグループのサポートは、Exchange Server 2010 以降のバージョンの Exchange から削除されました。 Exchange 2010 より前のバージョンの Exchange でデータベースおよびストレージグループとの下位互換性を維持するために、CHKSGFILES API ではストレージグループを指定できます。 Exchange 2013 データベースに対して CHKSGFILES を実行するときは、ストレージグループ識別子を指定するパラメーターを空の文字列に設定する必要があります。 
  
## <a name="file-location"></a>ファイルの場所
<a name="bk_fileslocation"> </a>

CHKSGFILES API は、Exchange 2013 の一部として出荷されます。 この API は、メールボックス サーバーの役割をインストールしたコンピューター上で使用できます。 
  
既定では、CHKSGFILES DLL は C:\Program Files\Microsoft\Exchange\V15\Bin ディレクトリにインストールされます。
  
Exchange 2013 には、CHKSGFILES API の64ビット (amd64) バージョンのみが含まれています。 
  
CHKSGFILE ライブラリおよび CHKSGFILES のヘッダーファイルを含む .zip ファイルは、 [Microsoft ダウンロードセンター](https://www.microsoft.com/download/details.aspx?id=36802)からカスタムアプリケーションで使用するためにダウンロードできます。
  
## <a name="development-languages"></a>開発言語
<a name="bk_developmentlanguages"> </a>

CHKSGFILES API は、visual studio 2005 (ネイティブ C/c + +) 以降のバージョンの Visual Studio で使用することを目的としています。 CHKSGFILES API は、マネージ コードでの使用を目的としていません。 COM 相互運用機能アセンブリは CHKSGFILES を使用して作成できますが、Exchange 2013 でサポートされている COM 相互運用機能アセンブリは提供していません。
  
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
    

