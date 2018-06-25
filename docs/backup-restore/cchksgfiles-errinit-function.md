---
title: CChkSGFiles.ErrInit 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: '最終更新日: 2013 年 3 月 3 日'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758860"
---
# <a name="cchksgfileserrinit-function"></a>CChkSGFiles.ErrInit 関数
  
**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
チェックするデータベースを指定することによって**CChkSGFiles**オブジェクトのパスおよびチェックするトランザクション ログ ファイルの基本名を初期化します。 アプリケーションでは、**新規**の関数の呼び出しに成功した直後にこの関数を呼び出す必要があります。 
  
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

## <a name="parameters"></a>Parameters

### <a name="rgwszdb"></a>rgwszDb
  
入力パラメーター。確認するデータベースを指定する配列。各配列要素には、確認するデータベースのパスとファイル名を NULL で終了する Unicode 文字列で格納します。
    
### <a name="cdb"></a>cDB
  
パラメーターを入力します。 **RgwszDb**配列内の有効なデータベースのパスの要素の数。 
    
#### <a name="wszlogpath"></a>wszLogPath
  
入力パラメーター。確認するトランザクション ログ ファイルのフルパス (NULL で終了する Unicode 文字列の形式)。
    
### <a name="wszbasename"></a>wszBaseName
  
入力パラメーター。Exchange トランザクション ログ ファイルの 3 文字のベース名 (NULL で終了する Unicode 文字列の形式)。
    
### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>�߂�l

[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。 
  
## <a name="remarks"></a>備考

**ErrInit**関数は、データベースとログ ファイルをチェックするを登録します。 **新規**の関数が呼び出されますが、他の**ChkSGFiles**する前に関数が呼び出される後、この関数を呼び出す必要があります。 
  
すべてのデータベースの名前、ログ ファイルのパス、およびベース名を NULL で終了する Unicode 文字列で指定する必要があります。
  
データベース ・ ファイルのみをチェックすることができますのみ、ログ ファイル、またはデータベース ファイルとログ ファイルの両方。 ただし、この関数を呼び出す場合アプリケーションはチェックするには、少なくとも 1 つのエンティティを指定する必要があります。 **WszLogPath**の**cDB**と NULL は 0 (ゼロ) を渡すと、エラーが返されます。 
  
**CDB**の値が 0 (ゼロ) 以外の場合は、 **rgwszDb**に NULL を渡すことと、エラーが発生します。 データベース ファイルをチェックするには、アプリケーションがデータベース名を入力してください。 
  
**WszBaseName**に NULL が渡される**wszLogPath**が NULL でない場合は、エラーが戻ります。 ログ ファイルのベース名は、ログ ファイルをチェックするときに常に必要です。 
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合、アプリケーションの単一の部分に、 **ErrInit**関数を呼び出す必要があり、 **CCheckSGFiles**オブジェクトごとに 1 回のみ呼び出すことができます。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

