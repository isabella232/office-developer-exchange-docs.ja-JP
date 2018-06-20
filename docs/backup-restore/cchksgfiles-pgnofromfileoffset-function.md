---
title: CChkSGFiles.PgnoFromFileOffset 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758869"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>CChkSGFiles.PgnoFromFileOffset 関数

**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
物理データベース ・ ファイルで指定したバイトのインデックスを作成するには、対応するデータベースの論理ページ番号を返します。 ファイル オフセットが正しくない場合、またはデータベースの**ErrCheckDbHeaders**関数が呼び出されていない場合は、この関数は 0 (ゼロ) を返します。 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Parameters

### <a name="ibfileoffset"></a>ibFileOffset
  
入力パラメーター。データベース ファイル内のオフセット (バイト単位)。
    
## <a name="return-value"></a>�߂�l

指定したオフセットを含んでいるデータベース ファイルの論理ページ番号。
  
## <a name="remarks"></a>備考

**IbFileOffset**パラメーターが有効でない場合、 **PgnoFromFileOffset**関数は、0 (ゼロ) を返します。 
  
**PgnoFromFileOffset**は、 **CCheckSGFiles**インスタンス上で、 **ErrCheckDbHeaders**関数を呼び出していない場合にも 0 (ゼロ) を返します。 データベース ヘッダーに割り当てられたページの数、データベースのページ サイズを初期化するために**ErrCheckDbHeaders**を呼び出す必要があります。 
  
入力するのには**PgnoFromFileOffset**を使用する必要があります、**ページ\_情報** **ErrCheckDbPages**を呼び出すための準備としての要素を構造化します。 **ErrCheckDbPages**に**rgPageInfo**パラメーターでは、配列の各要素が**ulPgno**メンバーの値が正しく初期化されると、 **PAGE_INFO**構造体である必要があります。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、マルチ スレッド アプリケーションの部分に、 **PgnoFromFileOffset**関数を呼び出すことができます。 通常この関数を複数回呼び出すデータベースごとにチェックされていることを確認します。 
  
## <a name="requirements"></a>必要条件

Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

