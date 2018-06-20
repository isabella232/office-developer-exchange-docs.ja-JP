---
title: CChkSGFiles.ErrCheckDbPages 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758861"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>CChkSGFiles.ErrCheckDbPages 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
指定したデータベースのページの範囲を検証します。  
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parameters

### <a name="idb"></a>iDb
  
パラメーターを入力します。 **ErrInit**関数に**rgwszDb の**パラメーターで指定されたデータベースの配列へのインデックスです。 このパラメーターでインデックス付けされたデータベースがチェックされます。 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
パラメーターを入力します。 チェックする 1 つまたは複数のデータベース ページを格納するバッファーへのポインター。 バッファーのサイズは、 **ErrCheckDbHeaders**関数によって、 **pcbDbPageSize**パラメーターで返されると、データベースのページ サイズの倍数にすることがあります。 呼び出し元のアプリケーションは、 **ErrCheckDbPages**を呼び出す前にデータベース ページの内容をバッファーに読み込む必要があります。
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
パラメーターを入力します。 **PvPageBuffer**パラメーターのバイト単位のサイズです。 この値は、 **ErrCheckDbHeaders**関数によって、 **pcbDbPageSize**パラメーターで返されると、データベースのページ サイズの倍数にすることがあります。 
    
### <a name="rgpageinfo"></a>rgPageInfo 
  
入力/出力パラメーターです。 配列の**ページ\_情報**構造体の**ErrCheckDbPages**が、チェックされている各データベース ・ ページの結果を詳しく説明します。 配列の各**ulPgno**フィールドと、 **pvPageBuffer**パラメーターで渡された各データベース ・ ページの要素が 1 つ必要があります**ページ\_情報**構造は、データベースのページに対応する論理ページ番号を設定する必要があります。 詳細については、このトピックの後半の「解説」を参照してください。 
    
### <a name="cpageinfo"></a>cPageInfo
  
パラメーターを入力します。 **RgPageInfo**配列内のエントリの数です。 この値は、 **pvPageBuffer**パラメーターで渡されたデータベース ・ ページの数と同じである必要があります。 
    
### <a name="ulflags"></a>ulFlags 
  
オプションの入力パラメーター。この値は、将来使用するために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>�߂�l

[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。 
  
## <a name="remarks"></a>備考

データベースのデータベースは、 **ErrInit**関数に渡される配列に指定する必要があることに注意してください。 また、 **ErrCheckDbHeaders**を**ErrCheckDbPages**する前に呼び出す必要があります。
  
呼び出し元のアプリケーションでは、確認対象のデータベース ページを保持できる大きさのメモリ バッファーを割り当てる必要があります。アプリケーションでは、このバッファーに、1 つ以上の該当するデータベース ページのコンテンツを設定する必要があります。  
  
呼び出し元のアプリケーションでは、 **ErrCheckDbPages**を呼び出す前に**ErrCheckDbHeaders**を呼び出す必要があります。 確認されるすべてのデータベース ファイル内のすべてのページをカバーするために必要な回数だけこの関数を呼び出すことができます。
  
**RgPageInfo**のパラメーターに返される各要素にで [データベース] ページについての情報が含まれています、**ページ\_情報**構造体です。 アプリケーションをそれぞれ確認する**ErrCheckDbPages**関数がエラーを返した場合は、**ページ\_情報**ページで、エラーが検出されましたを決定します。 たとえば、 **checksumActual**および**checksumExpected**の値を比較するには、そのデータベース ページのチェックサム エラーが検出されたかどうか示されます。 
  
**ErrCheckDbPages**がデータベースの内容のすべてのエラーを検出すると、Windows のエラーのイベント ログ エントリを作成します。 
  
**CChkSGFiles**オブジェクトは、 **ErrInit**関数を使用して登録されているすべてのデータベースが実際にチェック アウトするかどうかを決定します。 具体的には、 **CChkSGFiles**では、 **ErrCheckDbPages**関数を使用して、 **ErrCheckDbHeaders**で指定されたデータベース ・ ページ数が同じが実際に検証されたかどうかを決定します。 正しい数の各データベース内のページが正常にチェックしない場合、 **ErrTerm**関数はエラーを返します。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **ErrCheckDbPages**関数を呼び出すことができます。 **ErrCheckDbPages**は、通常という名前の複数回チェックされているデータベースごとに注意してください。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

