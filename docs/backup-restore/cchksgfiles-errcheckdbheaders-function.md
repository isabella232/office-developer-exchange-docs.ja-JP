---
title: CChkSGFiles.ErrCheckDbHeaders 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758868"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>CChkSGFiles.ErrCheckDbHeaders 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013 
  
**ErrInit**関数によって指定されているデータベース ファイルのヘッダーを検証します。 この関数では、ページ サイズとページ数も、指定されたデータベースのそれぞれに返します。 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parameters

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
出力パラメーター。指定されたデータベースごとのページ サイズ (バイト単位)。
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
出力パラメーターです。 それぞれの先頭ページの数は、内部で使用するデータベース エンジンによって予約されているデータベースを指定します。 *検証のための**ErrCheckDbPages**関数をヘッダー ページをパス*する必要があることに注意してください。 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
出力パラメーターです。 関数の戻り値がエラーを示す場合、このパラメーターは、 **ErrInit**関数に渡される**rgwszDb の**配列へのインデックスを指定します。 インデックス付きの配列要素は、エラーが検出されたデータベースを表します。 関数がエラー値を返さない場合、このパラメーターの値は有効ではありません。 
    
### <a name="ulflags"></a>ulFlags 
  
オプションの入力パラメーター。この値は、将来使用するために予約されています。渡された値は、0 (ゼロ) になります。
    
## <a name="return-value"></a>�߂�l

この関数は、 [CChkSGFiles.ERR 列挙型](cchksgfiles-err-enumeration.md)のエラー コードを返します。
  
## <a name="remarks"></a>備考

**ErrCheckDbHeaders**は、同じログとデータベースの署名ページのサイズを**ErrInit**に登録されているすべてのデータベースがあることを確認します。 クリーン シャット ダウン状態にするためのすべての登録されているデータベースに必要なログ ファイルのセットを決定するのには、 **genMin**パラメーターの値が最小と最大の**genMax**パラメーターの値を使用することもできます。 
  
エラーが検出された場合にのみ、 **piDbErrorEncountered**パラメーターが設定されて、 **ErrCheckDbHeaders**の戻り値に 0 以外で示されるようにします。 
  
この関数でエラーが発生すると、エラー イベントが Windows エラー イベント ログに追加されます。
  
**ErrInit**を呼び出した後にだけ、 **ErrCheckDbHeaders**を呼び出すことができますし、 **ErrCheckDbPages**と**ErrCheckLogs**を呼び出す前に呼び出す必要があります。
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、部分では、シングル スレッド、 **ErrCheckDbHeaders**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

