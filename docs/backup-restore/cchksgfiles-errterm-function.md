---
title: CChkSGFiles.ErrTerm 関数
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: '最終更新日: 2013 年 2 月 25 日'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758866"
---
# <a name="cchksgfileserrterm-function"></a>CChkSGFiles.ErrTerm 関数
  
**に適用されます:** Exchange Server 2003年 |Exchange Server 2007年 |Exchange Server 2010年 |Exchange Server 2013
  
すべてのデータベース ページとログが正常に検証されたかどうかを示す、データベースとログの検証の全体的な状態を提供します。
  
> [!IMPORTANT]
> ストレージ ・ グループは利用可能な Exchange 2013 です。 CHKSGFILES API では、データベースと Exchange Server 2010 より前のバージョンの Exchange ストレージ ・ グループの下位互換性のため、ストレージ ・ グループを指定できます。 Exchange 2013 のデータベースに対して CHKSGFILES を実行するときは、空の文字列にストレージ ・ グループの識別子を指定するパラメーターを設定してください。 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parameters

### <a name="ulflags"></a>ulFlags
  
オプションの入力パラメーター。この値は、今後の使用のために予約されています。このパラメーターで渡された値は 0 (ゼロ) になります。
    
## <a name="return-value"></a>�߂�l

[エラー](cchksgfiles-err-enumeration.md)の列挙体からのエラー コードです。 
  
## <a name="remarks"></a>備考

**CChkSGFiles**オブジェクトは、 **ErrInit**関数を使用して登録されているすべてのデータベースが実際にチェック アウトするかどうかを決定します。 このオブジェクト関数を使用して、 **ErrCheckDbPages**のことを確認するのには、 **ErrCheckDbHeaders**関数で指定されたページが実際にいることを確認するデータベースの数が同じです。 正しい数の各データベース内のページが正常にチェックされていない場合、 **ErrTerm**関数はエラーを返します。 
  
**ErrCheckDbPages**でチェックするデータベース ページの数が**ErrCheckDbHeaders**で示されるよりも短い場合は、この関数は、Windows イベント ログに、エラーを作成し、 **ErrTerm**には、エラーが返されます。 
  
**ErrCheckDbPages**でチェックするデータベース ページの数が**ErrCheckDbHeaders**で示されるよりも大きい場合は、この関数は、アプリケーションが不必要をチェックするいくつかを示すために Windows イベント ログに警告を作成します。データベースのページが 2 回以上。 この場合、ただし、 **ErrTerm**関数は成功します。 
  
**CChkSGFiles**オブジェクトは、 **ErrInit**に登録されているログ ファイルが実際にチェック アウトするかどうかも決定します。 表示しない場合は、すべてのログが正常にチェック、 **ErrTerm**関数はエラーを返します。 
  
**ErrTerm**にエラーが返されるときも、 **ErrInit**に登録されているすべてのデータベースの検証の状態をチェックすることが見つかると、最初のエラーになります。
  
マルチ スレッド アプリケーションで CHKSGFILES を使用する場合は、シングル スレッド アプリケーションの部分に、 **ErrTerm**関数を呼び出す必要があり、呼び出すことができます 1 回の**CCheckSGFiles**オブジェクトごとに。 
  
## <a name="requirements"></a>必要条件

Exchange 2013 には、CHKSGFILES の 64 ビット バージョンにはのみが含まれます。
  
アプリケーションを実行しているアカウントには、確認するデータベースとログ ファイルに対する読み取りアクセス許可が必要です。
  

