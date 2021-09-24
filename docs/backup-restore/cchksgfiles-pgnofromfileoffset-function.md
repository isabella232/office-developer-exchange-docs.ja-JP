---
title: CChkSGFiles.PgnoFromFileOffset 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: 3e2845cc326520ad875dc8bda52bac3d7c2e2cfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516245"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>CChkSGFiles.PgnoFromFileOffset 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
物理データベース ファイルで指定したバイト インデックスに対応するデータベースの論理ページ番号を返します。ファイル オフセットが無効な場合、またはデータベースに対する **ErrCheckDbHeaders** 関数の呼び出しが行われていない場合、この関数は 0 (ゼロ) を返します。 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>パラメーター

### <a name="ibfileoffset"></a>ibFileOffset
  
入力パラメーター。データベース ファイル内のオフセット (バイト単位)。
    
## <a name="return-value"></a>戻り値

指定したオフセットを含んでいるデータベース ファイルの論理ページ番号。
  
## <a name="remarks"></a>注釈

**ibFileOffset** パラメーターが無効な場合、**PgnoFromFileOffset** 関数は 0 (ゼロ) を返します。 
  

            また、**CCheckSGFiles** インスタンスの **ErrCheckDbHeaders** 関数を呼び出していない場合も、**PgnoFromFileOffset** 関数は 0 (ゼロ) を返します。**ErrCheckDbHeaders** を呼び出すことで、データベース ヘッダーに割り当てられたデータベースのページ サイズとページ数を初期化する必要があります。 
  
**PgnoFromFileOffset** を使用して **、ErrCheckDbPages** を呼び出す準備として **PAGE \_ INFO** 構造要素を入力する必要があります。 **ErrCheckDbPages** への **rgPageInfo** パラメーターは、配列内の各要素が **PAGE_INFO** 構造体であることと、**ulPgno** メンバーの値が正しく初期化されていることを必要とします。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合、**PgnoFromFileOffset** 関数は、そのアプリケーションのシングルスレッドの部分で呼び出すことができます。通常、この関数は確認するデータベースごとに複数回呼び出すことになります。 
  
## <a name="requirements"></a>要件

Exchange Server 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

