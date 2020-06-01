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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: 5ec9f4303b26ea95b125adac6943945ae1276439
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456340"
---
# <a name="cchksgfilespage_info-struct"></a>CChkSGFiles.PAGE_INFO 構造体

**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
Exchange データベース ページに関する情報を保持します。 この構造体は、**ErrCheckDbPages** 関数で使用されます。 
  
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

## <a name="members"></a>Members

### <a name="ulpgno"></a>ulPgNo
  
Unsigned Long。 確認するデータベース ページの論理ページ番号。 この値は、**ErrCheckDbPages** を呼び出す前に設定しておく必要があります。 アプリケーションがファイルのオフセットに基づいてファイルを読み取る場合は、該当するファイルのオフセットを論理ページ番号にマップする必要がありますが、**PgnoFromFileOffset** メソッドは、このフィールドの値の決定に役立ちます。 **ErrCheckDbPages** は、この値を変更しません。 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
ブール. TRUE の値は、データベース ページにデータが含まれていることを表します。 FALSE の値は、ページにゼロのみが含まれていることを表します。 **ErrCheckDbPages** は、この値を設定します。 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
ブール. TRUE の値は、データベース ページに修正可能なチェックサムの不一致が検出されたことを表します。 **ErrCheckDbPages** は、この値を設定します。 
    
### <a name="checksumactual"></a>checksumActual
  
64 ビット符号なし整数。 この論理ページのデータベースに格納されているチェックサム値を表します。 **ErrCheckDbPages** は、この値を設定します。 
    
### <a name="checksumexpected"></a>checksumExpected
  
64 ビット符号なし整数。 これは、データベースページに対して計算された、予想されるチェックサム値です。これは、 **Errcheckdbpages**によって設定されます。 この値がデータベースページに格納されている値と異なる場合 (つまり、 **checksumActual**で返される値)、 **Errcheckdbpages**は、このデータベースページでエラーが検出されたことを示します。 
    
### <a name="dbtime"></a>dbTime
  
64 ビット符号なし整数。 **ErrCheckDbPages** は、このメンバーをデータベース ページのタイムスタンプに設定します。 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Unsigned 64-bt 整数。 **Errcheckdbpages**は、このメンバーをページのコンテンツの計算されたチェックサム値に設定します。データは、論理的なページの同等性を決定するときには必要ありません。 たとえば、使用されていないデータベースページ領域のデータ値を考慮する必要はありません。 このメンバーは、 **checksumActual**と**checksumExpected**の値が互いに等しい場合にのみ有効です。 
    
### <a name="ulflags"></a>ulFlags
  
64 ビット符号なし整数。 将来使用するために予約されています。 このフィールドの値は、**ErrCheckDbPages** を呼び出す前に 0 (ゼロ) に設定しておく必要があります。
    
## <a name="remarks"></a>注釈

**Errcheckdbpages**関数を呼び出すとき、 **RgPageInfo**パラメーターは**ページ \_ 情報**構造の配列です。 チェックするデータベースページごとに1つの**ページ \_ 情報**構造が必要です。 
  
アプリケーションでは、Errcheckdbpages を呼び出す前に、 **Ulcheckdbpage**を呼び出す前に、パラメーターの値を**ulpgno**に設定する必要があります。また、 **ulflags**メンバーを 0 (ゼロ) に設定する必要もあります。 
  
## <a name="requirements"></a>Requirements

Exchange Server 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

