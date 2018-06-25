---
title: CChkSGFiles.PAGE_INFO 構造体
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759801"
---
# <a name="cchksgfilespageinfo-struct"></a>CChkSGFiles.PAGE_INFO 構造体

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
Exchange データベース ページの情報を保持します。 この構造体は、 **ErrCheckDbPages**関数で使用されます。 
  
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
  
Unsigned Long です。 チェックするデータベースのページの論理ページ数です。 **ErrCheckDbPages**を呼び出す前にこの値を設定する必要があります。 アプリケーション、ファイル ・ オフセットに基づいてファイルを読み込み、そのためこれらのファイルのオフセットを論理ページ番号に対応する必要がありますに役立つ**PgnoFromFileOffset**メソッドにこのフィールドの値を決定します。 **ErrCheckDbPages**では、この値は変更されません。 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
ブール値です。 TRUE の値は、データベースのページにデータが含まれていることを示します。 FALSE の値は、ページにのみゼロが含まれていることを示します。 **ErrCheckDbPages**は、この値を設定します。 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
ブール値です。 TRUE の値は、データベース ページにチェックサムの不一致が発生しましたが、修正可能なエラーであることを示します。 **ErrCheckDbPages**は、この値を設定します。 
    
### <a name="checksumactual"></a>checksumActual
  
64 ビットの符号なし整数です。 この論理ページのデータベースに格納されているチェックサム値を示します。 **ErrCheckDbPages**は、この値を設定します。 
    
### <a name="checksumexpected"></a>checksumExpected
  
64 ビットの符号なし整数です。 これは、データベース ページに対して計算されたチェックサムの予想値**ErrCheckDbPages**で設定されています。 この値は、データベースのページに格納されている場合と異なるかどうか (つまり、値が返されます**checksumActual**で)、 **ErrCheckDbPages**はこのデータベースのページでエラーが検出されたことを示します。 
    
### <a name="dbtime"></a>dbTime
  
64 ビットの符号なし整数です。 **ErrCheckDbPages**では、データベース ページのタイムスタンプにこのメンバーを設定します。 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
64 bt の符号なし整数です。 **ErrCheckDbPages**は、このメンバーを計算されたチェックサムの値は、論理ページの等価性を決定する際に、必要なデータを除外するページの内容に設定します。 たとえば、使用されていないデータベース ページの領域のデータの値を考慮する必要はありません。 このメンバーは、 **checksumActual**および**checksumExpected**の値は互いに等しい場合に有効なだけです。 
    
### <a name="ulflags"></a>ulFlags
  
64 ビットの符号なし整数です。 将来の使用のために予約されています。 このフィールドの値は、 **ErrCheckDbPages**を呼び出す前に 0 (ゼロ) に設定する必要があります。
    
## <a name="remarks"></a>備考

**RgPageInfo**パラメーターの配列では、 **ErrCheckDbPages**関数を呼び出すときに**ページ\_情報**の構造体です。 必要がありますいずれかの**ページ\_情報**をチェックするには、各データベース ページの構造体です。 
  
アプリケーションは、適切な値に**ulPgno**のメンバーを設定する必要があり、0 (ゼロ) に**ErrCheckDbPages**を呼び出す前に**ulFlags**メンバーを設定する必要がありますも。 
  
## <a name="requirements"></a>必要条件

Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

