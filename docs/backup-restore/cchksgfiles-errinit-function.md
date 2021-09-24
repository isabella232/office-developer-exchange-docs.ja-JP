---
title: CChkSGFiles.ErrInit 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: '最終更新日: 2013 年 3 月 3 日'
ms.openlocfilehash: ccb5293e35f20328181c4cf1cb5f0eddbb42e03f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516294"
---
# <a name="cchksgfileserrinit-function"></a>CChkSGFiles.ErrInit 関数
  
**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
確認するデータベース、およびトランザクション ログ ファイルのパスとベース名を指定することで **CChkSGFiles** オブジェクトを初期化します。アプリケーションでは、**New** 関数の呼び出しが成功した直後に、この関数を呼び出す必要があります。 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>パラメーター

### <a name="rgwszdb"></a>rgwszDb[]
  
入力パラメーター。確認するデータベースを指定する配列。各配列要素には、確認するデータベースのパスとファイル名を NULL で終了する Unicode 文字列で格納します。
    
### <a name="cdb"></a>cDB
  
入力パラメーター。**rgwszDb** 配列に含まれる有効なデータベース パスの要素数。 
    
#### <a name="wszlogpath"></a>wszLogPath
  
入力パラメーター。確認するトランザクション ログ ファイルのフルパス (NULL で終了する Unicode 文字列の形式)。
    
### <a name="wszbasename"></a>wszBaseName
  
入力パラメーター。Exchange トランザクション ログ ファイルの 3 文字のベース名 (NULL で終了する Unicode 文字列の形式)。
    
### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。 
  
## <a name="remarks"></a>注釈

**ErrInit** 関数により、確認するデータベースとログ ファイルを登録します。この関数は、**New** 関数が呼び出された直後に呼び出す必要があり、その後で、それ以外の **ChkSGFiles** 関数を呼び出します。 
  
すべてのデータベースの名前、ログ ファイルのパス、およびベース名を NULL で終了する Unicode 文字列で指定する必要があります。
  
データベース ファイルのみ、ログ ファイルのみ、またはデータベース ファイルとログ ファイルの両方を確認できます。 ただし、この関数を呼び出す場合、アプリケーションはチェックするエンティティを少なくとも 1 つ指定する必要があります。 **cDB** に 0 (ゼロ) を渡し **、wszLogPath** に NULL を指定すると、エラーが返されます。 
  
**cDB** の値が 0 (ゼロ) 以外の場合 **、rgwszDb** に NULL を渡す場合、エラーが発生します。 データベース ファイルを確認する場合、アプリケーションではデータベース名を指定する必要があります。 
  
**wszBaseName に NULL が渡され、wszLogPath** が NULL ではない場合は、エラーが返されます。  ログ ファイルを確認する場合は、必ずログ ファイルのベース名が必要になります。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合は、そのアプリケーションのシングルスレッドの部分で **ErrInit** 関数を呼び出す必要があります。また、その関数は **CCheckSGFiles** オブジェクトごとに 1 回だけ呼び出すことができます。  
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

