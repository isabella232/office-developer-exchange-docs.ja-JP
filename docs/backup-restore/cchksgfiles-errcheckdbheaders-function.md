---
title: CChkSGFiles.ErrCheckDbHeaders 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 215a0d1126fce48b7e3800016619b0c52915312b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510471"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>CChkSGFiles.ErrCheckDbHeaders 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013 
  
**ErrInit** 関数で指定されたデータベース ファイルのヘッダーを検証します。この関数は、指定されたデータベースごとのページ サイズとページ数も返します。 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>パラメーター

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
出力パラメーター。指定されたデータベースごとのページ サイズ (バイト単位)。
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
出力パラメーター。指定された各データベースの開始時のページ数。データベース エンジンによって、このページ数が内部使用のために予約されます。検証のために、**ErrCheckDbPages** 関数にヘッダー ページを渡しては *いけません*。 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
出力パラメーター。関数の戻り値がエラーを示している場合、このパラメーターは **ErrInit** 関数に渡した **rgwszDb[]** 配列のインデックスになります。インデックスで示された配列の要素は、エラーが発生したデータベースを表します。関数がエラー値を返さない場合、このパラメーターの値は無効になります。 
    
### <a name="ulflags"></a>ulFlags 
  
オプションの入力パラメーター。この値は、将来使用するために予約されています。渡された値は、0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

この関数は [、CChkSGFiles.ERR 列挙からエラー コードを返します](cchksgfiles-err-enumeration.md)。
  
## <a name="remarks"></a>注釈

**ErrCheckDbHeaders** は、**ErrInit** によって登録したすべてのデータベースで、ログ署名とデータベース ページ サイズが同じであることを検証します。また、最小の **genMin** パラメーター値と、最大の **genMax** パラメーター値を使用することで、登録されたすべてのデータベースをクリーン シャットダウン状態にするために必要になるログ ファイルのセットを決定することもできます。 
  
**piDbErrorEncountered** パラメーターは、ゼロ以外の **ErrCheckDbHeaders** の戻り値で示されるエラーが検出された場合にのみ設定されます。 
  
この関数でエラーが発生すると、エラー イベントが Windows エラー イベント ログに追加されます。
  
**ErrCheckDbHeaders** は、**ErrInit** を呼び出した後にのみ呼び出せるようになり、**ErrCheckDbPages** および **ErrCheckLogs** を呼び出す前に呼び出す必要があります。
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、シングル スレッド部分で **ErrCheckDbHeaders** 関数を呼び出す必要があります。また **、CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出す必要があります。 
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

