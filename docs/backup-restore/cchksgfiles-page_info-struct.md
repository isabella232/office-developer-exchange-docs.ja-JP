---
title: CChkSGFiles.PAGE_INFO 構造体
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: f324ec9aca6f94911041c227ce039139292a10aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516259"
---
# <a name="cchksgfilespage_info-struct"></a>CChkSGFiles.PAGE_INFO 構造体

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
Exchange データベース ページに関する情報を保持します。この構造体は、**ErrCheckDbPages** 関数で使用されます。  
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a>メンバー

### <a name="ulpgno"></a>ulPgNo
  
Unsigned Long。確認するデータベース ページの論理ページ番号。この値は、**ErrCheckDbPages** を呼び出す前に設定しておく必要があります。アプリケーションがファイルのオフセットに基づいてファイルを読み取る場合は、該当するファイルのオフセットを論理ページ番号にマップする必要がありますが、**PgnoFromFileOffset** メソッドは、このフィールドの値の決定に役立ちます。**ErrCheckDbPages** は、この値を変更しません。 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
ブール値。TRUE の値は、データベース ページにデータが含まれていることを表します。FALSE の値は、ページにゼロのみが含まれていることを表します。**ErrCheckDbPages** は、この値を設定します。 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
ブール値。TRUE の値は、データベース ページに修正可能なチェックサムの不一致が検出されたことを表します。**ErrCheckDbPages** は、この値を設定します。 
    
### <a name="checksumactual"></a>チェックサムActual
  
64 ビット符号なし整数。この論理ページのデータベースに格納されているチェックサム値を表します。**ErrCheckDbPages** は、この値を設定します。 
    
### <a name="checksumexpected"></a>チェックサムExpected
  
64 ビット符号なし整数。データベース ページについて計算された予想チェックサム値です。**ErrCheckDbPages** によって設定されます。この値がデータベース ページに格納されている値 (**checksumActual** で返される値) と異なる場合、**ErrCheckDbPages** は、このデータベース ページでエラーが見つかったことを表します。 
    
### <a name="dbtime"></a>dbTime
  
64 ビット符号なし整数。**ErrCheckDbPages** は、このメンバーをデータベース ページのタイムスタンプに設定します。 
    
### <a name="checksumpagestructure"></a>チェックサムPageStructure 
  
符号なし 64-bt 整数。 **ErrCheckDbPages** は、このメンバーを、論理ページの同等性を決定する際に不要なデータを除いて、ページの内容の計算されたチェックサム値に設定します。 たとえば、未使用のデータベース ページ領域のデータ値を考慮する必要は不要です。 このメンバーは、**チェックサムActual およびチェックサムExpected 値** が互いに等しい場合にのみ有効です。  
    
### <a name="ulflags"></a>ulFlags
  
64 ビット符号なし整数。将来使用するために予約されています。このフィールドの値は、**ErrCheckDbPages** を呼び出す前に 0 (ゼロ) に設定しておく必要があります。
    
## <a name="remarks"></a>注釈

**ErrCheckDbPages** 関数を呼び出す場合 **、rgPageInfo** パラメーターは **PAGE \_ INFO 構造体の配列** です。 チェックするデータベース ページごとに **\_ 1** つの PAGE INFO 構造が必要です。 
  
アプリケーションは **ulPgno** メンバーを適切な値に設定し **、ErrCheckDbPages** を呼び出す前に **ulFlags** メンバーを 0 (ゼロ) に設定する必要があります。 
  
## <a name="requirements"></a>要件

Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

