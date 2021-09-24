---
title: CChkSGFiles.ErrCheckDbPages 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: '最終更新日: 2013 年 2 月 22 日'
ms.openlocfilehash: e458e4ad552abfebb7611822a6e756bdd2ac6350
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510408"
---
# <a name="cchksgfileserrcheckdbpages-function"></a>CChkSGFiles.ErrCheckDbPages 関数

**適用対象: Exchange Server** 2003 |Exchange Server 2007 |Exchange Server 2010 |Exchange Server 2013
  
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

## <a name="parameters"></a>パラメーター

### <a name="idb"></a>iDb
  
入力パラメーター。**ErrInit** 関数への **rgwszDb[]** パラメーターで指定したデータベースの配列のインデックス。このパラメーターでインデックス指定されたデータベースが確認の対象になります。 
    
### <a name="pvpagebuffer"></a>pvPageBuffer 
  
入力パラメーター。確認対象のデータベース ページを 1 ページ以上格納しているバッファーへのポインター。バッファーのサイズは、**ErrCheckDbHeaders** 関数の **pcbDbPageSize** パラメーターで返されるデータベース ページのサイズの倍数になっている必要があります。呼び出し元のアプリケーションでは、**ErrCheckDbPages** を呼び出す前に、データベース ページのコンテンツでバッファーを満たしておく必要があります。
    
### <a name="cbpagebuffer"></a>cbPageBuffer
  
入力パラメーター。**pvPageBuffer** パラメーターのサイズ (バイト単位)。この値は、**ErrCheckDbHeaders** 関数の **pcbDbPageSize** パラメーターで返されるデータベース ページのサイズの倍数になっている必要があります。 
    
### <a name="rgpageinfo"></a>rgPageInfo[] 
  
入出力パラメーター。 **ErrCheckDbPages** がチェックされる各データベース ページの詳細な結果を入力する **PAGE \_ INFO** 構造体の配列。 **配列には、pvPageBuffer** パラメーターで渡されるデータベース ページごとに 1 つの要素が必要で、各 **PAGE \_ INFO** 構造体の **ulPgno** フィールドは、データベース ページに対応する論理ページ番号に設定する必要があります。 詳細については、このトピックの「備考」を参照してください。 
    
### <a name="cpageinfo"></a>cPageInfo
  
入力パラメーター。**rgPageInfo[]** 配列のエントリ数。この値は、**pvPageBuffer** パラメーターで渡したデータベース ページの数と等しくなっている必要があります。 
    
### <a name="ulflags"></a>ulFlags 
  
オプションの入力パラメーター。この値は、将来使用するために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>戻り値

[ERR](cchksgfiles-err-enumeration.md) 列挙型のエラー コード。 
  
## <a name="remarks"></a>注釈

指定するデータベースは、**ErrInit** 関数に渡したデータベースの配列内のものにする必要があります。また、**ErrCheckDbPages** の前に **ErrCheckDbHeaders** を呼び出す必要もあります。
  
呼び出し元のアプリケーションでは、確認対象のデータベース ページを保持できる大きさのメモリ バッファーを割り当てる必要があります。アプリケーションでは、このバッファーに、1 つ以上の該当するデータベース ページのコンテンツを設定する必要があります。  
  
呼び出し元のアプリケーションは **、ErrCheckDbPages** を呼び出す前に **ErrCheckDbHeaders を呼び出す必要があります**。 この関数は、すべてのデータベース ファイルに含まれる確認対象のすべてのページをカバーするために必要になる回数だけ呼び出しできます。
  
**rgPageInfo[]** パラメーターでは、返される各要素には、PAGE INFO 構造内のデータベース ページに関する **情報が \_ 含** まれる。 **ErrCheckDbPages** 関数がエラーを返す場合、アプリケーションは各 **PAGE \_ INFO** 構造をチェックして、エラーが見つかったページを特定する必要があります。 たとえば、**checksumActual** と **checksumExpected** の値を比較することで、そのデータベース ページでチェックサム エラーが検出されたかどうかがわかります。 
  
**ErrCheckDbPages** は、データベース コンテンツにエラーを検出すると、Windows エラーのイベント ログのエントリを作成します。 
  
**CChkSGFiles** オブジェクトでは、**ErrInit** 関数で登録したすべてのデータベースが実際に確認されたかどうかを判別します。具体的には、**CChkSGFiles** は **ErrCheckDbPages** 関数を使用することで、**ErrCheckDbHeaders** によって示されたデータベース ページ数が実際に検証されたページ数と同じかどうかを判断します。各データベースで適切なページ数が正常にチェックされていなかった場合、**ErrTerm** 関数はエラーを返します。 
  
マルチスレッド アプリケーションで CHKSGFILES を使用している場合、**ErrCheckDbPages** 関数は、そのアプリケーションのシングルスレッドの部分で呼び出すことができます。通常、**ErrCheckDbPages** は確認対象のデータベースごとに複数回呼び出されます。  
  
## <a name="requirements"></a>要件

Exchange 2013 には、CHKSGFILES API の 64 ビット バージョンだけが含まれています。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

