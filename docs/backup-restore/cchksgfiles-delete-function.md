---
title: CChkSGFiles.Delete 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758862"
---
# <a name="cchksgfilesdelete-function"></a>CChkSGFiles.Delete 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
**CChkSGFiles**クラスの既存のインスタンスを破棄します。 アプリケーションが指定したオブジェクトの操作を完了した後は、この関数を呼び出す必要があります。 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Parameters

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
パラメーターを入力します。 既存の**CCheckSGFiles**オブジェクトへのポインター。 オブジェクトに関連付けられているメモリを解放し、されます。 
    
## <a name="return-value"></a>Return value

なし。
  
## <a name="remarks"></a>備考

**削除**関数は、 **CCheckSGFiles**オブジェクトに関連付けられているメモリを解放します。 **削除**を呼び出すと、 *pcchecksgfiles*パラメーターに渡されたポインターが無効になりそのオブジェクトの他の操作を実行されません。 
  
アプリケーションがメモリ バッファーを手動で解放する必要がありますアプリケーションでは、 **ErrCheckDbPages**関数を使用する場合**削除**関数では、解放はしません。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、シングル スレッド アプリケーションの部分で**削除**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

