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
description: '最終更新日: 2013 年2月22日'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455248"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>CChkSGFiles.ErrCheckDbHeaders 関数

**適用対象:** Exchange Server 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013 
  
**ErrInit** 関数で指定されたデータベース ファイルのヘッダーを検証します。 この関数は、指定されたデータベースごとのページ サイズとページ数も返します。 
  
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
  
出力パラメーターです。 データベースエンジンによって内部使用のために予約されている、指定された各データベースの最初のページ数。 検証のために、ヘッダーページを**Errcheckdbpages**関数に渡さ*ない*ように注意してください。 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
出力パラメーターです。 関数の戻り値がエラーを示している場合、このパラメーターは **ErrInit** 関数に渡した **rgwszDb[]** 配列のインデックスになります。 インデックスで示された配列の要素は、エラーが発生したデータベースを表します。 関数がエラー値を返さない場合、このパラメーターの値は無効になります。 
    
### <a name="ulflags"></a>ulFlags 
  
オプションの入力パラメーター。この値は、将来使用するために予約されています。渡された値は、0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

この関数は、 [CChkSGFiles 列挙](cchksgfiles-err-enumeration.md)からエラーコードを返します。
  
## <a name="remarks"></a>注釈

**ErrCheckDbHeaders** は、**ErrInit** によって登録したすべてのデータベースで、ログ署名とデータベース ページ サイズが同じであることを検証します。 また、最小の **genMin** パラメーター値と、最大の **genMax** パラメーター値を使用することで、登録されたすべてのデータベースをクリーン シャットダウン状態にするために必要になるログ ファイルのセットを決定することもできます。 
  
**piDbErrorEncountered** パラメーターは、ゼロ以外の **ErrCheckDbHeaders** の戻り値で示されるエラーが検出された場合にのみ設定されます。 
  
この関数でエラーが発生すると、エラー イベントが Windows エラー イベント ログに追加されます。
  
**ErrCheckDbHeaders** は、**ErrInit** を呼び出した後にのみ呼び出せるようになり、**ErrCheckDbPages** および **ErrCheckLogs** を呼び出す前に呼び出す必要があります。
  
マルチスレッドアプリケーションで CHKSGFILES を使用している場合は、単一スレッドの部分で**Errcheckdbheaders**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに1回だけ呼び出すことができます。 
  
## <a name="requirements"></a>Requirements

Exchange 2013 には、CHKSGFILES API の64ビットバージョンのみが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

